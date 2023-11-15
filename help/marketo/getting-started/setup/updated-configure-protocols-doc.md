---
description: プロトコルの設定に関するドキュメント ( Marketoドキュメント ) を更新しました。製品ドキュメント
title: プロトコルの設定ドキュメントを更新しました
hide: true
hidefromtoc: true
feature: Getting Started
source-git-commit: 1152e81462fb77dd23ff57e26ded7f9b3c02c258
workflow-type: tm+mt
source-wordcount: '2104'
ht-degree: 41%

---

# プロトコルの設定ドキュメントを更新しました {#updated-configure-protocols-doc}

お客様またはお客様の組織が制限的なファイアウォールまたはプロキシサーバー設定を使用している場合、お客様またはネットワーク管理者は、Adobe Marketo Engage が期待通りに動作するように、特定のドメインおよび IP アドレス範囲を許可する必要が生じる場合があります。

以下のプロトコルの実装に関しては、この記事を IT 部門と共有してください。 を使用して Web アクセスを制限する場合許可リストに加えるは、次のドメイン（アスタリスクを含む）を追加して、すべてのMarketoリソースおよび Web ソケットを許可してください。

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

`[YourEmailCNAME]` が Marketo が割り当てたデフォルトのトラッキングリンク [MktoTrackingLink] を以下の形式で指すように、送信されたメール CNAME マーケティングを追加します。\
`[YourEmailCNAME].[YourDomain].com` CNAME 内 `[MktoTrackingLink]`

例：

`pages.abc.com IN CNAME mkto-a0244.com`

>[!NOTE]
>
>`[MktoTrackingLink]` は、デフォルトのブランディングドメインである必要があります。

`3` **マーケティングチームに通知する**

このプロセスが完了したら、マーケティングチームに通知します。

`4`SSL 証明書のプロビジョニングプロセスを開始するには、**[Marketo サポート](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}にお問い合わせください**。

プロセスが完了するまでに最大で 3 営業日かかります。

## 手順 2：Marketo IP の許可リスト {#step-allowlist-marketo-ips}

Marketo を使用してテストメールを送信する（メールの破棄を送信する前のベストプラクティス）と、メールが有効であることを検証するために送信者の IP アドレスに依存するスパム対策システムによってテストメールがブロックされる場合があります。これらのテスト用のメールが届くようにするには、許可リストに Marketo を追加します。

以下の IP アドレスを会社の許可リストに追加します。

94.236.119.0/26

103.237.104.0/22

130.248.172.0/24

130.248.173.0/24

130.248.244.88/29

185.28.196.0/22

192.28.144.0/20

192.28.160.0/19

199.15.212.0/22

一部のスパム対策システムでは、許可リストの IP アドレスの代わりにメールの Return-Path フィールドを使用します。Marketo は複数のメールボックスサブドメインを使用するので、このような場合の最善の方法は「&#42;.mktomail.com」を許可リストに追加することです。その他のスパム対策システムは送信元アドレスに基づいて許可リストに登録します。このような状況では、マーケティンググループがユーザーやリードとの通信に使用するすべての送信（「From」）ドメインを必ず含めてください。

