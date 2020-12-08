---
unique-page-id: 2360358
description: ユーザーログインのSSOのみに制限 — Marketto Docs — 製品ドキュメント
title: ユーザーログインをSSOのみに制限
translation-type: tm+mt
source-git-commit: c33b7ab59e612f37d3f64bb954579700dc574068
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 0%

---


# ユーザーログインをSSOのみに制限 {#restrict-user-login-to-sso-only}

SSOを [](add-single-sign-on-to-a-portal.md) 使用していて、ユーザーがSSOセキュリティをバイパスできないようにするには、次の手順に従います。

>[!NOTE]
>
>**必要な管理者権限**

1. 「管理者」に移動し、「ログイン設定」をクリックします。

![](assets/image2014-9-24-14-3a44-3a40.png)

1. 「セキュリティ設定を編集」をクリックします。

   ![](assets/image2014-9-24-14-3a44-3a53.png)

1. 詳細設定を展開し、「SSOが必要」をチェックして、「保存」をクリックします。

![](assets/image2014-9-24-14-3a45-3a6.png)

>[!TIP]
>
>「SSOを **必須にする」を選択する場合は**、ロールの設定時に [「シングルサインオンを](../../../product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) バイパス **** 」オプションを選択して、この制限からユーザーロールを除外できます。 これにより、ユーザーは通常どおりにサインインできます。 例えば、管理者ユーザーは、引き続きログイン画面を使用してMarketorにログインする必要があります。

>[!CAUTION]
>
>新しいユーザーが招待されると、招待用の電子メールが届きます。 ただし、「SSO **を必須にする** 」を選択した場合は、「シングルサインオンの **バイパス」に設定されているロールに割り当てられていない限り、これらの電子メールは受信されません**。

それだ！ 現在は、すべてのユーザー（シングルサインオンをバイパスする権限を持つユーザーを除く）が、SSOログインのみを使用するように制限されます。