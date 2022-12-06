---
unique-page-id: 11382122
description: 監査記録の有効化 - Marketo ドキュメント - 製品ドキュメント
title: 監査記録の有効化
exl-id: 3ab2d7b2-1be1-4b3f-a9cc-d3edfa963679
source-git-commit: 73d41904ca74ae265648c3ed91805be7c4d24fe0
workflow-type: ht
source-wordcount: '245'
ht-degree: 100%

---

# 監査記録の有効化 {#enable-audit-trail}

監査記録は、すべてのお客様が使用でき、2 つの管理権限で管理されます。

>[!NOTE]
>
>デフォルトでは、すべてのシステム管理者の役割で、両方の権限が有効になっています。

## 役割の監査記録を有効にする {#enable-audit-trail-for-a-role}

1. 「**管理者**」をクリックします。

   ![](assets/enable-audit-trail-1.png)

1. 「**ユーザーと役割**」を選択し、「**役割**」をクリックします。

   ![](assets/enable-audit-trail-2.png)

1. 監査記録を有効にする役割を選択し、「**役割の編集**」をクリックします。

   ![](assets/enable-audit-trail-3.png)

   >[!NOTE]
   >
   >また、新しい役割を作成し、監査記録アクセス権を付与するオプションも表示されます。

1. **管理アクセス**&#x200B;権限を展開します。必要に応じて、「**監査記録にアクセス**」と「**ログイン履歴にアクセス**」のいずれかまたは両方を選択します。「**保存**」をクリックします。

   ![](assets/enable-audit-trail-4.png)

   >[!NOTE]
   >
   >**定義**
   >
   >**監査記録にアクセス**：「アセット監査記録」と「管理監査記録」両方の権限をユーザーに付与します。
   >
   >**ログイン履歴にアクセス**：[ユーザーログイン履歴](/help/marketo/product-docs/administration/audit-trail/user-login-history.md)への権限をユーザーに付与します。

## 監査記録の役割をユーザーに割り当てる {#assign-audit-trail-role-to-a-user}

>[!PREREQUISITES]
>
>役割を[作成](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md#create-a-role)するか、既存の役割を[有効](#enable-audit-trail)にし、監査記録の権限を付与します。

1. **ユーザーと役割**&#x200B;で、「**ユーザー**」をクリックします。

   ![](assets/enable-audit-trail-5.png)

1. 監査記録の権限を付与したいユーザーを選択し「**ユーザーの編集**」をクリックします。

   ![](assets/enable-audit-trail-6.png)

   >[!NOTE]
   >
   >この手順は、新規ユーザーを作成している場合でも同様です。

1. 作成した監査記録の役割を選択します。ここでは、「監査記録 - アセットと管理」と「監査記録 - ログイン履歴」を作成しています。

   ![](assets/enable-audit-trail-7.png)

   >[!CAUTION]
   >
   >ワークスペースを有効にしている場合は、必ず役割のチェックボックスを選択し、ワークスペースをすべて選択してください。個々のワークスペースの選択を解除すると、「監査記録」が非表示になります。つまり、すべてのワークスペースの「監査記録」データが表示されます。[フィルター](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md)を適用すると、ワークスペースを非表示にするオプションがあります。

1. 「**保存**」をクリックします。

   ![](assets/enable-audit-trail-8.png)