>[!NOTE]
>
>Postini は独自のテクノロジーを採用しており、IP 範囲を許可リストに加えることが必要です。[Postini での許可リストへの登録](https://nation.marketo.com/docs/DOC-1066)を参照してください。

## 手順 3：SPF と DKIM の設定 {#step-set-up-spf-and-dkim}

また、DNS リソースレコード（以下にも示す）に追加する DKIM（ドメインキー識別メール）情報もマーケティングチームから送信されている必要があります。 次の手順に従って DKIM および SPF(Sender Policy Framework) を正しく設定し、更新されたことをマーケティングチームに通知します。

1. SPF を設定するには、DNS エントリに以下の行を追加します。

   `[CompanyDomain]` IN TXT v=spf1 mx ip4:`[CorpIP]`\
   include: mktomail.com ~all

   DNS エントリに既に SPF レコードが存在する場合は、以下のコードを追加します。\
   include: mktomail.com

   CompanyDomain を Web サイトのメインドメイン（例：`(company.com/)`）で置き換え、CorpIP を会社のメールサーバーの IP アドレス（例：255.255.255.255）で置き換えます。Marketo を通じて複数のドメインからメールを送信する場合は、IT スタッフに各ドメインに対してこの行を（1 行で）追加してもらう必要があります。

1. DKIM の場合は、設定するドメインごとに DNS リソースレコードを作成します。 署名する各ドメインのホストレコードと TXT 値を以下に示します。

   `[DKIMDomain1]`：ホストレコードが `[HostRecord1]` で、TXT 値が `[TXTValue1]` です。

   `[DKIMDomain2]`：ホストレコードが `[HostRecord2]` で、TXT 値が `[TXTValue2]` です。

   設定した DKIMDomain ごとに HostRecord と TXTValue をコピーします。 [こちらの説明](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}. IT スタッフがこの手順を完了したら、必ず管理者／メール／DKIM で各ドメインを確認してください。

## 手順 4:DMARC（ドメインベースのメッセージ認証、レポート、準拠）のセットアップ {#set-up-dmarc}

DMARC は、組織がドメインを不正使用から保護するのに役立つ認証プロトコルです。 DMARC は、SPF や DKIM などの既存の認証プロトコルを拡張し、ドメインで認証に失敗した場合に受信者が実行するアクションを受信者サーバーに通知します。 DMARC は現在オプションですが、組織のブランドとレピュテーションをより良く保護するため、強くお勧めします。 Googleや Yahoo などの主なプロバイダーは、2024 年 2 月以降、一括送信者に対して DMARC を使用する必要があります。

DMARC が機能するには、次の DNS TXT レコードの少なくとも 1 つが必要です。

* 有効な SPF
* FROM：ドメインに対する有効な DKIM レコード (Marketo Engageに推奨 )

さらに、FROM: Domain に対して DMARC 固有の DNS TXT レコードが必要です。 必要に応じて、選択した電子メールアドレスを定義して、組織内で DMARC レポートを配置する場所を指定し、レポートを監視できます。

ベストプラクティスとして、DMARC ポリシーを p=none から p=quarantine にエスカレートし、p=reject にエスカレートして DMARC の潜在的な影響を理解し、DMARC ポリシーを SPF と DKIM に緩和的に連携するように設定することを、DMARC の実装を徐々に展開することをお勧めます。

### DMARC ワークフローの例 {#dmarc-example-workflow}

1. DMARC レポートを受け取るように設定されている場合は、次の操作を行う必要があります。

   I.受信および使用するフィードバックおよびレポート (p=none) を分析します。これは、受信者に対して、認証に失敗したメッセージに対して何も実行せず、まだ送信者に電子メールレポートを送信するように指示します。

   2. 正当なメッセージが認証に失敗する場合は、SPF/DKIM の問題を確認および修正します。

   三。 SPF または DKIM が整列し、すべての正当な E メールに認証を渡しているかどうかを確認します。

   四位 レポートをレビューして、SPF/DKIM ポリシーに基づいて期待される結果であることを確認します。

1. ポリシーを (p=quarantine) に調整します。これは、受信側の E メールサーバーに対し、認証に失敗した E メールを強制隔離するよう伝えます（これは通常、これらのメッセージをスパムフォルダーに配置することを意味します）。

   I.レポートをレビューし、期待通りの結果が得られるかを確認します。

1. p=quarantine レベルでのメッセージの動作に満足している場合は、(p=reject) にポリシーを調整できます。 p=reject ポリシーは、認証に失敗したドメインの E メールを受信者に対して完全に拒否（バウンス）するように指示します。 このポリシーを有効にすると、ドメインで 100%認証された電子メールのみがインボックスに配置される機会を得ることができます。

>[!CAUTION]
>
>このポリシーを使用する際は慎重に行い、組織に適しているかどうかを判断してください。

### DMARC レポート {#dmarc-reporting}

DMARC は、SPF/DKIM に失敗した E メールに関するレポートを受け取る機能を備えています。 送信者が DMARC ポリシーの RUA/RUF タグを通じて受信できる認証プロセスの一環として、ISP サービス担当者が生成する 2 つの異なるレポートがあります。

* 集計レポート (RUA):GDPR（一般データ保護規則）の影響を受けやすい PII（個人を特定できる情報）が含まれていません。

* フォレンジックレポート (RUF):GDPR に影響を受ける電子メールアドレスが含まれます。 を利用する前に、GDPR に準拠する必要がある情報の処理方法を内部で確認することをお勧めします。

これらのレポートの主な使用方法は、スプーフィングを試行した電子メールの概要を受け取ることです。 これらは、サードパーティのツールを通じて最もよく消化される、非常に技術的なレポートです。

### DMARC レコードの例 {#example-dmarc-records}

* 最小レコード数： `v=DMARC1; p=none`

* レポートを受け取る電子メールアドレスにリダイレクトするレコード： `v=DMARC1; p=none;  rua=mailto:emaill@domain.com;     ruf=mailto:email@domain.com`

### DMARC タグとその機能 {#dmarc-tags-and-what-they-do}

DMARC レコードには、DMARC タグと呼ばれる複数のコンポーネントが含まれます。 各タグには、DMARC の特定の側面を指定する値が含まれます。

<table>
<thead>
  <tr>
    <th>タグ名 </th>
    <th>必須/オプション </th>
    <th>機能 </th>
    <th>例 </th>
    <th>デフォルト値 </th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>v</td>
    <td>必須</td>
    <td>この DMARC タグは、バージョンを指定します。 現時点では 1 つのバージョンのみなので、v=DMARC1 の固定値になります。</td>
    <td>V=DMARC1 DMARC1</td>
    <td>DMARC1</td>
  </tr>
  <tr>
    <td>p</td>
    <td>必須</td>
    <td>選択された DMARC ポリシーを表示し、認証チェックに失敗したメールをレポート、強制隔離、または拒否するよう受信者に指示します。</td>
    <td>p=なし、強制隔離または却下</td>
    <td>-</td>
  </tr>
  <tr>
    <td>～に対して</td>
    <td>任意</td>
    <td>ドメイン所有者がレポートオプションを指定できるようにします。</td>
    <td>0：すべてが失敗した場合にレポートを生成 
    <br>1：何か失敗した場合にレポートを生成 
    <br>d:DKIM が失敗した場合にレポートを生成 
    <br>s:SPF に失敗した場合にレポートを生成する</td>
    <td>1 （DMARC レポートに推奨）</td>
  </tr>
  <tr>
    <td>pct</td>
    <td>任意</td>
    <td>フィルタリングの対象となるメッセージの割合を示します。</td>
    <td>pct=20</td>
    <td>100</td>
  </tr>
  <tr>
    <td>rua</td>
    <td>オプション（推奨）</td>
    <td>集計レポートが配信される場所を識別します。</td>
    <td>rua=mailto:aggrep@example.com</td>
    <td>-</td>
  </tr>
  <tr>
    <td>ruf</td>
    <td>オプション（推奨）</td>
    <td>法医学レポートがどこに配信されるかを識別します。</td>
    <td>ruf=mailto:authfail@example.com</td>
    <td>-</td>
  </tr>
  <tr>
    <td>sp</td>
    <td>任意</td>
    <td>親ドメインのサブドメインに対して DMARC ポリシーを指定します。</td>
    <td>sp=reject</td>
    <td>-</td>
  </tr>
  <tr>
    <td>アドキム</td>
    <td>任意</td>
    <td>Strict (s) または Relaxed ®のいずれかです。 緩和された整列とは、DKIM 署名で使用されるドメインが「送信者」アドレスのサブドメインになる可能性があることを意味します。 厳密に整列させると、DKIM 署名で使用されるドメインは、送信元アドレスで使用されるドメインと完全に一致する必要があります。</td>
    <td>adkim=r </td>
    <td>r</td>
  </tr>
  <tr>
    <td>aspf</td>
    <td>任意</td>
    <td>Strict (s) または Relaxed ®のいずれかです。 緩和された配置とは、ReturnPath ドメインが From Address のサブドメインになることを意味します。 厳密に整列すると、Return-Path ドメインは From アドレスと完全に一致する必要があります。</td>
    <td>aspf=r</td>
    <td>r</td>
  </tr>
</tbody>
</table>

DMARC とそのすべてのオプションについて詳しくは、 [https://dmarc.org/](https://dmarc.org/){target="_blank"}.

### DMARC とMarketo Engage {#dmarc-and-marketo-engage}

DMARC には、DKIM の調整と SPF の調整の 2 種類があります。

>[!NOTE]
>
>Marketoの DKIM と SPF で DMARC の連携を行うことをお勧めします。

* DKIM-aligned DMARC - DKIM aligned DMARC を設定するには、次の操作を行う必要があります。

   * メッセージの「送信元： 」ドメインに DKIM を設定します。 手順を使用します [この記事では、](help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}.
   * 以前に設定した FROM:/DKIM ドメイン用に DMARC を設定します

* DMARC-aligned SPF — ブランドの Return Path を使用して DMARC aligned SPF を設定するには、次の手順を実行する必要があります。

   * ブランドの Return-Path ドメインの設定
      * 適切な SPF レコードの設定
      * MX レコードを変更して、メールが送信されるデータセンターのデフォルト MX を指すようにします。

   * ブランドの Return-Path ドメイン用の DMARC の設定

* 専用の IP 経由でMarketoからメールを送信する場合で、ブランドのリターンパスをまだ実装していない場合、または既に実装しているかどうかわからない場合は、 [Marketoサポート](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

* Marketoから IP の共有プールを通じてメールを送信する場合は、次の方法で信頼済み IP に該当するかどうかを確認できます。 [ここに適用](http://na-sjg.marketo.com/lp/marketoprivacydemo/Trusted-IP-Sending-Range-Program.html){target="_blank"}. Marketoの信頼済み IP から送信されるユーザーには、ブランド化された Return Path が無料で提供されます。 このプログラムが承認された場合は、Marketoサポートに連絡して、ブランドの Return Path を設定してください。

   * 信頼済み IP：専用 IP の対象とならない 75,000 人/月未満のボリュームのユーザーが送信するために予約された、IP の共有プール。 また、ベストプラクティス要件も満たす必要があります。

* Marketoから共有 IP 経由でメールを送信する場合で、信頼済み IP の条件を満たさず、1 ヶ月に 10 万件を超えるメッセージを送信する場合は、Adobeアカウントチーム（アカウントマネージャー）に連絡して専用 IP を購入する必要があります。

* Marketo内では、厳密な SPF 調整はサポートされておらず、推奨もされていません。

## 手順 5：ドメインの MX レコードの設定 {#step-set-up-mx-records-for-your-domain}

MX レコードを使用すると、返信や自動返信を処理するために、メールを送信するドメインにメールを受け取ることができます。会社ドメインから送信する場合は、既にこの設定が完了している可能性があります。そうでない場合は、通常、会社ドメインの MX レコードにマッピングするように設定できます。

## アウトバウンド IP アドレス {#outbound-ip-addresses}

アウトバウンド接続とは、Marketo Engage がお客様に代わってインターネット上のサーバーに接続するものです。取引先のパートナー／ベンダー、またはご自身の IT 組織では、サーバーへのアクセスを制限するために許可リストを使用する場合があります。その場合、Marketo Engage のアウトバウンド IP アドレスブロックを提供し、許可リストに追加してもらう必要があります。

**Webhook**

スマートキャンペーンの一環として、Marketo Engage [Webhook](/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md){target="_blank"} are an outbound integration mechanism. When a [Call Webhook](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/call-webhook.md){target="_blank"} フローアクションが実行されると、外部 web サービスに HTTP リクエストが行われます。Web サービス公開者が、外部の web サービスが存在するネットワークのファイアウォールで許可リストを使用している場合、公開者は以下に示す IP アドレスブロックを許可リストに追加する必要があります。

**CRM 同期**

Marketo Engage [Salesforce CRM 同期](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/add-an-existing-salesforce-field-to-the-marketo-sync.md){target="_blank"} and [Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md){target="_blank"}は、CRM ベンダーによって公開された API に対して送信 HTTP リクエストを行う統合メカニズムです。お客様の IT 組織が、以下の IP アドレスブロックのいずれからも CRM ベンダーの API へのアクセスをブロックしていないことを確認する必要があります。

**Marketo Engage アウトバウンド IP アドレスブロック**

以下の表は、アウトバウンドコールを行うすべての Marketo Engage サーバーを対象としています。IP 許可リスト、サーバー、ファイアウォール、アクセス制御リスト、セキュリティグループ、またはサードパーティサービスが Marketo Engage からの発信接続を受信するように設定している場合は、以下のリストを使用します。

<table>
 <tbody>
  <tr>
   <th>IP ブロック（CIDR 表記）</th>
  </tr>
  <tr>
   <td>94.236.119.0/26</td>
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
  </tr>
   <tr>
   <td>130.248.168.16</td>
  </tr>
  </tr>
   <tr>
   <td>130.248.168.17</td>
  </tr>
 </tbody>
</table>
