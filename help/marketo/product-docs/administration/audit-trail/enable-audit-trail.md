---
unique-page-id: 11382122
description: 役割の監査証跡とログイン履歴を有効にし、管理者権限を使用して役割をユーザーに割り当てます。
title: 監査記録の有効化
exl-id: 3ab2d7b2-1be1-4b3f-a9cc-d3edfa963679
feature: Audit Trail
TQID: 'https://experienceleague.adobe.com/-JXuS64rGSiaTMaiwUfzQWBAekwzj-53w8A2q1oLQWg'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
    internal-label: Configuration
subfeature_v2:
  - id: f7d2c504-7d5f-4a94-b77e-7fce7ef46c22
    internal-label: Audit trail
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 79%
---
# 監査記録の有効化 {#enable-audit-trail}

監査記録は、すべての顧客が使用でき、2 つの管理権限で制御されます。

>[!NOTE]
>
>デフォルトでは、すべてのシステム管理者のロールで、両方の権限が有効になっています。

## ロールの監査記録を有効にする {#enable-audit-trail-for-a-role}

1. 「**[!UICONTROL 管理者]**」をクリックします。

   ![](assets/enable-audit-trail-1.png)

1. 「**[!UICONTROL ユーザー＆ロール]**」を選択し、「**[!UICONTROL ロール]**」をクリックします。

   ![](assets/enable-audit-trail-2.png)

1. 監査記録を有効にするロールを選択し、「**[!UICONTROL ロールの編集]**」をクリックします。

   ![](assets/enable-audit-trail-3.png)

   >[!NOTE]
   >
   >ここで新しいロールを作成し、そのロールに監査記録へのアクセス権を付与することもできます。

1. **[!UICONTROL 管理アクセス]**&#x200B;権限を展開します。 必要に応じて、「**[!UICONTROL 監査記録にアクセス]**」と「**[!UICONTROL ログイン履歴にアクセス]**」のいずれかまたは両方を選択します。 「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/enable-audit-trail-4.png)

   >[!NOTE]
   >
   >**定義**
   >
   >**[!UICONTROL 監査記録にアクセス]** - [!UICONTROL アセット監査記録]と[!UICONTROL 管理監査記録]の両方にアクセスできるようにします。
   >
   >**[!UICONTROL ログイン履歴にアクセス]**：[ユーザーログイン履歴](/help/marketo/product-docs/administration/audit-trail/user-login-history.md)にアクセスできるようにします。

## 監査記録ロールをユーザーに割り当てる {#assign-audit-trail-role-to-a-user}

>[!PREREQUISITES]
>
>ロールを[作成](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md#create-a-role)するか、既存のロールを[有効](#enable-audit-trail)にして、監査記録の権限を付与します。

1. **[!UICONTROL ユーザー＆ロール]**&#x200B;で、「**[!UICONTROL ユーザー]**」をクリックします。

   ![](assets/enable-audit-trail-5.png)

1. 監査記録の権限を付与するユーザーを選択して、「**[!UICONTROL ユーザーを編集]**」をクリックします。

   ![](assets/enable-audit-trail-6.png)

   >[!NOTE]
   >
   >このプロセスは、新しいユーザーを作成する場合にも適用されます。

1. 作成した監査記録のロールを選択します。 この例では、「監査記録 – アセットと管理者」および「監査記録 – ログイン履歴あり」を作成する方法を示します。

   ![](assets/enable-audit-trail-7.png)

   >[!CAUTION]
   >
   >ワークスペースを有効にしている場合は、必ずロールのチェックボックスを選択してください。これにより、すべてのワークスペースが選択されます。 個々のワークスペースの選択を解除すると、監査証跡が非表示になります。 [フィルター](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md)を適用すると、ワークスペースを非表示にするオプションがあります。

1. 「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/enable-audit-trail-8.png)
