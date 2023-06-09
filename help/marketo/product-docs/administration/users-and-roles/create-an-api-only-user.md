---
unique-page-id: 2360207
description: API 専用ユーザーの作成 - Marketo ドキュメント - 製品ドキュメント
title: API 専用ユーザーの作成
exl-id: 23c92255-07a8-41c2-b7b8-8e495d135671
source-git-commit: 2d28d4b473815952231356691b1e9310c61a20f1
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 79%

---

# API 専用ユーザーの作成 {#create-an-api-only-user}

を使用してMarketoと統合する場合は、 [REST API](https://developers.marketo.com/documentation/rest/){target="_blank"}API のみのユーザーを作成する必要があります。 手順は以下のとおりです。

>[!PREREQUISITES]
>
>[API 専用ユーザーの役割の作成](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md){target="_blank"}

>[!NOTE]
>
>**管理者権限が必要**

1. 「**[!UICONTROL 管理者]**」領域に移動します。

   ![](assets/create-an-api-only-user-1.png)

1. 「**[!UICONTROL ユーザ＆ロール]**」をクリックします。

   ![](assets/create-an-api-only-user-2.png)

1. 「**[!UICONTROL 新しいユーザを招待]**」をクリックします。

   ![](assets/create-an-api-only-user-3.png)

1. API 専用ユーザーの電子メール、名、姓を入力します。「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/create-an-api-only-user-4.png)

   >[!TIP]
   >
   >理由（オプション）またはアクセスの有効期限を追加します。短期の従業員には、アクセスの有効期限が便利です。

1. 「**[!UICONTROL API のみ]**」の役割を選択し、「**[!UICONTROL API のみ]**」チェックボックスをオンにします。「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/create-an-api-only-user-5.png)

1. 「**[!UICONTROL 送信]**」をクリックします。

   ![](assets/create-an-api-only-user-6.png)

>[!NOTE]
>
>ポップアップに「招待状は API にのみ必要なものではありません」と表示されますが、何か間違ったことをしたわけではありません。これは、招待メールを送信しなくても役割が作成されることを意味します。

よろしいですか。先に進んでカスタムサービスを作成しましょう。

>[!MORELIKETHIS]
>
>[ReST API で使用するカスタムサービスの作成](/help/marketo/product-docs/administration/additional-integrations/create-a-custom-service-for-use-with-rest-api.md){target="_blank"}
