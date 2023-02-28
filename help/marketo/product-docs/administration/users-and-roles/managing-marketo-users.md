---
unique-page-id: 2359906
description: Marketo ユーザーの管理 - Marketo ドキュメント - 製品ドキュメント
title: Marketo ユーザーの管理
exl-id: 40506d3c-a7cb-45fb-bc10-021bd0c70806
source-git-commit: 3bb7e8155491f810cc0e71637482e6da788dc068
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 100%

---

# Marketo ユーザーの管理 {#managing-marketo-users}

## ユーザーを作成する {#create-users}

1. 「**管理者**」領域に移動します。

   ![](assets/managing-marketo-users-1.png)

1. 「**ユーザ＆ロール**」をクリックします。

   ![](assets/managing-marketo-users-2.png)

1. 「**新しいユーザを招待**」をクリックします。

   ![](assets/managing-marketo-users-3.png)

1. **電子メールアドレス**、**名**、**姓**&#x200B;を入力します。

   ![](assets/managing-marketo-users-4.png)

1. 必要に応じて、招待の理由を入力し、日付選択を使用して「**アクセス有効期限**」フィールドで有効期限を選択します。

   ![](assets/managing-marketo-users-5.png)

1. 「**次へ**」をクリックします。

   ![](assets/managing-marketo-users-6.png)

   >[!TIP]
   >
   >有効期限は、Marketo に短時間のみアクセスする必要がある、短期間の外部の関係者やコンサルタントに最適です。

   >[!NOTE]
   >
   >有効期限が来ると、ユーザーは有効期限通知を受け取り、アカウントがロックされます。

1. 任意の「**役割**」を選択し、「**次へ**」をクリックします。

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

1. 「**管理者**」領域に移動します。

   ![](assets/managing-marketo-users-10.png)

1. 「**ユーザ＆ロール**」をクリックします。

   ![](assets/managing-marketo-users-11.png)

1. 削除するユーザーを選択し、「**ユーザーの削除**」をクリックします。

   ![](assets/managing-marketo-users-12.png)

1. 「**OK**」をクリックして確認します。

   ![](assets/managing-marketo-users-13.png)

## ユーザーのパスワードをリセットする {#reset-user-passwords}

1. 「管理者」領域に移動します。

   ![](assets/managing-marketo-users-14.png)

1. 「**ユーザ＆ロール**」をクリックします。

   ![](assets/managing-marketo-users-15.png)

1. ユーザーを選択して「**パスワードのリセット**」をクリックします。

   ![](assets/managing-marketo-users-16.png)

1. 「**閉じる**」をクリックして、プロンプトを閉じます。

   ![](assets/managing-marketo-users-17.png)

パスワードのリセット手順を記したメールがユーザーに送信されます。

>[!TIP]
>
>ユーザーからメールが届かないと申告があった場合、迷惑メールフォルダーに振り分けられている可能性があるので、確認を促してください。

## 権限の変更とユーザー情報の編集 {#change-permissions-and-edit-user-information}

1. 「**管理者**」領域に移動します。

   ![](assets/managing-marketo-users-18.png)

1. 「**ユーザ＆ロール**」をクリックします。

   ![](assets/managing-marketo-users-19.png)

1. ユーザーを選択して「**ユーザの編集**」をクリックします。

   ![](assets/managing-marketo-users-20.png)

1. ユーザーの情報を編集して関連する役割を変更できます。「**保存**」をクリックします。

   ![](assets/managing-marketo-users-21.png)

>[!CAUTION]
>
>Marketo 管理者があなた 1 人しかいない場合、うっかり自分自身の管理者権限を削除しないようご注意ください。

>[!NOTE]
>
>新しいユーザーが管理者として招待された場合、または管理者が削除された場合、現在のすべての管理者にメール通知が送信されます。

素晴らしいです。これでユーザーの作成、削除、ユーザーパスワードのリセット、ユーザーの編集の方法をマスターできましたね。
