---
unique-page-id: 2360207
description: API 専用ユーザーの作成 - Marketo ドキュメント - 製品ドキュメント
title: API 専用ユーザーの作成
exl-id: 23c92255-07a8-41c2-b7b8-8e495d135671
feature: Users and Roles
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 100%

---

# API 専用ユーザーの作成 {#create-an-api-only-user}

[REST API](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/rest-api){target="_blank"} を使用して Marketo と統合する場合は、API 専用ユーザーを作成する必要があります。手順は次のとおりです。

>[!IMPORTANT]
>
>Adobe ID にオンボードされたサブスクリプションで API のみのユーザを作成している場合は、手順が異なります。[こちらを参照してください](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-api-only-user-for-adobe-ims-enabled-subscriptions.md){target="_blank"}。

>[!PREREQUISITES]
>
>[API 専用ユーザーのロールの作成](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md){target="_blank"}

>[!NOTE]
>
>**管理者権限が必要**

1. 「**[!UICONTROL 管理者]**」領域に移動します。

   ![](assets/create-an-api-only-user-1.png)

1. 「**[!UICONTROL ユーザー＆ロール]**」をクリックします。

   ![](assets/create-an-api-only-user-2.png)

1. 「**[!UICONTROL 新しいユーザーを招待]**」をクリックします。

   ![](assets/create-an-api-only-user-3.png)

1. API 専用ユーザーの電子メール、名、姓を入力します。「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/create-an-api-only-user-4.png)

   >[!TIP]
   >
   >[!UICONTROL 理由]（オプション）または[!UICONTROL アクセスの有効期限]を追加します。短期の従業員には、アクセスの有効期限が便利です。

1. 「**[!UICONTROL API のみ]**」のロールを選択し、「**[!UICONTROL API のみ]**」チェックボックスをオンにします。「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/create-an-api-only-user-5.png)

1. 「**[!UICONTROL 送信]**」をクリックします。

   ![](assets/create-an-api-only-user-6.png)

>[!NOTE]
>
>ポップアップに「招待状は API にのみ必要なものではありません」と表示されますが、何か間違ったことをしたわけではありません。招待メールを送信しなくてもロールが作成されるという意味です。

よろしいですか。先に進んでカスタムサービスを作成しましょう。

>[!MORELIKETHIS]
>
>[REST API で使用するカスタムサービスの作成](/help/marketo/product-docs/administration/additional-integrations/create-a-custom-service-for-use-with-rest-api.md){target="_blank"}
