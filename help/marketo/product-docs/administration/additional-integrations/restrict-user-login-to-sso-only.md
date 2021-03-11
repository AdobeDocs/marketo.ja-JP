---
unique-page-id: 2360358
description: ユーザーログインのSSOのみに制限 — Marketto Docs — 製品ドキュメント
title: ユーザーログインをSSOのみに制限
translation-type: tm+mt
source-git-commit: a7c90193e5c934119fa3b6bdf864d1458d1aad7c
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 0%

---


# ユーザーログインをSSOのみに制限{#restrict-user-login-to-sso-only}

SSO](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)を使用して[お客様がSSOセキュリティを回避できないようにする場合は、次の手順に従ってください。

>[!NOTE]
>
>**必要な管理者権限**

1. **管理者**&#x200B;に移動し、**ログイン設定**&#x200B;をクリックします。

   ![](assets/image2014-9-24-14-3a44-3a40.png)

1. 「**セキュリティ設定を編集**」をクリックします。

   ![](assets/image2014-9-24-14-3a44-3a53.png)

1. 詳細設定を展開し、「**SSOを必要**」を選択して、「**保存**」をクリックします。

![](assets/image2014-9-24-14-3a45-3a6.png)

>[!NOTE]
>
>ベストプラクティスは、ユーザーを招待して招待を受諾することです。 _招待が受け入れら_ れたら、管理者は招待を「SSOを必要とする」に設定する必要があります。

>[!TIP]
>
>「**SSOを必須にする**」を選択した場合は、ロールの設定時に「**シングルサインオンをバイパス**」オプションをオンにすると、この制限から[ユーザーロール](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md)を除外できます。 これにより、ユーザーは通常どおりにサインインできます。 例えば、管理者ユーザーは、引き続きログイン画面を使用してMarketorにログインする必要があります。

>[!CAUTION]
>
>新しいユーザーが招待されると、招待用の電子メールが届きます。 ただし、「**SSOを要求**」が選択されている場合、「**シングルサインオンをバイパス**」に設定されている役割に割り当てられていない限り、これらの電子メールは受信されません。

それだ！ 現在は、すべてのユーザー（シングルサインオンをバイパスする権限を持つユーザーを除く）が、SSOログインのみを使用するように制限されます。

>[!MORELIKETHIS]
>
>* [ポータル追加へのシングルサインオン](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)
>* [購読ログインでのユニバーサルIDの使用](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md)
>* [ユニバーサルIDを持つ2つのインスタンスへのマーケティングユーザーの招待](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)

