---
unique-page-id: 4720710
description: Eメール配信品質のSPFとDKIMの設定 — Marketoドキュメント — 製品ドキュメント
title: Eメール配信品質のSPFとDKIMの設定
exl-id: a0f88e94-3348-4f48-bbd2-963e2af93dc0
source-git-commit: 46812deb41ed56328a4a64fbd36340d13c50dde4
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---

# Eメール配信品質のSPFとDKIMの設定 {#set-up-spf-and-dkim-for-your-email-deliverability}

Eメール配信率を簡単に改善する方法の1つは、**SPF**(Sender Policy Framework)と&#x200B;**DKIM**(Domain Keys Identified Mail)をDNS設定に組み込むことです。 DNSエントリにこの追加が加えられると、Marketoが代理でEメールを送信する権限を受信者に伝えることになります。 この変更をおこなわないと、Eメールはドメインから送信され、MarketoドメインのIPアドレスから送信されるので、Eメールがスパムとしてマークされる可能性が高くなります。

>[!CAUTION]
>
>この変更をDNSレコードに加えるには、ネットワーク管理者が必要です。

## SPFの設定 {#set-up-spf}

**ドメインにSPFレコードがない場合**

ネットワーク管理者に次の行をDNSエントリに追加するよう依頼します。 [domain]をWebサイトのメインドメイン(例： 「company.com」)および[corpIP]（会社の電子メールサーバーのIPアドレスを使用） &quot;255.255.255.255&quot;)と表示されます。 Marketoを通じて複数のドメインからEメールを送信する場合は、これを各ドメインに（1行で）追加する必要があります。

`[domain] IN TXT v=spf1 mx ip4:[corpIP] include:mktomail.com ~all`

**ドメインにSPFレコードがある場合**

DNSエントリに既にSPFレコードがある場合は、次の内容を追加します。

include:mktomail.com

## DKIMの設定 {#set-up-dkim}

**dkimとはなぜDKIMを設定したいのですか？**

DKIMは、Eメールの受信者が、Eメールの送信者によってEメールメッセージが送信されたかどうかを判断するために使用する認証プロトコルです。 DKIMは、受信者がメッセージが偽物ではないと確信できるので、多くの場合、受信ボックスへのEメールの配信品質を向上させます。

**DKIMの仕組み**

DNSレコードに公開鍵を設定し、Adminセクション(A)で送信ドメインを有効にした後、送信メッセージのカスタムDKIM署名を有効にします。この署名には、送信されるEメールごとに暗号化されたデジタル署名が含まれます(B)。 受信者は、送信ドメインのDNS(C)の「公開鍵」を調べることで、デジタル署名を復号化できます。 EメールのキーがDNSレコードのキーに対応する場合、受信側のメールサーバーは、代理で送信されたEメールMarketoを受け入れる可能性が高くなります。

![](assets/image2015-1-12-13-3a56-3a55.png)

**DKIMの設定方法を教えてください。**

[カスタムDKIM署名の設定](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md)を参照してください。

>[!MORELIKETHIS]
>
>* [SPFとその仕組みの詳細](http://www.open-spf.org/Introduction/)
>* [Marketo Eメール配信品質ツール](https://www.marketo.com/software/email-marketing/email-deliverability/)
>* [SPFが正しく設定されているか](https://www.kitterman.com/spf/validate.html)
>* [正しい構文を使用したか。](https://www.open-spf.org/SPF_Record_Syntax/)

