---
unique-page-id: 4720710
description: E メール配信品質の SPF および DKIM の設定 — Marketo Docs — 製品ドキュメント
title: メール到達率のための SPF と DKIM の設定
exl-id: a0f88e94-3348-4f48-bbd2-963e2af93dc0
source-git-commit: de32becbfe74c2a88c53de8af8be4ee022782114
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 5%

---

# メール到達率のための SPF と DKIM の設定 {#set-up-spf-and-dkim-for-your-email-deliverability}

E メール配信率を向上させるための簡単な方法の 1 つは、 **SPF** （送信者ポリシーの枠組み）および **DKIM** （ドメインキー識別メール）を DNS 設定に追加します。 DNS エントリに加えて、Marketoが代理で E メールを送信する権限を受信者に付与することになります。 この変更がないと、E メールはドメインから送信されたが、Marketoドメインの IP アドレスから送信されたので、E メールがスパムとしてマークされる可能性が高くなります。

>[!CAUTION]
>
>この変更を DNS レコードに加えるには、ネットワーク管理者が必要です。

## SPF の設定 {#set-up-spf}

**ドメインに SPF レコードがない場合**

DNS エントリに次の行を追加するよう、ネットワーク管理者に依頼します。 置換 [ドメイン] を Web サイトのメインドメイン ( 例： &quot;company.com&quot;) および [corpIP] 会社の電子メールサーバーの IP アドレス ( 例： 255.255.255.255）で置き換えます。Marketoを通じて複数のドメインから E メールを送信する場合は、これを各ドメインに（1 行で）追加する必要があります。

`[domain] IN TXT v=spf1 mx ip4:[corpIP] include:mktomail.com ~all`

**ドメインに SPF レコードがある場合**

DNS エントリに既に SPF レコードがある場合は、次の内容を追加します。

include: mktomail.com

## DKIM の設定 {#set-up-dkim}

**DKIM とは DKIM を設定する理由**

DKIM は、E メールの受信者が、E メールの送信者によって E メールメッセージが送信されたかどうかを判断するために使用される認証プロトコルです。 DKIM は、多くの場合、受信者はメッセージが偽造ではないと確信できるので、受信ボックスへの E メールの配信品質を向上させます。

**DKIM の仕組み**

DNS レコードに公開鍵を設定し、Admin セクション (A) で送信ドメインを有効にした後、送信メッセージのカスタム DKIM 署名を有効にします。この署名には、送信メールごとに暗号化されたデジタル署名が含まれます (B)。 受信者は、送信ドメインの DNS(C) の「公開鍵」を検索することで、デジタル署名を復号化できます。 電子メールのキーが DNS レコードのキーに対応している場合、受信側の電子メールサーバーは、お客様に代わって送信された電子メールMarketoを受け入れる可能性が高くなります。

![](assets/image2015-1-12-13-3a56-3a55.png)

**DKIM の設定方法を教えてください。**

詳しくは、 [カスタム DKIM 署名の設定](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md).

>[!MORELIKETHIS]
>
>* [SPF の詳細と仕組み](http://www.open-spf.org/Introduction/)
>* [Marketo E メール配信ツール](https://www.marketo.com/software/email-marketing/email-deliverability/)
>* [SPF が正しく設定されているか](https://www.kitterman.com/spf/validate.html)
>* [正しい構文を使用したか。](http://www.open-spf.org/SPF_Record_Syntax/)

