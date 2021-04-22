---
unique-page-id: 4720433
description: Marketoのプロトコルの設定 —Marketoドキュメント — 製品ドキュメント
title: Marketoのプロトコルの設定
exl-id: cf2fd4ac-9229-4e52-bb68-5732b44920ef
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '712'
ht-degree: 1%

---

# Marketoのプロトコルの設定{#configure-protocols-for-marketo}

マーケティンググループがMarketoを使用してブランドキャンペーンのランディングページや電子メールを作成している。 これらのランディングページや電子メールが確実に機能するように、IT部門から少し支援が必要です。 次のプロトコルを、マーケティンググループから電子メールで送信されるべき情報と共に設定してください。

この記事は、これらのプロトコルを実装したい会社のIT部門と共有する必要があります。

>[!NOTE]
>
>ITチームがMarketoを使用したWebアクセスを制限し許可リストている場合は、すべてのリソースとWebソケットを許可するために、次のドメイン（アスタリスクを含む）を追加するように依頼してください。

* `*.marketo.com`

* `*.marketodesigner.com`

* `*.mktoweb.com`

## 手順1:ランディングページと電子メールのDNSレコードの作成{#step-create-dns-records-for-landing-pages-and-email}

**トラッキングリンクCNAME**

マーケティングチームから、新しいCNAMEレコードに関する2つのリクエストが送信されている必要があります。 1つ目はランディングページURL用です。これにより、ランディングページは、Marketo（実際のホスト）ではなく、ドメインを反映したURLで表示されます。 2つ目は、Marketoから送信される電子メールに含まれるトラッキングリンクです。

`1` **ランディングページ追加のCNAME**

DNSレコードに追加送信されたランディングページCNAME。`[YourLandingPageCNAME]`は、Marketoランディングページに割り当てられた一意のアカウント文字列を指すようにします。 ドメイン登録機関のサイトにログインし、ランディングページのCNAMEとアカウント文字列を入力します。 通常、これには次の3つのフィールドが含まれます。

* エイリアス：`[YourLandingPageCNAME]`を入力（マーケティングから提供）
* タイプ：CNAME
* ポイント先：`[MarketoAccountString].mktoweb.com`を入力（マーケティングから提供）

`2` **E メールトラッキングログ追加リンクのCNAME**

電子メール追加のCNAMEマーケティングからユーザーが送信されたので、`[YourEmailCNAME]`が、Marketoが割り当てたデフォルトのトラッキングリンク[MktoTrackingLink]を次の形式で指すように指定します。\
`[YourEmailCNAME].[YourDomain].com` CNAME内  `[MktoTrackingLink]`

次に例を示します。

`pages.abc.com IN CNAME mkto-a0244.com`

`3` **マーケティングチームに通知**

この処理が完了したら、マーケティングチームに通知します。

## 手順2:許可リストMarketoIP {#step-allowlist-marketo-ips}

マーケティンググループがMarketoを使用してテスト電子メール（電子メールの発信前のベストプラクティス）を送信する場合、送信者のIPアドレスに依存するスパム対策システムによってテスト電子メールがブロックされることがあります。 テスト用の電子メールが届くようにするには、許可リストMarketoにを追加します。

追加会社の許可リストに送信するIPアドレス:

199.15.212.0/22\
192.28.144.0/20
192.28.160.0/19\
185.28.196.0/22\
130.248.172.0/24\
130.248.173.0/24\
103.237.104.0/22\
94.236.119.0/26

一部のスパム対策システムでは、許可するIPアドレスの代わりに電子メールのReturn-Pathフィールドを使用します。 Marketoでは複数のメールボックスサブドメインを使用するので、この場合の最善の方法は許可リスト「*.mktomail.com」です。 送信元アドレスに基づくその他の許可リストスパム対策システムの。 このような場合は、マーケティンググループが人やリードとの通信に使用するすべての送信ドメイン(「From」)を必ず含めてください。

>[!NOTE]
>
>Postiniは独自のテクノロジーを採用しており、許可リストに加えるのIP範囲が必要です。 [許可リストに加えるをPostini](https://nation.marketo.com/docs/DOC-1066)と共に参照。

## 手順3:SPFとDKIMの設定{#step-set-up-spf-and-dkim}

また、マーケティングチームから、DNSリソースレコードに追加するDKIM情報を送信する必要があります（以下にも示します）。 手順に従ってDKIMとSPFを正しく設定し、更新されたことをマーケティングチームに通知します。

1. SPFを設定するには、DNSエントリに次の行を追加します。

   `[CompanyDomain]` TXT v=spf1 mx ip4内：`[CorpIP]`\
   含める：mktomail.com ～all

   DNSエントリに既にSPFレコードが存在する場合は、次を追加します。\
   含める：mktomail.com

   CompanyDomainをWebサイトのメインドメイン(例：&quot;`(company.com/)`&quot;)とCorpIP (例： &quot;255.255.255.255&quot;)。 複数のドメインからMarketo経由で電子メールを送信する場合は、ITスタッフに各ドメインに対してこの行を（1行で）追加してもらう必要があります。

1. DKIMの場合、セットアップする各ドメインに対してDNSリソースレコードを作成します。 署名する各ドメインのホストレコードとTXT値を以下に示します。

   `[DKIMDomain1]`:「Host Record」 `[HostRecord1]` はで、「TXT Value」はで `[TXTValue1]`す。

   `[DKIMDomain2]`:「Host Record」 `[HostRecord2]` はで、「TXT Value」はで `[TXTValue2]`す。

   [](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md)の指示に従って、設定した各DKIMDomainのHostRecordとTXTValueをコピーします。 ITスタッフがこの手順を完了した後は、管理者/電子メール/DKIMで各ドメインを確認するのを忘れないでください。

## 手順4:ドメイン{#step-set-up-mx-records-for-your-domain}のMXレコードの設定

MXレコードを使用すると、返信や自動返信を処理するために、電子メールの送信元のドメインにメールを受信できます。 会社ドメインから送信する場合は、既にこの設定が行われている可能性があります。 そうでない場合は、通常、会社ドメインのMXレコードにマップするように設定できます。
