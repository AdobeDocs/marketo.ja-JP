---
description: 電子メール接続のスロットリング — Marketto Docs — 製品ドキュメント
title: 電子メール接続のスロットリング
translation-type: tm+mt
source-git-commit: f3e3efc1cc480e9c6501b7e808f53c3a8bdc93d8
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 0%

---


# 電子メール接続のスロットリング{#email-connection-throttling}

Sales Connectアカウントを統合してExchangeまたはGmailの電子メールプロバイダー経由で送信するオファーは、合理化されたセットアップを行い、1:1の販売コミュニケーションのための電子メール配信品質を最適化します。 ただし、システムの健全性とアカウントの安全性を維持するために、GmailとExchangeでは電子メールの送信制限が適用されます。 これらの制限は、プロバイダの判断で増減できます。

## 電子メール接続の制限（ベータ） {#email-connection-throttling-beta}

>[!AVAILABILITY]
>
>この機能は、現在ベータ版リリース中です。 このベータ版に参加するには、カスタマーサクセスマネージャーにお問い合わせください。

電子メール接続のスロットリングを使用すると、Sales Connect管理者は、GmailまたはExchangeを配信チャネルとして使用する場合に、電子メールが配信チャネルプロバイダーに引き渡される速度が強制的な制限を超えないように、電子メールの送信率を設定できます。

制限を常に超える場合は、配信チャネルプロバイダーからの不審な動作と見なされ、電子メールの失敗やアカウントの無効化が発生する場合があります。

**メモ/ハイライト**

* ユーザーがGmailまたはExchangeに接続すると自動的に有効になる
* ニーズに合わせてレコメンデーションの設定を増減する場合は、カスタマイズできます。
* GmailまたはExchange経由で送信される電子メールの制限のみが行われ、カスタム配信チャネルの制限は行われません。
* 電子メール接続のスロットリングは、各ユーザーが自分の電子メールプロバイダーと独自の接続を持つので、各ユーザーの電子メールを個別にキューに入れます

**電子メール接続のスロットリング設定の指定**

1. 歯車アイコンをクリックし、**設定**&#x200B;を選択します。

   ![](assets/email-connection-throttling-1.png)

1. [**一般**]をクリックします。

   ![](assets/email-connection-throttling-2.png)

1. 「電子メールチャネルのスロットリング」カードで、電子メール接続プロバイダーに送信する電子メールのバッチサイズを入力します。

   ![](assets/email-connection-throttling-3.png)

1. 各バッチが送信されるまでの待機時間を設定します。 この例では、45秒ごとに25件の電子メールを選択しています。

   ![](assets/email-connection-throttling-4.png)

1. 「**保存**」をクリックします。

   ![](assets/email-connection-throttling-5.png)

変更を保存すると、すべてのユーザーは、接続されているGmailまたはExchangeアカウントに、配信用に電子メールをバッチで送信できます。

## 電子メールプロバイダーの制限{#email-provider-limits}

**Outlook 365**

Business/Enterprise

* 1日に10,000
* 30/分
* 電子メールあたり500受信者

[詳細は](https://docs.microsoft.com/en-us/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#RecipientLimits)を参照してください。

**Gmail**

* 1日あたり2,000件（体験版およびフラグ付きのアカウントの場合は500件）
* 1秒あたり2件の電子メール（APIの制限）
* メッセージあたり2,000受信者(外部受信者の場合は最大500)

[詳細は](https://support.google.com/a/answer/166852?hl=en)を参照してください。

**Microsoft Exchange Server (2010、2013)**

制限は、組織のIT部門が設定します。これは、サーバが組織でホストされているためです。 詳細については、ネットワーク管理者またはシステム管理者に問い合わせてください。

>[!MORELIKETHIS]
>
>* [配信チャネルの概要](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/delivery-channel-overview.md)
>* [Gmailユーザーの電子メール接続](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [Outlookユーザー用電子メール接続](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)

