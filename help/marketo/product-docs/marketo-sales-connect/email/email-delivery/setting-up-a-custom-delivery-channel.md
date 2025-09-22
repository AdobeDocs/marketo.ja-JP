---
unique-page-id: 14746470
description: カスタム配信チャネルの設定 - Marketo ドキュメント - 製品ドキュメント
title: カスタム配信チャネルの設定
exl-id: a31f7bfd-a4ee-4948-9bdc-b49d47054d40
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 100%

---

# カスタム配信チャネルの設定 {#setting-up-a-custom-delivery-channel}

[!DNL Marketo Sales Connect] を使用すると、カスタム SMTP サーバーを統合してメールを配信できます。これは、Gmail や [!DNL Exchange] の配信チャネルから一括メールを送信しない場合に最適です。

ユーザは、個々の使用に合わせてカスタム SMTP サーバーを設定できます。また、管理者は、インスタンス内のすべての [!DNL Sales Connect] ユーザで共有されるチーム SMTP を設定できます。

>[!NOTE]
>
>* SMTP サーバーの設定に加えて、メールを送信する前に、[メール ID を認証する必要があります](/help/marketo/product-docs/marketo-sales-connect/getting-started/email-settings/verify-your-email.md)。
>* お使いの SMTP サーバーに適したサーバー資格情報を取得するには、IT チームまたは SMTP サーバーのベンダーと協力することをお勧めします。
>* SMTP サーバーの資格情報を使用して Gmail サーバーや [!DNL Exchange] サーバーに接続できません。これらのプロバイダーとの統合には、アドビのメール接続サービスをご利用ください。

## カスタム SMTP {#custom-smtp}

1. [web アプリケーション](https://toutapp.com/login)にログインし、右上の歯車アイコンをクリックして、「**[!UICONTROL 設定]**」を選択します。

   ![](assets/setting-up-a-custom-delivery-channel-1.png)

1. 「[!UICONTROL マイアカウント]」で、「**[!UICONTROL メール設定]**」をクリックします。

   ![](assets/setting-up-a-custom-delivery-channel-2.png)

1. 「**[!UICONTROL カスタム配信チャネル]**」をクリックします。

   ![](assets/setting-up-a-custom-delivery-channel-3.png)

1. [!UICONTROL SMTP サーバー]の資格情報を入力し、「**[!UICONTROL 接続]**」をクリックします。

   ![](assets/setting-up-a-custom-delivery-channel-4.png)

   >[!NOTE]
   >
   >これが唯一の配信チャネルの場合、すべてのメール ID に自動的に割り当てられるため、ここで完了です。これが唯一の配信チャネルでない場合は、手順 5 に進んでください。

1. 「[!UICONTROL メール設定]」で、「**[!UICONTROL アドレスと署名]**」をクリックします。

   ![](assets/setting-up-a-custom-delivery-channel-5.png)

1. 配信チャネルを選択するメール ID を見つけ、「**[!UICONTROL 配信チャネルを選択]**」を選択します。

   ![](assets/setting-up-a-custom-delivery-channel-6.png)

1. [!UICONTROL 配信品質]カードで、「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/setting-up-a-custom-delivery-channel-7.png)

1. [!UICONTROL チャネル]ドロップダウンをクリックし、先ほど追加したカスタム配信チャネルを選択します。「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/setting-up-a-custom-delivery-channel-8.png)

   >[!NOTE]
   >
   >チーム管理者がチーム SMTP サーバーを設定すると、これはデフォルトのメール ID にのみ自動的に適用され、他のメール ID のオプションとして使用できます。

## チーム SMTP サーバー {#team-smtp-server}

>[!NOTE]
>
>**管理者権限が必要**

1. [web アプリケーション](https://toutapp.com/login)にログインし、右上の歯車アイコンをクリックして、「**[!UICONTROL 設定]**」を選択します。

   ![](assets/setting-up-a-custom-delivery-channel-9.png)

1. 「[!UICONTROL 管理設定]」で、「**[!UICONTROL 一般]**」をクリックします。

   ![](assets/setting-up-a-custom-delivery-channel-10.png)

1. 「**[!UICONTROL チーム配信チャネル]**」をクリックします。

   ![](assets/setting-up-a-custom-delivery-channel-11.png)

1. [!UICONTROL SMTP サーバー]の資格情報を入力し、「**[!UICONTROL 接続]**」をクリックします。

   ![](assets/setting-up-a-custom-delivery-channel-12.png)

   >[!NOTE]
   >
   >チーム SMTP サーバーは、すべてのチームメンバーに対するデフォルトのメール ID のデフォルトの配信チャネルになります。さらに、その他のすべてのメール ID の配信チャネルオプションとして使用できます。

   >[!MORELIKETHIS]
   >
   >* [Gmail ユーザのメール接続](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
   >
   >* [ [!DNL Outlook]  ユーザのメール接続](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
