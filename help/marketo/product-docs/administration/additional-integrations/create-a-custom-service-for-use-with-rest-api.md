---
unique-page-id: 2360350
description: ReST API - Marketto Docs — 製品ドキュメントで使用するカスタムサービスの作成
title: ReST APIで使用するカスタムサービスの作成
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---


# ReST APIで使用するカスタムサービスの作成{#create-a-custom-service-for-use-with-rest-api}

ReST APIを介してMarketoと統合する場合は、カスタムサービスを作成する必要があります。 これが方法です。

>[!PREREQUISITES]
>
>* [APIのみのユーザーロールの作成](../../../product-docs/administration/users-and-roles/create-an-api-only-user-role.md)
>* [APIのみのユーザーの作成](../../../product-docs/administration/users-and-roles/create-an-api-only-user.md)

>



>[!NOTE]
>
>**必要な管理者権限**

>[!NOTE]
>
>**ディープダイブ**
>
>[ReST API](http://developers.marketo.com/documentation/rest/)の詳細については、開発者向けのドキュメントを参照してください。 また、必要に応じて、[SOAP API](http://developers.marketo.com/documentation/soap/)も用意しています。

>[!NOTE]
>
>MarketoのSparkレベルを持っている場合は、カスタムサービスを作成できません。

## カスタムサービスの作成{#create-custom-service}

1. **管理者**&#x200B;に移動し、**LaunchPoint**&#x200B;をクリックします。

   ![](assets/image2014-9-19-10-3a38-3a15.png)

1. 「**新しい**」で、「**新しいサービス**」をクリックします。

   ![](assets/image2014-9-19-10-3a38-3a22.png)

1. サービスの&#x200B;**表示名**&#x200B;を入力します。 **APIのみユーザー** [以前に作成した](../../../product-docs/administration/users-and-roles/create-an-api-only-user.md)を選択します。

   >[!NOTE]
   >
   >**Reminder**
   >
   >一般的なウェビナーサービスには、既にネイティブ統合が用意されています。

   ![](assets/image2014-9-19-10-3a38-3a32.png)

1. 「**作成**」をクリックします。

   ![](assets/image2014-9-19-10-3a39-3a28.png)

   ああ！ サービスが作成されました。次に、アクセスを提供するためのすべての資格情報を取得します。

## APIアクセスの資格情報{#credentials-for-api-access}

1. **管理者**&#x200B;に移動し、**LaunchPoint**&#x200B;をクリックします。

   ![](assets/image2014-9-19-10-3a42-3a11.png)

1. 上記で作成したカスタムLaunchPointサービスの&#x200B;**表示の詳細**&#x200B;をクリックします。

   ![](assets/image2014-9-19-10-3a42-3a16.png)

1. 「**トークンを取得**」をクリックします。

   ![](assets/image2014-9-19-10-3a42-3a24.png)

1. 接続の確立の担当者に、**クライアントID**、**クライアントシークレット**、**許可されたユーザー**、**トークン**&#x200B;を提供します。

   ![](assets/image2014-9-19-10-3a42-3a38.png)

>[!CAUTION]
>
>この情報は共有しないでください。データのバックドアです。 安全に！

