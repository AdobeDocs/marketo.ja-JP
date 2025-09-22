---
unique-page-id: 2360358
description: ユーザーログインを SSO のみに制限 - Marketo ドキュメント - 製品ドキュメント
title: ユーザーログインを SSO のみに制限
exl-id: 74915871-dcf5-478d-a5ae-b20c3d2de553
feature: Administration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 100%

---

# ユーザーログインを SSO のみに制限 {#restrict-user-login-to-sso-only}

[SSO を使用していて](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)、ユーザーが SSO セキュリティをバイパスできないようにする場合は、以下の手順に従います。

>[!IMPORTANT]
>
>この記事は、[Adobe IMS 対応](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md) Marketo サブスクリプションには適用されません。

>[!NOTE]
>
>**管理者権限が必要**

1. 「**[!UICONTROL 管理者]**」領域に移動します。

   ![](assets/restrict-user-login-to-sso-only-1.png)

1. 「**[!UICONTROL ログイン設定]**」をクリックします。

   ![](assets/restrict-user-login-to-sso-only-2.png)

1. 「**[!UICONTROL セキュリティ設定を編集]**」をクリックします。

   ![](assets/restrict-user-login-to-sso-only-3.png)

1. 「**[!UICONTROL 詳細設定]**」を展開し、「**[!UICONTROL SSO が必要]**」をオンにして、「**[!UICONTROL 保存]**」をクリックします。

![](assets/restrict-user-login-to-sso-only-4.png)

>[!NOTE]
>
>ベストプラクティスは、ユーザーを招待して、ユーザーが招待を受け入れることです。招待が&#x200B;_受け入れられた後_&#x200B;に、管理者は、「[!UICONTROL SSO が必要]」に設定する必要があります。

>[!TIP]
>
>「**[!UICONTROL SSO が必要]**」を選択した場合は、ロールの設定時に「[シングルサインオンをバイパス](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md)」オプションをオンにすることで、この制限から&#x200B;**[!UICONTROL ユーザーのロール]**&#x200B;を除外できます。これにより、ユーザーは通常どおりにログインできます。例えば、管理者ユーザーは、引き続きログイン画面から Marketo にログインする必要が生じる場合があります。SSO とユニバーサル ID の両方が有効になっている場合、サブスクリプションを切り替えるには「シングルサインオンをバイパス」権限を設定する必要があります。

>[!CAUTION]
>
>新しいユーザーを招待すると、ユーザーに招待メールが届きます。ただし、「**[!UICONTROL SSO が必要]**」が選択されている場合は、「**[!UICONTROL シングルサインオンをバイパス]**」に設定されているロールに割り当てられていない限り、招待メールは届きません。

これで完了です。これで、すべてのユーザーが、SSO ログインのみを使用するように制限されます（シングルサインオンをバイパスする権限を持つユーザーを除く）。

>[!MORELIKETHIS]
>
>* [ポータルへのシングルサインオンの追加](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)
>* [サブスクリプションログインでのユニバーサル ID の使用](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md)
>* [ユニバーサル ID を使用して、2 つのインスタンスに Marketo ユーザーを招待](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)
