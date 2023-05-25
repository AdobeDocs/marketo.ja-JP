---
unique-page-id: 15695874
description: '"接続 [!DNL BrightTALK] Marketo - Marketoドキュメント — 製品ドキュメント»'
title: '"接続 [!DNL BrightTALK] Marketoへ」'
exl-id: 5c6a12ec-301b-4dec-975c-24ec759ebb37
source-git-commit: 1f10e1fcdbd5cf91481f749236fd37050ade29f8
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 37%

---

# 接続 [!DNL BrightTALK] Marketo {#connect-brighttalk-to-marketo}

接続方法 [!DNL BrightTALK] Marketoインスタンスにチャネルで接続できます。 これを行うには、両方の管理者である必要があります。

>[!NOTE]
>
>**管理者権限が必要**

## 手順： [!DNL BrightTALK] {#steps-in-brighttalk}

1. にログインします。 [business.brighttalk.com/demandcentral](https://business.brighttalk.com/demandcentral/login){target="_blank"} をクリックし、 **[!UICONTROL 今すぐ接続]**.
1. の下 [!UICONTROL 高度なMarketoコネクタ]をクリックし、 **[!UICONTROL 接続]**.
1. 資格情報画面が表示され、次の情報が求められます。クライアント ID、クライアントシークレット、ID サービス URL、REST サービス URL。この情報を取得するには、Marketo にログインします。

## Marketo での手順 {#steps-in-marketo}

>[!NOTE]
>
>この時点で、 [!DNL API Only User Role] および [!DNL API User] どの権限を制限するために [!DNL BrightTALK] は、Marketoインスタンスに含まれます。 これらの手順に関する記事が既にあり、以下が記事のリンクです。

1. [API のみのユーザー役割を作成する](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md){target="_blank"}。

1. 手順 4 で作成した API の役割を使用して、[API ユーザーを作成](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md){target="_blank"}[!DNL BrightTALK]します。

1. に戻ります。 **[!UICONTROL 管理者]** 領域

   ![](assets/connect-brighttalk-to-marketo-1.png)

1. の下 **[!UICONTROL 統合]**&#x200B;をクリックし、 **[!UICONTROL LaunchPoint]**.

   ![](assets/connect-brighttalk-to-marketo-2.png)

1. 「**[!UICONTROL 新規]**」ドロップダウンをクリックして、「**[!UICONTROL 新規サービス]**」を選択します。

   ![](assets/connect-brighttalk-to-marketo-3.png)

1. を入力します。 **[!UICONTROL 表示名]** 選択した内容です。 次をクリック： **[!UICONTROL サービス]** ドロップダウンして「 」を選択します。 **[!UICONTROL カスタム]** ( _not_ 選択 [!DNL BrightTALK]) をクリックします。

   ![](assets/connect-brighttalk-to-marketo-4.png)

   >[!CAUTION]
   >
   >必ず選択しないでください [!DNL BrightTALK] 」と入力します。 このフィールドは、削除中で、選択すると、 [!DNL Marketo/BrightTALK] 統合とも呼ばれます。

1. を入力します。 [!UICONTROL 説明] 選択した内容です。 次をクリック： **[!UICONTROL API 専用ユーザー]** ドロップダウンで、 [!DNL BrightTALK API User] 手順 5 で作成した内容。 「**[!UICONTROL 作成]**」をクリックします。

   ![](assets/connect-brighttalk-to-marketo-5.png)

1. 先ほど作成したカスタムサービスの「**[!UICONTROL 詳細を表示]**」をクリックします。

   ![](assets/connect-brighttalk-to-marketo-6.png)

1. **[!UICONTROL クライアント ID]** および&#x200B;**[!UICONTROL クライアントシークレット]**&#x200B;をコピー（および保存）します。「**[!UICONTROL 閉じる]**」をクリックします。

   ![](assets/connect-brighttalk-to-marketo-7.png)

1. の下 **[!UICONTROL 統合]**&#x200B;を選択します。 **[!UICONTROL Web サービス]**.

   ![](assets/connect-brighttalk-to-marketo-8.png)

1. の下 **[!UICONTROL Rest API]**、コピー（および保存） **[!UICONTROL エンドポイント]** および **[!UICONTROL ID]**.

   ![](assets/connect-brighttalk-to-marketo-9.png)

## その他の手順： [!DNL BrightTALK] {#additional-steps-in-brighttalk}

1. に戻る [!DNL BrightTALK] 手順 3 のコネクタ設定画面を開き、手順 12 および 14 で保存した資格情報を入力します。

資格情報が認証されると、正式に接続されます [!DNL BrightTALK] Marketo 次のステップは、 [同期するデータフィールド](https://support.brighttalk.com/hc/en-us/articles/115005131274-BrightTALK-Connector-for-Marketo-Choose-the-Fields-to-Sync){target="_blank"}.
