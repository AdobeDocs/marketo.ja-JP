---
unique-page-id: 4720433
description: Marketo のプロトコルの設定 - Marketo ドキュメント - 製品ドキュメント
title: Marketo のプロトコルの設定
exl-id: cf2fd4ac-9229-4e52-bb68-5732b44920ef
feature: Getting Started
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '2131'
ht-degree: 96%

---

# Marketo のプロトコルの設定{#configure-protocols-for-marketo-engage}

お客様またはお客様の組織が制限的なファイアウォールまたはプロキシサーバー設定を使用している場合、お客様またはネットワーク管理者は、Adobe Marketo Engage が期待通りに動作するように、特定のドメインおよび IP アドレス範囲を許可する必要が生じる場合があります。

以下のプロトコルの実装に関するヘルプについては、この記事を IT 部門と共有してください。許可リストを使用して web アクセスを制限する場合は、次のドメイン（アスタリスクを含む）を追加して、すべての Marketo リソースと WebSocket を許可します。

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`
* `*.adobe.net`

## 手順 1：ランディングページとメールの DNS レコードを作成する {#step-create-dns-records-for-landing-pages-and-email}

**トラッキングリンク CNAME**

マーケティングチームから、新しい CNAME レコードに関する 2 件のリクエストが送信されているはずです。1 件目はランディングページの URL 用です。これにより、ランディングページは、Marketo（実際のホスト）ではなく、顧客のドメインを反映した URL で表示されます。2 件目は、Marketo から送信されるメールに含まれるトラッキングリンク用です。

`1` **ランディングページ用の CNAME の追加**

`[YourLandingPageCNAME]`が Marketo のランディングページに割り当てられた一意のアカウント文字列を指すように、DNS レコードに送信したランディングページ CNAME を追加します。ドメイン登録機関のサイトにログインし、ランディングページの CNAME とアカウント文字列を入力します。通常、これには 3 つのフィールドが含まれます。

* エイリアス：`[YourLandingPageCNAME]` と入力します（マーケティングから提供）。
* タイプ：CNAME
* ポイント：`[MunchkinID].mktoweb.com` と入力します（マーケティングから提供）。

`2` **メールトラッキングリンク用の CNAME の追加**

CNAME マーケティングから送信されたメールを追加し、Marketo Engage`[YourEmailCNAME]` 割り当てたデフォルトのトラッキングリンクである [MktoTrackingLink] を、次の形式で指すようにします。
CNAME `[YourEmailCNAME].[YourDomain].com` の `[MktoTrackingLink]`

例：

`pages.abc.com IN CNAME mkto-a0244.com`

>[!NOTE]
>
>`[MktoTrackingLink]` は、デフォルトのブランディングドメインである必要があります。

`3` **マーケティングチームに通知する**

このプロセスが完了したら、マーケティングチームに通知します。

`4` **SSL 証明書のプロビジョニングプロセスを開始するには、[Marketo サポート](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}にお問い合わせください。**

プロセスが完了するまでに最大で 3 営業日かかります。

## 手順 2：Marketo IP の許可リスト {#step-allowlist-marketo-ips}

Marketo を使用してテストメールを送信する（メールの破棄を送信する前のベストプラクティス）と、メールが有効であることを検証するために送信者の IP アドレスに依存するスパム対策システムによってテストメールがブロックされる場合があります。これらのテスト用のメールが届くようにするには、許可リストに Marketo を追加します。

以下の IP アドレスを会社の許可リストに追加します。

103.237.104.0/22

130.248.172.0/24

130.248.173.0/24

130.248.244.88/29

185.28.196.0/22

192.28.144.0/20

192.28.160.0/19

199.15.212.0/22

一部のスパム対策システムでは、許可リストの IP アドレスの代わりにメールの Return-Path フィールドを使用します。Marketo は複数のメールボックスサブドメインを使用するので、このような場合の最善の方法は&#42;「*.mktomail.com」を許可リストに追加することです。その他のスパム対策システムは送信元アドレスに基づいて許可リストに登録します。その他のスパム対策システムは送信元アドレスに基づいて許可リストに登録します。このような状況では、マーケティンググループがユーザーやリードとの通信に使用するすべての送信（「From」）ドメインを必ず含めてください。

>[!NOTE]
>
>Postini は独自のテクノロジーを採用しており、IP 範囲を許可リストに加えることが必要です。[Postini での許可リストへの登録](https://nation.marketo.com/docs/DOC-1066)を参照してください。

## 手順 3：SPF と DKIM の設定 {#step-set-up-spf-and-dkim}

マーケティングチームは、DNS リソースレコードに追加する DKIM（Domain Keys Identified Mail）情報も送信しています（以下も参照）。手順に従って DKIM と SPF（Sender Policy Framework）を正しく設定し、この設定が更新されたことをマーケティングチームに通知します。

1. SPF を設定するには、DNS エントリに以下の行を追加します。

   `[CompanyDomain]` IN TXT v=spf1 mx ip4:`[CorpIP]`
include: mktomail.com ～all

   DNS エントリに既存の SPF レコードがある場合は、次のレコードを追加するだけです。
次を含む：mktomail.com

   CompanyDomain を Web サイトのメインドメイン（例：`(company.com/)`）で置き換え、CorpIP を会社のメールサーバーの IP アドレス（例：&quot;255.255.255.255&quot;）が該当します。 Marketo を通じて複数のドメインからメールを送信する場合は、IT スタッフに各ドメインに対してこの行を（1 行で）追加してもらう必要があります。

1. DKIM の場合は、設定するドメインごとに DNS リソースレコードを作成します。署名する各ドメインのホストレコードと TXT 値を以下に示します。

   `[DKIMDomain1]`：ホストレコードが `[HostRecord1]` で、TXT 値が `[TXTValue1]` です。

   `[DKIMDomain2]`：ホストレコードが `[HostRecord2]` で、TXT 値が `[TXTValue2]` です。

   [こちらの手順](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}に従って、設定した DKIMDomain ごとに HostRecord と TXTValue をコピーします。IT スタッフがこの手順を完了したら、必ず管理者／メール／DKIM で各ドメインを確認してください。

## 手順 4：DMARC の設定 {#set-up-dmarc}

DMARC（Domain-based Message Authentication, Reporting &amp; Conformance）は、組織がドメインを不正使用から保護するのに役立つ認証プロトコルです。DMARC は、SPF や DKIM などの既存の認証プロトコルを拡張して、ドメインで認証の失敗が発生した場合に受信者サーバーで実行する必要があるアクションを通知します。DMARC は現在オプションですが、組織のブランドとレピュテーションをより良く保護できるので、DMARC を使用することを強くお勧めします。Google や Yahoo などの大手プロバイダーは、2024年2月から一括送信者に DMARC の使用を義務付けます。

DMARC が機能するには、次の DNS TXT レコードの 1 つ以上が必要です。

* 有効な SPF
* 送信元：ドメインに対する有効な DKIM レコード（Marketo Engage に推奨）

さらに、送信元：ドメインに対して DMARC 固有の DNS TXT レコードが必要です。オプションで、選択したメールアドレスを定義して、組織内の DMARC レポートの送信先を指定できるので、レポートを監視できます。

ベストプラクティスとして、DMARC の潜在的な影響を理解し、SPF と DKIM の整列を緩和するように DMARC ポリシーを設定するにつれて、DMARC ポリシーを p=none、p=quarantine、p=reject にエスカレートすることで、DMARC 実装をゆっくりロールアウトすることをお勧めします。

### DMARC のワークフローの例 {#dmarc-example-workflow}

1. DMARC レポートを受信するように設定している場合は、次の操作を行う必要があります。

   (1) 受信して使用するフィードバックとレポートを分析します（p=none）。これは、認証に失敗したメッセージに対して何もアクションを実行しないように受信者に指示しますが、まだ送信者にメールレポートを送信します。

   (2) 正当なメッセージが認証に失敗する場合は、SPF／DKIM に関する問題を確認して修正します。

   (3) SPF または DKIM が整列され、すべての正規メールの認証に合格しているかどうかを確認します。

   (4) レポートを確認して、結果が SPF／DKIM ポリシーに基づいて期待どおりであることを確認します。

1. ポリシーを（p=quarantine）に調整します。これにより、認証に失敗したメールを強制隔離するように受信メールサーバーに通知されます（これは通常、メッセージをスパムフォルダーに配置することを意味します）。

   (1) レポートを確認して、結果が期待どおりであることを確認します。

1. p=quarantine レベルでのメッセージの動作に満足している場合は、ポリシーを（p=reject）に調整できます。p=reject ポリシーは、認証に失敗したドメイン宛てのメールを完全に拒否（バウンス）するように受信者に通知します。このポリシーを有効にすると、ドメインによって 100％認証されたことが確認されたメールのみがインボックスに配置される可能性があります。

>[!CAUTION]
>
>このポリシーは慎重に使用し、組織に対して適切かどうかを判断します。

### DMARC レポート {#dmarc-reporting}

DMARC は、SPF／DKIM に失敗したメールに関するレポートを受信する機能を備えています。認証プロセスの一部として ISP サービサーによって生成される 2 つの異なるレポートがあり、送信者は DMARC ポリシーの RUA／RUF タグを通じて受信できます。

* 集計レポート（RUA）：GDPR（EU 一般データ保護規則）の対象となる PII（個人を特定できる情報）は含まれません。

* フォレンジックレポート（RUF）：GDPR の対象となるメールアドレスが含まれます。利用する前に、GDPR に準拠する必要がある情報の処理方法を社内で確認することをお勧めします。

これらのレポートの主な使用方法は、スプーフィングが試みられたメールの概要を取得することです。これらは技術的なレポートであり、サードパーティのツールを使用するのが最も効果的です。

### DMARC レコードの例 {#example-dmarc-records}

* 最低限のレコード：`v=DMARC1; p=none`

* レポートを受信するメールアドレスに指示するレコード：`v=DMARC1; p=none;  rua=mailto:emaill@domain.com;     ruf=mailto:email@domain.com`

### DMARC タグとその機能 {#dmarc-tags-and-what-they-do}

DMARC レコードには、DMARC タグと呼ばれる複数のコンポーネントがあります。各タグには、DMARC の特定の側面を指定する値があります。

<table>
<thead>
  <tr>
    <th>タグ名 </th>
    <th>必須／オプション </th>
    <th>機能 </th>
    <th>例 </th>
    <th>デフォルト値 </th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>v</td>
    <td>必須</td>
    <td>この DMARC タグは、バージョンを指定します。現時点ではバージョンが 1 つしかないので、v=DMARC1 の固定値になります</td>
    <td>V=DMARC1 DMARC1</td>
    <td>DMARC1</td>
  </tr>
  <tr>
    <td>p</td>
    <td>必須</td>
    <td>選択された DMARC ポリシーを表示し、認証チェックに失敗したメールを報告、強制隔離または却下するよう受信者に指示します。</td>
    <td>p=なし、強制隔離または却下</td>
    <td>-</td>
  </tr>
  <tr>
    <td>fo</td>
    <td>オプション</td>
    <td>ドメイン所有者はレポートオプションを指定できます。</td>
    <td>0：すべてが失敗した場合にレポートを生成
    <br>1：失敗した場合にレポートを生成する
    <br>d: DKIMが失敗した場合にレポートを生成
    <br>s:SPF が失敗した場合にレポートを生成</td>
    <td>1（DMARC レポートに推奨）</td>
  </tr>
  <tr>
    <td>pct</td>
    <td>オプション</td>
    <td>フィルタリングの対象となるメッセージの割合を示します。</td>
    <td>pct=20</td>
    <td>100</td>
  </tr>
  <tr>
    <td>rua</td>
    <td>オプション（推奨）</td>
    <td>集計レポートの配信先を識別します。</td>
    <td>rua=mailto:aggrep@example.com</td>
    <td>-</td>
  </tr>
  <tr>
    <td>ruf</td>
    <td>オプション（推奨）</td>
    <td>フォレンジックレポートの配信先を識別します。</td>
    <td>ruf=mailto:authfail@example.com</td>
    <td>-</td>
  </tr>
  <tr>
    <td>sp</td>
    <td>オプション</td>
    <td>親ドメインのサブドメインに対して DMARC ポリシーを指定します。</td>
    <td>sp=reject</td>
    <td>-</td>
  </tr>
  <tr>
    <td>adkim</td>
    <td>オプション</td>
    <td>Strict (s) または Relaxed ® のいずれかになります。Relaxed 整列では、DKIM 署名で使用されるドメインが「送信元」アドレスのサブドメインになる可能性があります。Strict 整列では、DKIM 署名で使用されるドメインが送信元アドレスで使用されるドメインと完全に一致する必要があります。</td>
    <td>adkim=r </td>
    <td>r</td>
  </tr>
  <tr>
    <td>aspf</td>
    <td>オプション</td>
    <td>Strict (s) または Relaxed ® のいずれかになります。Relaxed 整列では、ReturnPath ドメインが送信元アドレスのサブドメインできることを意味します。Strict 整列では、Return-Path ドメインが送信元アドレスと完全に一致する必要があります。</td>
    <td>aspf=r</td>
    <td>r</td>
  </tr>
</tbody>
</table>

DMARC とそのすべてのオプションについて詳しくは、[https://dmarc.org/](https://dmarc.org/){target="_blank"}を参照してください。

### DMARC と Marketo Engage {#dmarc-and-marketo-engage}

DMARC の整列には、DKIM 整列と SPF 整列の 2 つのタイプがあります。

>[!NOTE]
>
>Marketo では、DKIM と SPF で DMARC の整列を行うことをお勧めします。

* DKIM に整列された DMARC - DKIM に整列された DMARC を設定するには、以下を行う必要があります。

   * メッセージの送信元ドメインに対して DKIM を設定します。[この記事](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}の手順に従ってください。
   * 以前に設定した送信元／DKIM ドメインに対して DMARC を設定します

* DMARC に整列された SPF - DMARC に整列された SPF をブランドの Return-Path を通じて設定するには、以下を行う必要があります。

   * ブランドの Return-Path ドメインを設定します
      * 適切な SPF レコードを設定します
      * メールの送信元となるデータセンターのデフォルトの MX を指すように MX レコードを変更します

   * ブランドの Return-Path ドメインに対して DMARC を設定します

* 専用 IP を通じて Marketo からメールを送信していて、ブランドの Return-Path をまだ実装していない場合や、実装しているかどうかわからない場合は、[Marketo サポート](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}でチケットを開いてください。

* IP の共有プールを通じて Marketo からメールを送信している場合は、[こちらで申請](https://na-sjg.marketo.com/lp/marketoprivacydemo/Trusted-IP-Sending-Range-Program.html){target="_blank"}することで、信頼済み IP の資格があるかどうかを確認できます。Marketo の信頼済み IP から送信するユーザには、ブランドの Return-Path が無料で提供されます。このプログラムに対して承認された場合は、Marketo サポートに連絡してブランドの Return-Path を設定してください。

   * 信頼済み IP：専用 IP の資格がなく、月あたりの送信メッセージが 75,000 件未満の低メッセージ量ユーザ用に予約された共有 IP プール。また、これらのユーザは、ベストプラクティスの要件も満たす必要があります。

* 共有 IP を通じて Marketo からメールを送信していて、信頼済み IP の資格がなく、毎月 100,000 件を超えるメッセージを送信している場合は、アドビのアカウントチーム（アカウントマネージャー）に連絡して専用 IP を購入する必要があります。

* Strict SPF 整列は Marketo 内ではサポートされておらず、推奨されてもいません。

## 手順 5：ドメインの MX レコードの設定 {#step-set-up-mx-records-for-your-domain}

MX レコードを使用すると、メールの送信元のドメインに対するメールを受信して、返信や自動返信を処理することができます。会社ドメインから送信する場合は、既にこの設定が完了している可能性があります。そうでない場合は、通常、会社ドメインの MX レコードにマッピングするように設定できます。

## アウトバウンド IP アドレス {#outbound-ip-addresses}

アウトバウンド接続とは、Marketo Engage がお客様に代わってインターネット上のサーバーに接続するものです。取引先のパートナー／ベンダー、またはご自身の IT 組織では、サーバーへのアクセスを制限するために許可リストを使用する場合があります。その場合、Marketo Engage のアウトバウンド IP アドレスブロックを提供し、許可リストに追加してもらう必要があります。

**Webhook**

Marketo Engage[Webhook](/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md){target="_blank"}は、アウトバウンド統合メカニズムです。スマートキャンペーンの一部として[ Webhook を呼び出し](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/call-webhook.md){target="_blank"}フローアクションが実行されると、外部の web サービスに対して HTTP リクエストが行われます。 Web サービス公開者が、外部の web サービスが存在するネットワークのファイアウォールで許可リストを使用している場合、公開者は以下に示す IP アドレスブロックを許可リストに追加する必要があります。

**CRM 同期**

Marketo Engage[Salesforce CRM 同期](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/add-an-existing-salesforce-field-to-the-marketo-sync.md){target="_blank"}と[ Microsoft Dynamics同期](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md){target="_blank"}は、CRM ベンダーによって公開された API へのアウトバウンド HTTP リクエストを行う統合メカニズムです。 お客様の IT 組織が、以下の IP アドレスブロックのいずれからも CRM ベンダーの API へのアクセスをブロックしていないことを確認する必要があります。

**Marketo Engage アウトバウンド IP アドレスブロック**

以下の表は、アウトバウンドコールを行うすべての Marketo Engage サーバーを対象としています。IP 許可リスト、サーバー、ファイアウォール、アクセス制御リスト、セキュリティグループ、またはサードパーティサービスが Marketo Engage からの発信接続を受信するように設定している場合は、以下のリストを使用します。

<table>
 <tbody>
  <tr>
   <th>IP ブロック（CIDR 表記）</th>
  </tr>
  <tr>
   <td>103.237.104.0/22</td>
  </tr>
   <tr>
   <td>130.248.172.0/24</td>
  </tr>
   <tr>
   <td>130.248.173.0/24</td>
  </tr>
  <tr>
   <td>130.248.244.88/29</td>
  </tr>
  <tr>
   <td>185.28.196.0/22</td>
  </tr>
  <tr>
   <td>192.28.144.0/20</td>
  </tr>
  <tr>
   <td>192.28.160.0/19</td>
  </tr>
  <tr>
   <td>199.15.212.0/22</td>
  </tr>
 </tbody>
</table>

<table>
 <tbody>
  <tr>
   <th>個別の IP アドレス</th>
  </tr>
  <tr>
   <td>13.237.155.207</td>
  </tr>
   <tr>
   <td>13.55.192.247</td>
  </tr>
  <tr>
   <td>18.200.201.81</td>
  </tr>
  <tr>
   <td>34.247.24.245</td>
  </tr>
  <tr>
   <td>35.165.244.220</td>
  </tr>
  <tr>
   <td>44.235.171.179</td>
  </tr>
  <tr>
   <td>52.20.211.99</td>
  </tr>
  <tr>
   <td>52.64.109.86</td>
  </tr>
  <tr>
   <td>54.160.246.246</td>
  </tr>
  <tr>
   <td>54.212.167.17</td>
  </tr>
  <tr>
   <td>54.220.138.65</td>
  </tr>
   <tr>
   <td>54.237.141.197</td>
  </tr>
  <tr>
   <td>124.47.174.193</td>
  </tr>
  <tr>
   <td>130.248.168.16</td>
  </tr>
   <tr>
   <td>130.248.168.17</td>
  </tr>
  <tr>
   <td>199.15.213.245</td>
  </tr>
  <tr>
   <td>199.15.215.245</td>
  </tr>
 </tbody>
</table>
