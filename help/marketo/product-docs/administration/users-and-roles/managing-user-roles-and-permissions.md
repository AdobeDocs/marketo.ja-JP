---
unique-page-id: 2359909
description: ユーザーの役割と権限の管理 — Marketoドキュメント — 製品ドキュメント
title: ユーザーの役割と権限の管理
exl-id: e0213c5f-04e0-41a9-ac7b-873e2e39ac79
source-git-commit: a360b46ab1cd7149f609d139590124dcfcda8dad
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 7%

---

# ユーザーの役割と権限の管理 {#managing-user-roles-and-permissions}

ユーザーの役割を設定、作成および編集し、ユーザーに割り当てます。 これにより、各Marketoユーザーがアクセスできる領域と機能を制御できます。

例えば、通常、マーケティングユーザーは、E メール、ランディングページ、プログラムを作成、変更、デプロイするために、アプリケーション全体で幅広いアクセス権を持つ必要があります。 一方、Web デザイナーは、デザインスタジオでほとんどの時間を過ごし、電子メールやランディングページで使用するアセットを作成します。 また、会社のリーダーは Analytics 領域のMarketoのレポートを幅広く利用しますが、アセットやプログラムを自ら作成または駆動する必要がない場合があります。

>[!NOTE]
>
>**管理者権限が必要**

Marketoには、様々なレベルのアクセス権を持つ、次の組み込みの役割が用意されています。

* **管理者**  — 管理セクションを含む、アプリケーションのすべての部分
* **標準ユーザー**  — 管理セクションを除く、アプリケーションのすべての部分
* **マーケティングユーザー**  — 管理セクションを除く、アプリケーションのすべての部分
* **Web デザイナー**  — デザインスタジオのみ
* **Analytics ユーザー** - 「Analytics」セクションのみ

管理者ロールと標準ユーザーロールは編集できませんが、他のロールは編集できます。 また、会社の特定の組織構造に合致する新しいカスタムロールを作成することもできます。

## Marketo と Adobe ID {#marketo-with-adobe-identity}

MarketoをAdobeID と共に使用している場合、プロファイルの説明のリスト [ここにあります](/help/marketo/product-docs/administration/marketo-with-adobe-identity/overview.md#profile-levels).

## ユーザーへのロールの割り当て {#assign-roles-to-a-user}

ユーザーにロールを割り当てる際には、 [初めてのユーザー作成](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) または [既存のユーザーの編集](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md).

1. 既存のユーザーを編集するには、に移動します。 **管理者** をクリックし、 **ユーザーとロール**.

   ![](assets/image2014-9-9-18-3a7-3a32.png)

1. リストから、編集するユーザーを選択し、 **ユーザーを編集**.

   ![](assets/image2014-9-9-18-3a7-3a42.png)

1. の下 **役割**&#x200B;で、必要な権限に応じて、ユーザーに割り当てる役割を選択し、 **保存**.

   ![](assets/image2014-9-9-18-3a7-3a57.png)

   >[!NOTE]
   >
   >各役割について詳しくは、  [役割権限の説明](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions/descriptions-of-role-permissions.md).

## 新しいロールの作成 {#create-a-new-role}

組織には、権限のカスタム組み合わせが必要な特定の役割を持つ従業員がいる場合があります。

1. 新しいユーザーロールを作成するには、「管理者」に移動し、 **ユーザーとロール**.

   ![](assets/image2014-9-9-18-3a8-3a12.png)

1. 次をクリック： **役割** タブをクリックします。

   ![](assets/image2014-9-9-18-3a8-3a22.png)

1. クリック **新しい役割**.

   ![](assets/image2014-9-9-18-3a8-3a38.png)

1. を入力します。 **ロール名**, a **説明** （オプション）を選択し、この役割のユーザーが必要とする権限を選択します。

   ![](assets/image2014-9-9-18-3a9-3a3.png)

## ロールの編集 {#edit-a-role}

既存のロールに関連付けられている権限を変更する必要がある場合は、ロールを編集できます。

1. 「**管理**」エリアに移動して、「**ユーザーと役割**」をクリックします。

   ![](assets/image2014-9-9-18-3a9-3a15.png)

1. 次をクリック： **役割** タブをクリックします。

   ![](assets/image2014-9-9-18-3a9-3a26.png)

1. リストから、変更するロールを選択し、 **ロールの編集**.

   ![](assets/image2014-9-9-18-3a9-3a40.png)

1. を **ロール名** および **説明** 必要に応じて、関連付けられた **権限**.

   ![](assets/image2014-9-9-18-3a10-3a3.png)

   >[!NOTE]
   >
   >編集した役割を持つユーザーは、ログアウトしてから再度ログインすると、変更された権限を受け取ります。

## ロールの削除 {#delete-a-role}

役割が不要になった場合は、役割を削除できます。

1. 「管理」に移動して、「**ユーザーと役割**」をクリックします。

   ![](assets/image2014-9-9-18-3a10-3a15.png)

1. 次をクリック： **役割** タブをクリックします。

   ![](assets/image2014-9-9-18-3a10-3a27.png)

1. リストから、削除するロールを選択し、 **ロールを削除**.

   ![](assets/image2014-9-9-18-3a10-3a39.png)

1. 「**削除**」をクリックして確定します。

   ![](assets/image2014-9-9-18-3a10-3a50.png)
