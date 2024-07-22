---
unique-page-id: 2359906
description: Marketo ユーザーの管理 - Marketo ドキュメント - 製品ドキュメント
title: Marketo ユーザーの管理
exl-id: 40506d3c-a7cb-45fb-bc10-021bd0c70806
feature: Users and Roles
source-git-commit: ab4358ac1d3e1aa1d3733fa5191c5d59022bdf9f
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 100%

---

# Marketo ユーザーの管理 {#managing-marketo-users}

>[!IMPORTANT]
>
>この記事は、[Adobe ID で Marketo](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md){target="_blank"} を使用し&#x200B;_ない_&#x200B;ユーザのみを対象としています。その場合は、[この記事](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md){target="_blank"}の手順に従ってください。

## ユーザーを作成する {#create-users}

1. 「**[!UICONTROL 管理者]**」領域に移動します。

   ![](assets/managing-marketo-users-1.png)

1. 「**[!UICONTROL ユーザー＆ロール]**」をクリックします。

   ![](assets/managing-marketo-users-2.png)

1. 「**[!UICONTROL 新しいユーザーを招待]**」をクリックします。

   ![](assets/managing-marketo-users-3.png)

1. **[!UICONTROL メール]**、**[!UICONTROL 名]**、**[!UICONTROL 姓]**&#x200B;を入力します。

   ![](assets/managing-marketo-users-4.png)

1. 必要に応じて、招待の理由を入力し、日付選択を使用して「**[!UICONTROL アクセス有効期限]**」フィールドで有効期限を選択します。

   ![](assets/managing-marketo-users-5.png)

1. 「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/managing-marketo-users-6.png)

   >[!TIP]
   >
   >有効期限は、Marketo に短時間のみアクセスする必要がある、短期間の外部の関係者やコンサルタントに最適です。

   >[!NOTE]
   >
   >有効期限が来ると、ユーザーは有効期限通知を受け取り、アカウントがロックされます。

1. 任意の「**[!UICONTROL ロール]**」を選択し、「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/managing-marketo-users-7.png)

1. 必要に応じて、招待メッセージを編集します。「**送信**」をクリックします。

   ![](assets/managing-marketo-users-8.png)

   >[!NOTE]
   >
   >メール（ログイン名）は一意でなくてはなりません。サンドボックスで既に使用されている場合、本番環境では別のメールアドレスが必要になります。その逆も同様です。

   ![](assets/managing-marketo-users-9.png)

   >[!NOTE]
   >
   >招待は、新しいユーザーが追加されてから 3 日で期限切れになります。

アカウント有効化の手順を記したメールがユーザーに送信されます。

## ユーザーを削除する {#delete-users}

>[!NOTE]
>
>削除するユーザが Dynamic Chat ユーザでもある場合は、Marketo Engage で削除する前に、Admin Console で [Dynamic Chat からユーザを削除](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users.md#remove-a-chat-user){target="_blank"}する必要があります。

1. 「**[!UICONTROL 管理者]**」領域に移動します。

   ![](assets/managing-marketo-users-10.png)

1. 「**[!UICONTROL ユーザー＆ロール]**」をクリックします。

   ![](assets/managing-marketo-users-11.png)

1. 削除するユーザーを選択し、「**[!UICONTROL ユーザーの削除]**」をクリックします。

   ![](assets/managing-marketo-users-12.png)

1. 「**[!UICONTROL OK]**」をクリックして確認します。

   ![](assets/managing-marketo-users-13.png)

## ユーザーのパスワードをリセットする {#reset-user-passwords}

1. 「**[!UICONTROL 管理者]**」領域に移動します。

   ![](assets/managing-marketo-users-14.png)

1. 「**[!UICONTROL ユーザー＆ロール]**」をクリックします。

   ![](assets/managing-marketo-users-15.png)

1. ユーザーを選択して「**[!UICONTROL パスワードをリセット]**」をクリックします。

   ![](assets/managing-marketo-users-16.png)

1. 「**[!UICONTROL 閉じる]**」をクリックして、プロンプトを閉じます。

   ![](assets/managing-marketo-users-17.png)

パスワードのリセット手順を記したメールがユーザーに送信されます。

>[!TIP]
>
>ユーザーからメールが届かないと申告があった場合、迷惑メールフォルダーに振り分けられている可能性があるので、確認を促してください。

## 権限の変更とユーザー情報の編集 {#change-permissions-and-edit-user-information}

1. 「**[!UICONTROL 管理者]**」領域に移動します。

   ![](assets/managing-marketo-users-18.png)

1. 「**[!UICONTROL ユーザー＆ロール]**」をクリックします。

   ![](assets/managing-marketo-users-19.png)

1. ユーザーを選択して「**[!UICONTROL ユーザーの編集]**」をクリックします。

   ![](assets/managing-marketo-users-20.png)

1. ユーザーの情報を編集して関連するロールを変更できます。「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/managing-marketo-users-21.png)

>[!CAUTION]
>
>Marketo 管理者があなた 1 人しかいない場合、うっかり自分自身の管理者権限を削除しないようご注意ください。

>[!NOTE]
>
>新しいユーザーが管理者として招待された場合、または管理者が削除された場合、現在のすべての管理者にメール通知が送信されます。

素晴らしいです。これでユーザーの作成、削除、ユーザーパスワードのリセット、ユーザーの編集の方法をマスターできましたね。
