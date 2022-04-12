---
unique-page-id: 2359909
description: ユーザーの役割と権限の管理 - Marketo ドキュメント - 製品ドキュメント
title: ユーザーの役割と権限の管理
exl-id: e0213c5f-04e0-41a9-ac7b-873e2e39ac79
source-git-commit: a360b46ab1cd7149f609d139590124dcfcda8dad
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 96%

---

# ユーザーの役割と権限の管理 {#managing-user-roles-and-permissions}

ユーザーの役割を設定、作成および編集し、ユーザーに割り当てます。これにより、各 Marketo ユーザーがアクセスできる領域と機能を制御できます。

例えば、通常、マーケティングユーザーは、メール、ランディングページ、プログラムを作成、変更、デプロイするために、アプリケーション全体で幅広いアクセス権を持つ必要があります。一方、web デザイナーは、Design Studio でほとんどの時間を過ごし、メールやランディングページで使用するアセットを作成します。また、会社のリーダーは、分析領域の Marketo のレポートを幅広く利用しますが、アセットやプログラムを自ら作成したり駆動したりする必要はないでしょう。

>[!NOTE]
>
>**管理者権限が必要**

Marketo には様々なレベルのアクセス権を持つ、次の組み込みの役割が用意されています。

* **管理者** - 「管理者」セクションを含む、アプリケーションのすべての部分
* **標準ユーザー** - 「管理者」セクションを除く、アプリケーションのすべての部分
* **マーケティングユーザー** - 「管理者」セクションを除く、アプリケーションのすべての部分
* **Web デザイナー** - Design Studio のみ
* **分析ユーザー** - 「分析」セクションのみ

管理者役割と標準ユーザー役割は編集できませんが、他の役割は編集できます。また、会社の特定の組織構造に合致するカスタムの役割を新たに作成することもできます。

## Marketo と Adobe ID {#marketo-with-adobe-identity}

MarketoをAdobeID と共に使用している場合、プロファイルの説明のリスト [ここにあります](/help/marketo/product-docs/administration/marketo-with-adobe-identity/overview.md#profile-levels).

## ユーザーへの役割の割り当て {#assign-roles-to-a-user}

[初めてユーザーを作成する](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md)とき、または[既存のユーザーを編集](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md)するときに、ユーザーに役割を割り当てることができます。

1. 既存のユーザーを編集するには、「**管理者**」領域に移動して、「**ユーザーと役割**」をクリックします

   ![](assets/image2014-9-9-18-3a7-3a32.png)

1. リストから、編集するユーザーを選択し、「**ユーザーを編集**」をクリックします。

   ![](assets/image2014-9-9-18-3a7-3a42.png)

1. 「**役割**」で、必要な権限に応じてユーザーに割り当てる役割を選択し、「**保存**」をクリックします。

   ![](assets/image2014-9-9-18-3a7-3a57.png)

   >[!NOTE]
   >
   >各役割について詳しくは、[役割権限の説明](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions/descriptions-of-role-permissions.md)を参照してください。

## 役割の新規作成 {#create-a-new-role}

組織によっては、カスタムの権限の組み合わせが必要な特定の役割を持つ従業員がいる場合があります。

1. 新しいユーザー役割を作成するには、「管理者」に移動し、「**ユーザーと役割**」をクリックします。

   ![](assets/image2014-9-9-18-3a8-3a12.png)

1. 「**役割**」タブをクリックします。

   ![](assets/image2014-9-9-18-3a8-3a22.png)

1. 「**新しい役割**」をクリックします。

   ![](assets/image2014-9-9-18-3a8-3a38.png)

1. 「**役割名**」、「**説明**」（オプション）を入力し、この役割のユーザーが必要とする権限を選択します。

   ![](assets/image2014-9-9-18-3a9-3a3.png)

## 役割の編集 {#edit-a-role}

既存の役割に関連付けられている権限を変更する必要がある場合は、役割を編集できます。

1. 「**管理者**」に移動して、「**ユーザーと役割**」をクリックします。

   ![](assets/image2014-9-9-18-3a9-3a15.png)

1. 「**役割**」タブをクリックします。

   ![](assets/image2014-9-9-18-3a9-3a26.png)

1. リストから、変更する役割を選択し、「**役割を編集**」をクリックします。

   ![](assets/image2014-9-9-18-3a9-3a40.png)

1. 必要に応じて、「**役割名**」と「**説明**」を変更し、関連する「**権限**」の選択を変更します。

   ![](assets/image2014-9-9-18-3a10-3a3.png)

   >[!NOTE]
   >
   >編集した役割を持つユーザーは、ログアウトしてから再度ログインすると、変更された権限を受け取ります。

## 役割の削除 {#delete-a-role}

役割が不要になった場合は、役割を削除できます。

1. 「管理者」に移動して、「**ユーザーと役割**」をクリックします。

   ![](assets/image2014-9-9-18-3a10-3a15.png)

1. 「**役割**」タブをクリックします。

   ![](assets/image2014-9-9-18-3a10-3a27.png)

1. リストから、削除する役割を選択し、「**役割を削除**」をクリックします。

   ![](assets/image2014-9-9-18-3a10-3a39.png)

1. 「**削除**」をクリックして確定します。

   ![](assets/image2014-9-9-18-3a10-3a50.png)
