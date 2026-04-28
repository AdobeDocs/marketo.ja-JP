---
unique-page-id: 15695874
description: Connect your [!DNL BrightTALK] channel to Marketo via LaunchPoint using API-only user credentials.
title: ' [!DNL BrightTALK]  の Marketo への接続'
exl-id: 5c6a12ec-301b-4dec-975c-24ec759ebb37
feature: Administration, Integrations
source-git-commit: 40f06a5391f2f7263bea0c5b8cefc1f3a607c68c
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 63%

---

# [!DNL BrightTALK] の Marketo への接続 {#connect-brighttalk-to-marketo}

[!DNL BrightTALK] チャネルを Marketo インスタンスに接続する方法を説明します。 これを行うには、両方の管理者である必要があります。

>[!NOTE]
>
>**管理者権限が必要**

## [!DNL BrightTALK] での手順 {#steps-in-brighttalk}

1. [business.brighttalk.com/demandcentral](https://business.brighttalk.com/demandcentral/login){target="_blank"} にログインし、「**[!UICONTROL 今すぐ接続]**」をクリックします。

1. 「[!UICONTROL Marketo コネクタの詳細設定]」で、「**[!UICONTROL 接続]**」をクリックします。

1. The credentials screen appears, asking for: Client ID, Client Secret, Identity Service URL, and Rest Service URL. To get this information, log in to Marketo.

## Marketo での手順 {#steps-in-marketo}

>[!NOTE]
>
>At this point you are required to set up an [!DNL API Only User Role] and [!DNL API User] in order to restrict what permissions [!DNL BrightTALK] will have in your Marketo instance. Articles are available for those steps.

1. [API 専用ユーザーロール](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md){target="_blank"}を作成する。

1. 手順 4 で作成した [!DNL BrightTALK] API ロールを使用して、[API ユーザーを作成](/help/marketo/product-docs/administration/users-and-roles/create-api-only-user.md){target="_blank"}します。

1. **[!UICONTROL 管理]**&#x200B;領域に戻ります。

   ![](assets/connect-brighttalk-to-marketo-1.png)

1. 「**[!UICONTROL 統合]**」で、「**[!UICONTROL LaunchPoint]**」をクリックします。

   ![](assets/connect-brighttalk-to-marketo-2.png)

1. **[!UICONTROL 新規]**&#x200B;ドロップダウンをクリックして、**[!UICONTROL 新規サービス]**&#x200B;を選択します。

   ![](assets/connect-brighttalk-to-marketo-3.png)

1. 任意の&#x200B;**[!UICONTROL 表示名]**&#x200B;を入力します。 **[!UICONTROL サービス]**&#x200B;ドロップダウンをクリックし、**[!UICONTROL カスタム]**&#x200B;を選択します（[!DNL BrightTALK] は&#x200B;_選択しません_）。

   ![](assets/connect-brighttalk-to-marketo-4.png)

   >[!CAUTION]
   >
   >ドロップダウンの [!DNL BrightTALK] は選択しないでください。 This field is in the process of being removed, and selecting it could create significant issues with your [!DNL Marketo/BrightTALK] integration.

1. 任意の「[!UICONTROL 説明]」を入力します。 **[!UICONTROL API 専用ユーザー]**&#x200B;ドロップダウンをクリックし、手順 5 で作成した [!DNL BrightTALK API User] を選択します。 「**[!UICONTROL 作成]**」をクリックします。

   ![](assets/connect-brighttalk-to-marketo-5.png)

1. 先ほど作成したカスタムサービスの「**[!UICONTROL 詳細を表示]**」をクリックします。

   ![](assets/connect-brighttalk-to-marketo-6.png)

1. **[!UICONTROL クライアント ID]** および&#x200B;**[!UICONTROL クライアントシークレット]**&#x200B;をコピー（および保存）します。 「**[!UICONTROL 閉じる]**」をクリックします。

   ![](assets/connect-brighttalk-to-marketo-7.png)

1. 「**[!UICONTROL 統合]**」で、「**[!UICONTROL Web サービス]**」を選択します。

   ![](assets/connect-brighttalk-to-marketo-8.png)

1. **[!UICONTROL Rest API]** で、**[!UICONTROL エンドポイント]**&#x200B;および **[!UICONTROL ID]** をコピー（および保存）します。

   ![](assets/connect-brighttalk-to-marketo-9.png)

## [!DNL BrightTALK] での追加手順 {#additional-steps-in-brighttalk}

1. 手順 3 の [!DNL BrightTALK] コネクタの設定画面に戻り、手順 12 および 14 で保存した資格情報を入力します。

After the credentials are authenticated, you have officially connected [!DNL BrightTALK] to Marketo. The next step is to determine which data fields you want to sync. If you need assistance with that, contact [BrightTALK Support](https://www.brighttalk.com/){target="_blank"}.
