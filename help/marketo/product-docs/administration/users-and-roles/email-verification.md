---
description: メールの検証 - Marketo ドキュメント - 製品ドキュメント
title: メールの検証
exl-id: 976e46a7-8c85-45ed-86c1-0c5cdb2d5c3e
source-git-commit: 44cca5ebad831cc39babac87ac9ebbf53df6c795
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 33%

---

# メールの検証 {#email-verification}

Adobe Marketo Engageサブスクリプションを使用する場合、Marketo Engage管理者を含む、API 以外のすべてのユーザーが電子メールアドレスを検証する必要があります。 管理者の役割が割り当てられていない、または「SSO のバイパス」権限を持つ役割が割り当てられたシングルサインオン (SSO) ユーザーは、電子メールの検証機能で配信が有効になると、自動的に電子メールを検証します。

## ユーザ招待 {#user-invite}

管理者がユーザを招待した場合、招待リンクをクリックすると、そのユーザは自動的に検証されます。管理者の役割が割り当てられていない SSO ユーザーは、自動的に検証されます。

## メールアドレスの変更 {#changing-an-email-address}

ユーザのメールアドレスが変更されると、そのメールアドレスは検証されなくなります。再検証を許可するメールが送信されます。ユーザは、「**検証を再送信**」をクリックして、手動でメールを再送できます。

![](assets/email-verification-1.png)

![](assets/email-verification-2.png)

## ユーザとロール {#users-and-roles}

In **管理者** > **ユーザーとロール**「 E メールステータス」列には、各ユーザーの検証ステータスが表示されます。

![](assets/email-verification-3.png)

## 複数のユーザーログイン ID {#multiple-user-login-ids}

1 つの電子メールアドレスに関連付けることができるユーザーアカウントは 1 つだけです。 1 つの電子メールアドレスに複数のMarketo Engageアカウントが関連付けられている場合、競合を解決し、その電子メールアドレスに関連するすべてのユーザーログインと 3 つの解決オプションを表示する必要があります。<p>
`1` 現在のユーザーログイン ID に対して現在の電子メールを使用<p>
`2` 現在のユーザーログイン ID に新しい電子メールを使用<p>
`3` 次回のログインまで決定を遅延

![](assets/email-verification-4.png)

## 確認メール {#verification-email}

招待されたユーザーには次の電子メールが送信されます。

![](assets/email-verification-5.png)

>[!NOTE]
>
>未検証のユーザに検証メールを再送信するには、レコードを選択し、「**メールを確認**」ボタンをクリックします。
