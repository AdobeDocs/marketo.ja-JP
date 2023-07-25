---
unique-page-id: 2360350
description: ReST API で使用するカスタムサービスの作成 - Marketo ドキュメント - 製品ドキュメント
title: ReST API で使用するカスタムサービスの作成
exl-id: d94f723b-2e98-4350-a9e5-bd57aff2303b
feature: Administration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 100%

---

# ReST API で使用するカスタムサービスの作成 {#create-a-custom-service-for-use-with-rest-api}

Marketo との統合に ReST API を使用する場合、カスタムサービスの作成をお勧めします。手順は以下のとおりです。

>[!PREREQUISITES]
>
>* [API 専用ユーザのロールの作成](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md)
>* [API 専用ユーザの作成](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md)
>

>[!NOTE]
>
>**管理者権限が必要**

>[!TIP]
>
>[ReST API](https://developers.marketo.com/documentation/rest/) の詳細については、開発者向けドキュメントを参照してください。必要に応じて、[SOAP API](https://developers.marketo.com/documentation/soap/) も用意しています。

## カスタムサービスの作成 {#create-custom-service}

1. 「**[!UICONTROL 管理者]**」領域に移動します。

   ![](assets/create-a-custom-service-for-use-with-rest-api-1.png)

1. **LaunchPoint**.をクリックします。

   ![](assets/create-a-custom-service-for-use-with-rest-api-2.png)

1. 「**[!UICONTROL 新規]**」を選択し、次に「**[!UICONTROL 新規サービス]**」を選択します。

   ![](assets/create-a-custom-service-for-use-with-rest-api-3.png)

1. サービスの「**[!UICONTROL 表示名]**」を入力します。**[!UICONTROL 先ほど作成した]**「[API のみのユーザ](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md)」を選択します。

   ![](assets/create-a-custom-service-for-use-with-rest-api-4.png)

   >[!NOTE]
   >
   >一般的なウェビナーサービスに対しては、既にネイティブ統合が行われています。

1. 「**[!UICONTROL 作成]**」をクリックします。

   ![](assets/create-a-custom-service-for-use-with-rest-api-5.png)

   これでサービスが作成されました。次に、アクセス用の認証情報をすべて取得します。

## API アクセスの認証情報 {#credentials-for-api-access}

1. 「**[!UICONTROL 管理者]**」領域に移動します。

   ![](assets/create-a-custom-service-for-use-with-rest-api-6.png)

1. **[!UICONTROL LaunchPoint]**.をクリックします。

   ![](assets/create-a-custom-service-for-use-with-rest-api-7.png)

1. 上記で作成したカスタム LaunchPoint サービスの「**[!UICONTROL 詳細を表示]**」をクリックします。

   ![](assets/create-a-custom-service-for-use-with-rest-api-8.png)

1. 「**[!UICONTROL トークンを取得]**」をクリックします。

   ![](assets/create-a-custom-service-for-use-with-rest-api-9.png)

1. 接続を確立する担当者に、**[!UICONTROL クライアント ID]**、**[!UICONTROL クライアントシークレット]**、**[!UICONTROL 許可されたユーザ]**、**[!UICONTROL トークン]**&#x200B;を提供します。

   ![](assets/create-a-custom-service-for-use-with-rest-api-10.png)

>[!CAUTION]
>
>これらの情報は共有しないでください。データの裏の侵入経路になります。安全な取り扱いを心がけてください。
