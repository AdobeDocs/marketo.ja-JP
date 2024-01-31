---
description: メールの検証 - Marketo ドキュメント - 製品ドキュメント
title: メールの検証
exl-id: 976e46a7-8c85-45ed-86c1-0c5cdb2d5c3e
feature: Users and Roles
source-git-commit: 5ef17e8c3988706a4d95332312ffb035f35bb269
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 78%

---

# メールの検証 {#email-verification}

Adobe Marketo Engageサブスクリプションを使用する場合、Marketo Engage管理者を含む、API 以外のすべてのユーザーが電子メールアドレスを検証する必要があります。

## この機能が導入された理由 {#why-this-feature-was-introduced}

Marketo Engage では、Adobe ID へのユーザー移行を含む、Adobe Business Platform へのお客様の移行に備えて、メール検証を継続的にロールアウトしています。この機能は、既存の Marketo Engage ユーザーアカウントのセキュリティを強化します。確実に Marketo Engage ユーザーが適切な Adobe ID に関連付けられているようにするために、既存の Marketo Engage ユーザーは、メールアドレスを検証する必要があります。Marketo Engage ユーザーは、Adobe ID に移行される、検証済みのメールアドレスを持っている必要があります。Marketo Engage ユーザーがメールアドレスを検証していない場合、Adobe ID に移行できず、サブスクリプションのユーザー移行の完了後、Marketo サブスクリプションへのアクセス権を失います。

## ユーザー招待 {#user-invite}

管理者がユーザーを招待した場合、招待リンクをクリックすると、そのユーザーは自動的に検証されます。

>[!IMPORTANT]
>
>上記の例外は、SSO 専用サブスクリプションでは、管理者は新しいユーザー招待を受け取りますが、管理者以外は受け取りません。 管理者以外のユーザーは、電子メールの検証プロセスを経て、ユーザーレコードを確実に移行する必要があります。 管理者は、 **電子メールの検証を再送信** ボタンをクリックします。

## 確認用メール {#verification-email}

サブスクリプションのメール検証が有効化されるか、管理者／ユーザーによってトリガーされると、ユーザーは、以下のメールを受け取ります

![](assets/email-verification-1.png)

>[!NOTE]
>
>未検証のユーザーに検証メールを再送信するには、レコードを選択し、「**[!UICONTROL メールを確認]**」ボタンをクリックします。

## メールアドレスの変更 {#changing-an-email-address}

ユーザーのメールアドレスが変更されると、そのメールアドレスは検証されなくなります。再検証を許可するメールが送信されます。ユーザーは、「**[!UICONTROL 検証を再送信]**」をクリックして、手動でメールを再送できます。

![](assets/email-verification-2.png)

![](assets/email-verification-3.png)

## ユーザーとロール {#users-and-roles}

**[!UICONTROL 管理者]**／**[!UICONTROL ユーザー＆ロール]**&#x200B;で、「メールのステータス」列に各ユーザーの検証ステータスが表示されます。

![](assets/email-verification-4.png)

## 複数のユーザーのログイン ID {#multiple-user-login-ids}

1 つのユーザーアカウントのみ、単一のメールアドレスに関連付けることができます。単一のメールアドレスに関連付けられた複数のユーザーアカウントがある場合、Marketo Engage では、競合を解決する必要があり、メールアドレスに関連付けられたすべてのユーザーログインが、以下の 3 つの解決オプションと共に表示されます。

* 現在のユーザーログイン ID に現在のメールを使用
* 現在のユーザーログイン ID に新しいメールを使用
* 次回のログインまで決定を延期

  ![](assets/email-verification-5.png)

>[!NOTE]
>
>ユーザーアカウントが単一のアドレスに関連付けらている必要があるのに対して、ユーザーアカウントは、ユニバーサル ID を経由して、多くのサブスクリプションをまたいで使用できます。
