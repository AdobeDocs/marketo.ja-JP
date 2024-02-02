---
description: メールの検証 - Marketo ドキュメント - 製品ドキュメント
title: メールの検証
exl-id: 976e46a7-8c85-45ed-86c1-0c5cdb2d5c3e
feature: Users and Roles
source-git-commit: c5d5fd490fe2800dc7a34d02c73d728e115646a0
workflow-type: tm+mt
source-wordcount: '466'
ht-degree: 65%

---

# メールの検証 {#email-verification}

Adobe Marketo Engageサブスクリプションを使用する場合、Marketo Engage管理者を含む、API 以外のすべてのユーザーが電子メールアドレスを検証する必要があります。

## この機能が導入された理由 {#why-this-feature-was-introduced}

Marketo Engage では、Adobe ID へのユーザー移行を含む、Adobe Business Platform へのお客様の移行に備えて、メール検証を継続的にロールアウトしています。この機能は、既存の Marketo Engage ユーザーアカウントのセキュリティを強化します。確実に Marketo Engage ユーザーが適切な Adobe ID に関連付けられているようにするために、既存の Marketo Engage ユーザーは、メールアドレスを検証する必要があります。Marketo Engage ユーザーは、Adobe ID に移行される、検証済みのメールアドレスを持っている必要があります。Marketo Engage ユーザーがメールアドレスを検証していない場合、Adobe ID に移行できず、サブスクリプションのユーザー移行の完了後、Marketo サブスクリプションへのアクセス権を失います。

## ユーザー招待 {#user-invite}

管理者がユーザーを招待した場合、招待リンクをクリックすると、そのユーザーは自動的に検証されます。

>[!IMPORTANT]
>
>上記の例外は、 _SSO 専用サブスクリプション内_&#x200B;管理者には新しいユーザーの招待メールが送信されますが、管理者以外のユーザーには送信されません。 管理者以外のユーザーは、レコードを確実に移行するために、電子メールの検証プロセスを実行する必要があります。 ユーザーは、 **管理者** > **マイアカウント** > **アカウント設定** をクリックし、 **検証を再送信**.

![](assets/email-verification-1.png)

## 確認用メール {#verification-email}

配信登録の電子メール検証が有効化された場合、または管理者/ユーザーによってトリガーされた場合、ユーザーは以下の電子メールを受け取ります。

電子メールの検証を成功させるには、アクティブなユーザーセッションが必要です。 ユーザーは、最初に ID プロバイダー (IdP)URL を使用してMarketoサブスクリプションにログインする必要があります。 セッションが確立されると、次のようになります。 _その後_ をクリックします。 **電子メールアドレスを確認** リンクをクリックします。

![](assets/email-verification-2.png)

>[!TIP]
>
>未検証のユーザーに検証メールを再送信するには、レコードを選択し、「**[!UICONTROL メールを確認]**」ボタンをクリックします。

## メールアドレスの変更 {#changing-an-email-address}

ユーザーのメールアドレスが変更されると、そのメールアドレスは検証されなくなります。再検証を許可するメールが送信されます。ユーザーは、「**[!UICONTROL 検証を再送信]**」をクリックして、手動でメールを再送できます。

![](assets/email-verification-3.png)

![](assets/email-verification-4.png)

## ユーザーとロール {#users-and-roles}

**[!UICONTROL 管理者]**／**[!UICONTROL ユーザー＆ロール]**&#x200B;で、「メールのステータス」列に各ユーザーの検証ステータスが表示されます。

![](assets/email-verification-5.png)

## 複数のユーザーのログイン ID {#multiple-user-login-ids}

1 つのユーザーアカウントのみ、単一のメールアドレスに関連付けることができます。単一のメールアドレスに関連付けられた複数のユーザーアカウントがある場合、Marketo Engage では、競合を解決する必要があり、メールアドレスに関連付けられたすべてのユーザーログインが、以下の 3 つの解決オプションと共に表示されます。

* 現在のユーザーログイン ID に現在のメールを使用
* 現在のユーザーログイン ID に新しいメールを使用
* 次回のログインまで決定を延期

  ![](assets/email-verification-6.png)

>[!NOTE]
>
>ユーザーアカウントが単一のアドレスに関連付けらている必要があるのに対して、ユーザーアカウントは、ユニバーサル ID を経由して、多くのサブスクリプションをまたいで使用できます。
