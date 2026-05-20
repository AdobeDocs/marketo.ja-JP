---
unique-page-id: 2360350
description: ReST API統合用にAPIのみのユーザーにリンクされたカスタム LaunchPoint サービスを作成します。
title: ReST API で使用するカスタムサービスの作成
exl-id: d94f723b-2e98-4350-a9e5-bd57aff2303b
feature: Administration
TQID: https://experienceleague.adobe.com/7RYZTS-1WiaU0A8ThqHvk01S7GLIIP65xyKI3SIuPyo
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b13bd2ad-8e65-49e5-9691-2a0d31067b35id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 175
ht-degree: 63%

---

# ReST API で使用するカスタムサービスの作成 {#create-a-custom-service-for-use-with-rest-api}

ReST APIを介してMarketoと統合する場合は、カスタムサービスを作成します。

>[!PREREQUISITES]
>
>* [API 専用ユーザーのロールの作成](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md)
>* [API 専用ユーザーの作成](/help/marketo/product-docs/administration/users-and-roles/create-api-only-user.md)
>

>[!NOTE]
>
>**管理者権限が必要**

>[!TIP]
>
>[REST API](https://developer.adobe.com/marketo-apis/)について詳しくは、開発者ドキュメントを参照してください。

## カスタムサービスの作成 {#create-custom-service}

1. 「**[!UICONTROL 管理者]**」領域に移動します。

   ![](assets/create-a-custom-service-for-use-with-rest-api-1.png)

1. **[!UICONTROL LaunchPoint]**.をクリックします。

   ![](assets/create-a-custom-service-for-use-with-rest-api-2.png)

1. 「**[!UICONTROL 新規]**」を選択し、次に「**[!UICONTROL 新規サービス]**」を選択します。

   ![](assets/create-a-custom-service-for-use-with-rest-api-3.png)

1. サービスの「**[!UICONTROL 表示名]**」を入力します。 **[!UICONTROL 先ほど作成した]**「[API 専用ユーザー](/help/marketo/product-docs/administration/users-and-roles/create-api-only-user.md)」を選択します。

   ![](assets/create-a-custom-service-for-use-with-rest-api-4.png)

1. 「**[!UICONTROL 作成]**」をクリックします。

   ![](assets/create-a-custom-service-for-use-with-rest-api-5.png)

   これでサービスが作成されました。 アクセス用に提供する資格情報を取得します。

## API アクセスの資格情報 {#credentials-for-api-access}

1. 「**[!UICONTROL 管理者]**」領域に移動します。

   ![](assets/create-a-custom-service-for-use-with-rest-api-6.png)

1. **[!UICONTROL LaunchPoint]**.をクリックします。

   ![](assets/create-a-custom-service-for-use-with-rest-api-7.png)

1. 上記で作成したカスタム [!UICONTROL LaunchPoint] サービスの「**[!UICONTROL 詳細を表示]**」をクリックします。

   ![](assets/create-a-custom-service-for-use-with-rest-api-8.png)

1. 「**[!UICONTROL トークンを取得]**」をクリックします。

   ![](assets/create-a-custom-service-for-use-with-rest-api-9.png)

1. 接続を確立する担当者に、**[!UICONTROL クライアント ID]**、**[!UICONTROL クライアントシークレット]**、**[!UICONTROL 許可されたユーザー]**、**[!UICONTROL トークン]**&#x200B;を提供します。

   ![](assets/create-a-custom-service-for-use-with-rest-api-10.png)

>[!CAUTION]
>
>この情報はデータへのアクセスを提供するので、共有しないでください。
