---
unique-page-id: 4720433
description: Marketo のプロトコルの設定 - Marketo ドキュメント - 製品ドキュメント
title: Marketo のプロトコルの設定
exl-id: cf2fd4ac-9229-4e52-bb68-5732b44920ef
source-git-commit: 6c1699ce986608e8b9d991f21fd649f9330e3d12
workflow-type: ht
source-wordcount: '1021'
ht-degree: 100%

---

# Marketo のプロトコルの設定 {#configure-protocols-for-marketo}

お客様またはお客様の組織が制限的なファイアウォールまたはプロキシサーバー設定を使用している場合、お客様またはネットワーク管理者は、Adobe Marketo Engage が期待通りに動作するように、特定のドメインおよび IP アドレス範囲を許可する必要が生じる場合があります。

## ブランディングキャンペーンのランディングページとメール {#branded-campaign-landing-pages-and-emails}

マーケティンググループが Marketo を使用して、ブランドキャンペーンのランディングページとメールを作成しています。これらのランディングページとメールが確実に機能するように、IT 部門の支援が必要です。次のプロトコルを、マーケティンググループからメールで送信された情報と共に設定してください。

この記事は、これらのプロトコルを導入する企業の IT 部門と共有する必要があります。

IT チームが許可リストを使用して Web アクセスを制限している場合は、次のドメイン（アスタリスクを含む）を追加して、すべての Marketo リソースと WebSocket を許可するように依頼してください。

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`

## 手順 1：ランディングページとメールの DNS レコードを作成する {#step-create-dns-records-for-landing-pages-and-email}

**トラッキングリンク CNAME**

マーケティングチームから、新しい CNAME レコードに関する 2 件のリクエストが送信されているはずです。1 件目はランディングページの URL 用です。これにより、ランディングページは、Marketo（実際のホスト）ではなく、顧客のドメインを反映した URL で表示されます。2 件目は、Marketo から送信されるメールに含まれるトラッキングリンク用です。

`1` **ランディングページ用の CNAME の追加**

`[YourLandingPageCNAME]`が Marketo のランディングページに割り当てられた一意のアカウント文字列を指すように、DNS レコードに送信したランディングページ CNAME を追加します。ドメイン登録機関のサイトにログインし、ランディングページの CNAME とアカウント文字列を入力します。通常、これには 3 つのフィールドが含まれます。

* エイリアス：`[YourLandingPageCNAME]` と入力します（マーケティングから提供）。
* タイプ：CNAME
* ポイント：`[MunchkinID].mktoweb.com` と入力します（マーケティングから提供）。

`2` **メールトラッキングリンク用の CNAME の追加**

`[YourEmailCNAME]` が Marketo が割り当てたデフォルトのトラッキングリンク [MktoTrackingLink] を次の形式で指すように、送信されたメール CNAME マーケティングを追加します。\
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

次の IP アドレスを会社の許可リストに追加します。

199.15.212.0/22\
192.28.144.0/20
192.28.160.0/19\
185.28.196.0/22\
130.248.172.0/24\
130.248.173.0/24\
103.237.104.0/22\
94.236.119.0/26

一部のスパム対策システムでは、許可リストの IP アドレスの代わりにメールの Return-Path フィールドを使用します。Marketo は複数のメールボックスサブドメインを使用するため、このような場合の最善の方法は「&#42;.mktomail.com」を許可リストに追加することです。その他のスパム対策システムは送信元アドレスに基づいて許可リストに登録します。このような状況では、マーケティンググループがユーザやリードとの通信に使用するすべての送信（「From」）ドメインを必ず含めてください。

>[!NOTE]
>
>Postini は独自のテクノロジーを採用しており、IP 範囲を許可リストに加えることが必要です。[Postini での許可リストへの登録](https://nation.marketo.com/docs/DOC-1066)を参照してください。

## 手順 3：SPF と DKIM の設定 {#step-set-up-spf-and-dkim}

また、マーケティングチームから、DNS リソースレコードに追加する DKIM 情報が送信されている必要があります（以下も参照）。手順に従って DKIM と SPF を正しく設定し、この設定が更新されたことをマーケティングチームに通知します。

1. SPF を設定するには、DNS エントリに次の行を追加します。

   `[CompanyDomain]` IN TXT v=spf1 mx ip4:`[CorpIP]`\
   include: mktomail.com ~all

   DNS エントリに既に SPF レコードが存在する場合は、次のコードを追加します。\
   include: mktomail.com

   CompanyDomain を Web サイトのメインドメイン（例：`(company.com/)`）で置き換え、CorpIP を会社のメールサーバーの IP アドレス（例：255.255.255.255）で置き換えます。Marketo を通じて複数のドメインからメールを送信する場合は、IT スタッフに各ドメインに対してこの行を（1 行で）追加してもらう必要があります。

1. DKIM の場合は、設定するドメインごとに DNS リソースレコードを作成します。署名する各ドメインのホストレコードと TXT 値を次に示します。

   `[DKIMDomain1]`：ホストレコードが `[HostRecord1]` で、TXT 値が `[TXTValue1]` です。

   `[DKIMDomain2]`：ホストレコードが `[HostRecord2]` で、TXT 値が `[TXTValue2]` です。

   [](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}に示す手順に従って、設定した DKIMDomain ごとに HostRecord と TXTValue をコピーします。IT スタッフがこの手順を完了したら、必ず管理者／メール／DKIM で各ドメインを確認してください。

## 手順 4：ドメインの MX レコードの設定 {#step-set-up-mx-records-for-your-domain}

MX レコードを使用すると、返信や自動返信を処理するために、メールを送信するドメインにメールを受け取ることができます。会社ドメインから送信する場合は、既にこの設定が完了している可能性があります。そうでない場合は、通常、会社ドメインの MX レコードにマッピングするように設定できます。

## アウトバウンド IP アドレス {#outbound-ip-addresses}

アウトバウンド接続とは、Marketo Engage がお客様に代わってインターネット上のサーバーに接続するものです。取引先のパートナー／ベンダー、またはご自身の IT 組織では、サーバーへのアクセスを制限するために許可リストを使用する場合があります。その場合、Marketo Engage のアウトバウンド IP アドレスブロックを提供し、許可リストに追加してもらう必要があります。

**Webhook**

スマートキャンペーンの一環として、Marketo Engage [Webhook](/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md){target="_blank"} are an outbound integration mechanism. When a [Call Webhook](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/call-webhook.md){target="_blank"} フローアクションが実行されると、外部 web サービスに HTTP リクエストが行われます。Web サービス公開者が、外部の web サービスが存在するネットワークのファイアウォールで許可リストを使用している場合、公開者は以下に示す IP アドレスブロックを許可リストに追加する必要があります。

**CRM 同期**

Marketo Engage [Salesforce CRM 同期](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/add-an-existing-salesforce-field-to-the-marketo-sync.md){target="_blank"} and [Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md){target="_blank"}は、CRM ベンダーによって公開された API に対して送信 HTTP リクエストを行う統合メカニズムです。お客様の IT 組織が、以下の IP アドレスブロックのいずれからも CRM ベンダーの API へのアクセスをブロックしていないことを確認する必要があります。

**Marketo Engage アウトバウンド IP アドレスブロック**

次の表は、アウトバウンドコールを行うすべての Marketo Engage サーバーを対象としています。IP 許可リスト、サーバー、ファイアウォール、アクセス制御リスト、セキュリティグループ、またはサードパーティサービスが Marketo Engage からの発信接続を受信するように設定している場合は、以下のリストを使用します。

<table>
 <tbody>
  <tr>
   <th>IP ブロック（CIDR 表記）</th>
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
   <tr>
   <td>185.28.196.0/22</td>
  </tr>
   <tr>
   <td>130.248.172.0/24</td>
  </tr>
   <tr>
   <td>130.248.173.0/24</td>
  </tr>
  <tr>
   <td>103.237.104.0/22</td>
  </tr>
  <tr>
   <td>94.236.119.0/26</td>
  </tr>
 </tbody>
</table>

<table>
 <tbody>
  <tr>
   <th>個人の IP アドレス</th>
  </tr>
  <tr>
   <td>54.212.167.17</td>
  </tr>
   <tr>
   <td>44.235.171.179</td>
  </tr>
   <tr>
   <td>35.165.244.220</td>
  </tr>
   <tr>
   <td>52.20.211.99</td>
  </tr>
   <tr>
   <td>54.237.141.197</td>
  </tr>
  <tr>
   <td>54.160.246.246</td>
  </tr>
   <tr>
   <td>18.200.201.81</td>
  </tr>
  <tr>
   <td>34.247.24.245</td>
  </tr>
   <tr>
   <td>54.220.138.65</td>
  </tr>
  <tr>
   <td>13.237.155.207</td>
  </tr>
   <tr>
   <td>13.55.192.247</td>
  </tr>
  <tr>
   <td>52.64.109.86</td>
  </tr>
 </tbody>
</table>

