---
unique-page-id: 4720433
description: Marketorのプロトコルの設定 — Marketto Docs — 製品ドキュメント
title: Marketorのプロトコルの設定
translation-type: tm+mt
source-git-commit: 23428a6e0ba9b2108a8f2f7dd6a69929dd069834
workflow-type: tm+mt
source-wordcount: '703'
ht-degree: 1%

---


# Marketorのプロトコルの設定 {#configure-protocols-for-marketo}

マーケティンググループがマーケティングを使用してブランドのキャンペーンランディングページや電子メールを作成している。 これらのランディングページや電子メールが確実に機能するように、IT部門から少し支援が必要です。 次のプロトコルを、マーケティンググループから電子メールで送信されるべき情報と共に設定してください。

>[!NOTE]
>
>この記事は、会社のIT部門がこれらのプロトコルの実装を希望する場合に表示されます。

## 手順1:ランディングページと電子メールのDNSレコードの作成 {#step-create-dns-records-for-landing-pages-and-email}

**トラッキングリンクCNAME**

マーケティングチームから、新しいCNAMEレコードに関する2つのリクエストが送信されている必要があります。 1つ目はランディングページURL用です。これにより、ランディングページは、Marketo（実際のホスト）ではなく、自分のドメインを反映したURLで表示されます。 2つ目の引数は、Marketoから送信される電子メールに含まれるトラッキングリンクです。

1 -ランディングページの **追加CNAME**

DNSレコ追加ードに送信されたランディングページCNAME。これにより、Markettoランディングページに割り当てられている一意のアカウント文字列が参照されます。 `[YourLandingPageCNAME]` ドメイン登録機関のサイトにログインし、ランディングページのCNAMEとアカウント文字列を入力します。 通常、これには次の3つのフィールドが含まれます。

・エイリアス：入力 `[YourLandingPageCNAME]` （マーケティングによって提供）・タイプ：CNAME\
・ポイント先：入力 `[MarketoAccountString].mktoweb.com` （マーケティングから提供）

2 -E メールトラッキングログリンクの **追加CNAME**

電子メール追加のCNAMEマーケティングから送信されたので、Marketorが割り当てたデフォルトのトラッキングリンクである `[YourEmailCNAME]`[]MktoTrackingLinkを次の形式で参照します。\
`[YourEmailCNAME].[YourDomain].com` CNAME内 `[MktoTrackingLink]`

次に例を示します。

`pages.abc.com IN CNAME mkto-a0244.com`

3 — マーケティングチーム **に通知**

この処理が完了したら、マーケティングチームに通知します。

## 手順2:許可リストマーケティングIP {#step-allowlist-marketo-ips}

マーケティンググループがMarketoを使用してテスト電子メール（電子メールの発行を送信する前のベストプラクティス）を送信する場合、送信者のIPアドレスに依存して電子メールが有効であることを確認するスパム対策システムによってテスト電子メールがブロックされることがあります。 これらのテスト電子メールが届くようにするには、許可リストにマーケティングツールを追加します。

会社の追加許可リストに送信するIPアドレス：

199.15.212.0/22\
192.28.144.0/20\
192.28.160.0/19\
185.28.196.0/22\
130.248.172.0/24\
130.248.173.0/24\
103.237.104.0/22\
94.236.119.0/26

一部のスパム対策システムでは、許可するIPアドレスの代わりに電子メールのReturn-Pathフィールドを使用します。 このような場合、最善の方法は許可リスト「*.mktomail.com」です。これは、Marketoが複数のメールボックスサブドメインを使用するためです。 送信元アドレスに基づくその他のスパム対策システム許可リスト。 このような場合は、マーケティンググループが人やリードとの通信に使用するすべての送信ドメイン(「From」)を必ず含めてください。

>[!NOTE]
>
>Postiniでは、独自のテクノロジーを採用しており、IP範囲の許可が必要です。 Postiniを使用した [許可リストを参照してください](http://nation.marketo.com/docs/DOC-1066)。

## 手順3:SPFとDKIMの設定 {#step-set-up-spf-and-dkim}

また、マーケティングチームから、DNSリソースレコードに追加するDKIM情報を送信する必要があります（以下にも示します）。 手順に従ってDKIMとSPFを正しく設定し、更新されたことをマーケティングチームに通知します。

1. SPFを設定するには、DNSエントリに次の行を追加します。

   `[CompanyDomain]` TXT v=spf1 mx ip4内：`[CorpIP]`\
   含める： [mktomail.com](http://mktomail.com/) ～all

   DNSエントリに既にSPFレコードが存在する場合は、次を追加します。\
   含める： [mktomail.com](http://mktomail.com)

   CompanyDomainをWebサイトのメインドメイン(例：「`(company.com/)`」)およびCorpIPと企業の電子メールサーバーのIPアドレス( &quot;255.255.255.255&quot;). 複数のドメインからMarketor経由で電子メールを送信する場合は、ITスタッフに各ドメインに対してこの行を（1行で）追加してもらう必要があります。

1. DKIMの場合、セットアップする各ドメインに対してDNSリソースレコードを作成します。 署名する各ドメインのホストレコードとTXT値を以下に示します。

   `[DKIMDomain1]`:「Host Record」 `[HostRecord1]` はで、「TXT Value」はで `[TXTValue1]`す。

   `[DKIMDomain2]`:「Host Record」 `[HostRecord2]` はで、「TXT Value」はで `[TXTValue2]`す。

   ここで説明する [手順に従って、設定した各DKIMDomainのHostRecordとTXTValueをコピーします](https://docs.marketo.com/display/public/DOCS/Set+up+a+Custom+DKIM+Signature)。 ITスタッフがこの手順を完了した後は、管理者/電子メール/DKIMで各ドメインを確認するのを忘れないでください。

## 手順4:ドメインのMXレコードの設定 {#step-set-up-mx-records-for-your-domain}

MXレコードを使用すると、返信や自動返信を処理するために、電子メールの送信元のドメインにメールを受信できます。 会社ドメインから送信する場合は、既にこの設定が行われている可能性があります。 そうでない場合は、通常、会社ドメインのMXレコードにマップするように設定できます。
