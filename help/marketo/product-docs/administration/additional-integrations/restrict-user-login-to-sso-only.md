---
unique-page-id: 2360358
description: Admin Login Settingsを介したSSO セキュリティを回避できないように、すべてのユーザーにSSOが必要です（Adobe IMSには適用されません）。
title: ユーザーログインを SSO のみに制限
exl-id: 74915871-dcf5-478d-a5ae-b20c3d2de553
feature: Administration
TQID: https://experienceleague.adobe.com/2YaweRRhrf8po6RR3V64kCan8qQhDNKDrhr7TfnNNJs
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b13bd2ad-8e65-49e5-9691-2a0d31067b35id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2: id: d095671a-1355-40aa-8b5f-06c33c68080bid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 273
ht-degree: 66%

---

# ユーザーログインを SSO のみに制限 {#restrict-user-login-to-sso-only}

[SSO](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)を使用しており、ユーザーがSSO セキュリティを回避できないようにしたい場合は、次の手順に従ってください。

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
>ベストプラクティスは、ユーザーを招待して、ユーザーが招待を受け入れることです。 招待が&#x200B;_受け入れられた後_&#x200B;に、管理者は、「[!UICONTROL SSO が必要]」に設定する必要があります。

>[!TIP]
>
>「**[!UICONTROL SSO が必要]**」を選択した場合は、ロールの設定時に「[シングルサインオンをバイパス](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md)」オプションをオンにすることで、この制限から&#x200B;**[!UICONTROL ユーザーのロール]**&#x200B;を除外できます。 これにより、ユーザーは正常にログインできます。 例えば、管理者ユーザーは、引き続きログイン画面から Marketo にログインする必要が生じる場合があります。 SSO とユニバーサル ID の両方が有効になっている場合、サブスクリプションを切り替えるには「シングルサインオンをバイパス」権限を設定する必要があります。

>[!CAUTION]
>
>新しいユーザーを招待すると、ユーザーに招待メールが届きます。 ただし、**[!UICONTROL SSO]**&#x200B;が選択されている場合は、**[!UICONTROL シングルサインオンをバイパス]**&#x200B;に設定されている役割に割り当てられていない限り、これらのメールは受信されません。

これで、すべてのユーザー（シングルサインオンをバイパスする権限を持つユーザーを除く）は、SSO ログインのみを使用するように制限されました。

>[!MORELIKETHIS]
>
>* [ポータルへのシングルサインオンの追加](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)
>* [ユニバーサル ID を使用して、2 つのインスタンスに Marketo ユーザーを招待](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)
