---
unique-page-id: 4720710
description: 電子メール配信品質のSPFおよびDKIMの設定 — Marketto Docs — 製品ドキュメント
title: 電子メールの配信品質に対するSPFおよびDKIMの設定
translation-type: tm+mt
source-git-commit: 07ae1b3f3ee3e9d7f35373eea039d336bd786f97
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 0%

---


# 電子メールの配信品質に対するSPFおよびDKIMの設定 {#set-up-spf-and-dkim-for-your-email-deliverability}

電子メールの配信率を向上させる1つの簡単な方法は、 **SPF** (Sender Policy Framework)と **DKIM** (Domain Keys Identified Mail)をDNS設定に組み込むことです。 DNSエントリに加えて、Marketingが自分の代わりに電子メールを送信することを承認したことを受信者に伝えています。 この変更を行わないと、電子メールはドメインから送信された電子メールですが、MarketoドメインのIPアドレスから送信された電子メールであるため、スパムとしてマークされる可能性が高くなります。

>[!CAUTION]
>
>この変更をDNSレコードに行うには、ネットワーク管理者が必要です。

## SPFの設定 {#set-up-spf}

**ドメインにSPFレコードがない場合**

ネットワーク管理者に問い合わせて、DNSエントリに次の行を追加してください。 「 [domain] 」をWebサイトのメインドメイン( 「会社.com」)と [corpIP] (会社の電子メールサーバーのIPアドレスを含む &quot;255.255.255.255&quot;). Marketorを通じて複数のドメインからの電子メールを送信する場合は、この電子メールを各ドメインに（1行で）追加する必要があります。
[domain] IN TXT v=spf1 mx ip4:[corpIP] include:mktomail.com ～all\
ドメインにSPFレコードがある場合

DNSエントリに既にSPFレコードがある場合は、次を追加します。

include:mktomail.com

## DKIMの設定 {#set-up-dkim}

### DKIMとは？ DKIMを設定する理由 {#what-is-dkim-why-do-i-want-to-set-up-dkim}

DKIMは、電子メールの受信者が、電子メールの送信者によって電子メールメッセージが送信されたかどうかを判断するために使用する認証プロトコルです。 DKIMは、受信者がメッセージが偽造でないと確信できるので、受信トレイへの電子メールの配信品質を向上させることがよくあります。

DKIMの仕組みは？

DNSレコードに公開鍵を設定し、管理者セクション(A)で送信ドメインをアクティブにした後、送信メッセージに対するカスタムDKIM署名を有効にします。この設定には、送信する各電子メールと共に暗号化された電子署名が含まれます(B)。 受信側は、送信側ドメインのDNS(C)の「公開鍵」を調べることで、デジタル署名を復号化できます。 電子メール内のキーがDNSレコード内のキーに対応している場合、受信側のメールサーバーは、送信元の電子メールマーケティング担当者に代わって送信された電子メールを受け入れる可能性が高くなります。

![](assets/image2015-1-12-13-3a56-3a55.png)

DKIMの設定方法

詳しくは、「カスタムDKIM署名の [設定](set-up-a-custom-dkim-signature.md)」を参照してください。

>[!NOTE]
>
>**関連記事**
>
>* [SPFの詳細と仕組み](http://www.open-spf.org/Introduction/)
>* [マーケティング担当者向け電子メール配信品質ツール](https://www.marketo.com/software/email-marketing/email-deliverability/)
>* [SPFが正しく設定されているか](http://www.kitterman.com/spf/validate.html)
>* [正しい構文を使用したか。](http://www.open-spf.org/SPF_Record_Syntax/)

>



