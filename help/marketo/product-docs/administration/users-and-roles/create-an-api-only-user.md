---
unique-page-id: 2360207
description: API 専用ユーザーの作成 - Marketo ドキュメント - 製品ドキュメント
title: API 専用ユーザーの作成
exl-id: 23c92255-07a8-41c2-b7b8-8e495d135671
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '163'
ht-degree: 100%

---

# API 専用ユーザーの作成 {#create-an-api-only-user}

[REST API](https://developers.marketo.com/documentation/rest/) を使用して Marketo と統合する場合は、API 専用ユーザーを作成する必要があります。手順は以下のとおりです。

>[!PREREQUISITES]
>
>[API 専用ユーザーの役割の作成](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md)

>[!NOTE]
>
>**管理者権限が必要**

1. 「**管理者**」で「**ユーザーと役割**」をクリックします。

   ![](assets/image2014-9-17-9-3a31-3a31.png)

1. 「**新しいユーザーを招待**」をクリックします。

   ![](assets/image2014-9-17-9-3a32-3a3.png)

1. API 専用ユーザーの電子メール、名、姓を入力します。「**次へ**」をクリックします。

   ![](assets/image2016-5-24-10-3a53-3a7.png)

   >[!TIP]
   >
   >理由（オプション）またはアクセスの有効期限を追加します。短期の従業員には、アクセスの有効期限が便利です。

1. 「**API のみ**」の役割を選択し、「**API のみ**」チェックボックスをオンにします。「**次へ**」をクリックします。

   ![](assets/four.png)

1. 「**送信**」をクリックします。

   ![](assets/image2016-5-24-11-3a8-3a20.png)

>[!NOTE]
>
>ポップアップに「招待状は API にのみ必要なものではありません」と表示されますが、何か間違ったことをしたわけではありません。招待メールを送信しなくても役割が作成されるという意味です。

よろしいですか。先に進んでカスタムサービスを作成しましょう。

>[!MORELIKETHIS]
>
>[ReST API で使用するカスタムサービスの作成](/help/marketo/product-docs/administration/additional-integrations/create-a-custom-service-for-use-with-rest-api.md)
