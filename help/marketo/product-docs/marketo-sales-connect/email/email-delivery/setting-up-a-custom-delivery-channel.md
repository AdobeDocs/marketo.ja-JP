---
unique-page-id: 14746470
description: カスタム配信チャネルの設定 — Marketto Docs — 製品ドキュメント
title: カスタム配信チャネルの設定
translation-type: tm+mt
source-git-commit: f3e3efc1cc480e9c6501b7e808f53c3a8bdc93d8
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 0%

---


# カスタム配信チャネルの設定{#setting-up-a-custom-delivery-channel}

Marketo Sales Connectを使用すると、カスタムSMTPサーバーと統合して電子メールの配信を行うことができます。 これは、GmailやExchange配信チャネルから大量のメールを送信したくない場合に便利です。

ユーザーは、独自の個人用にカスタムSMTPサーバーを設定できます。また、管理者は、インスタンス内のすべてのSales Connectユーザーで共有するチームSMTPを設定できます。

>[!NOTE]
>
>* SMTPサーバーを設定するだけでなく、電子メールを送信する前に、[電子メールIDを確認](/help/marketo/product-docs/marketo-sales-connect/getting-started/email-settings/verify-your-email.md)する必要があります。
>* ITチームまたはSMTPサーバーのベンダーと協力して、SMTPサーバーに適したサーバー資格情報を取得することをお勧めします。
>* SMTPサーバーの資格情報を使用してGmailとExchangeサーバーに接続することはできません。 アドビの電子メール接続サービスを使用して、これらのプロバイダーと統合してください。


## カスタムSMTP {#custom-smtp}

1. [Webアプリケーション](https://toutapp.com/login)にログインし、右上の歯車アイコンをクリックして、「**設定**」を選択します。

   ![](assets/setting-up-a-custom-delivery-channel-1.png)

1. 「マイアカウント」で、「**電子メール設定**」をクリックします。

   ![](assets/setting-up-a-custom-delivery-channel-2.png)

1. 「**カスタム配信チャネル**」をクリックします。

   ![](assets/setting-up-a-custom-delivery-channel-3.png)

1. SMTP Serverの資格情報を入力し、「**接続**」をクリックします。

   ![](assets/setting-up-a-custom-delivery-channel-4.png)

   >[!NOTE]
   >
   >これが唯一の配信チャネルの場合は、すべての電子メールIDに自動的に割り当てられ、ここで処理が完了します。 これが配信チャネル以外の場合は、手順5に進んでください。

1. 「電子メールの設定」に進んだまま、「**アドレスと署名**」をクリックします。

   ![](assets/setting-up-a-custom-delivery-channel-5.png)

1. 配信チャネルを選択する電子メールIDを探し、**配信チャネルを選択**&#x200B;をクリックします。

   ![](assets/setting-up-a-custom-delivery-channel-6.png)

1. 配信品質カードで、「**編集**」をクリックします。

   ![](assets/setting-up-a-custom-delivery-channel-7.png)

1. 「チャネル」ドロップダウンをクリックし、先ほど追加したカスタム配信チャネルを選択します。 「**保存**」をクリックします。

   ![](assets/setting-up-a-custom-delivery-channel-8.png)

   >[!NOTE]
   >
   >チーム管理者がチームSMTPサーバーを設定すると、そのサーバーは自動的にデフォルトの電子メールIDにのみ適用され、他の電子メールIDのオプションとして使用できます。

## チームSMTPサーバー{#team-smtp-server}

>[!NOTE]
>
>**必要な管理者権限**

1. [Webアプリケーション](https://toutapp.com/login)にログインし、右上の歯車アイコンをクリックして、「**設定**」を選択します。

   ![](assets/setting-up-a-custom-delivery-channel-9.png)

1. 「管理設定」で、「**一般**」をクリックします。

   ![](assets/setting-up-a-custom-delivery-channel-10.png)

1. 「**チーム配信チャネル**」をクリックします。

   ![](assets/setting-up-a-custom-delivery-channel-11.png)

1. SMTP Serverの資格情報を入力し、「**接続**」をクリックします。

   ![](assets/setting-up-a-custom-delivery-channel-12.png)

   >[!NOTE]
   >
   >チームSMTPサーバーは、すべてのチームメンバーの既定の電子メールIDの既定の配信チャネルです。 さらに、他のすべての電子メールIDの配信チャネルオプションとしても使用できます。

   >[!MORELIKETHIS]
   >
   >* [Gmailユーザーの電子メール接続](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
      >
      >
   * [Outlookユーザー用電子メール接続](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)

