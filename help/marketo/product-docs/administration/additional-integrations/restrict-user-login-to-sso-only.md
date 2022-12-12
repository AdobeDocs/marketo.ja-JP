---
unique-page-id: 2360358
description: ユーザログインを SSO のみに制限 - Marketo ドキュメント - 製品ドキュメント
title: ユーザログインを SSO のみに制限
exl-id: 74915871-dcf5-478d-a5ae-b20c3d2de553
source-git-commit: 5f509a7aa27692e54bf129b94c657aff0f645f2b
workflow-type: ht
source-wordcount: '233'
ht-degree: 100%

---

# ユーザログインを SSO のみに制限 {#restrict-user-login-to-sso-only}

[SSO を使用していて](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)、ユーザが SSO セキュリティをバイパスできないようにする場合は、次の手順に従います。

>[!IMPORTANT]
>
>この記事は、[Adobe IMS 対応](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md) Marketo サブスクリプションには適用されません。

>[!NOTE]
>
>**管理者権限が必要**

1. 「**管理者**」領域に移動します。

   ![](assets/restrict-user-login-to-sso-only-1.png)

1. 「**ログイン設定**」をクリックします。

   ![](assets/restrict-user-login-to-sso-only-2.png)

1. 「**セキュリティ設定を編集**」をクリックします。

   ![](assets/restrict-user-login-to-sso-only-3.png)

1. 「詳細設定」を展開し、「**SSO が必要**」をオンにして、「**保存**」をクリックします。

![](assets/restrict-user-login-to-sso-only-4.png)

>[!NOTE]
>
>ベストプラクティスは、ユーザを招待して、ユーザが招待を受け入れることです。ユーザが招待を&#x200B;_受け入れた後_&#x200B;に、管理者は、「SSO が必要」に設定する必要があります。

>[!TIP]
>
>「**SSO が必要**」を選択した場合は、ロールの設定時に「[シングルサインオンをバイパス](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md)」オプションをオンにすることで、この制限から&#x200B;**ユーザのロール**&#x200B;を除外できます。これにより、ユーザは通常どおりにログインできます。例えば、管理者ユーザは、引き続きログイン画面から Marketo にログインする必要が生じる場合があります。

>[!CAUTION]
>
>新しいユーザを招待すると、ユーザに招待メールが届きます。ただし、「**SSO が必要**」が選択されている場合は、「**シングルサインオンをバイパス**」に設定されているロールに割り当てられていない限り、招待メールは届きません。

これで完了です。これで、すべてのユーザが、SSO ログインのみを使用するように制限されます（シングルサインオンをバイパスする権限を持つユーザを除く）。

>[!MORELIKETHIS]
>
>* [ポータルへのシングルサインオンの追加](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)
>* [サブスクリプションログインでのユニバーサル ID の使用](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md)
>* [ユニバーサル ID を使用して、2 つのインスタンスに Marketo ユーザを招待](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)

