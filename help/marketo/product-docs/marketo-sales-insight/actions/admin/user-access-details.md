---
description: Sales Insightのアクションで、管理者および管理者以外のユーザーがアクセスできる内容を理解します。 テンプレート、キャンペーン、分析、人物の権限を比較できます。
title: ユーザアクセスの詳細
exl-id: 20e19848-fc46-4f12-af8a-3fa2b88e1af4
feature: Sales Insight Actions
TQID: 'https://experienceleague.adobe.com/cW6bqn-RNZOKcqbcoKCsDVRUwrOIxeXTFrknaXBtGAc'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
    internal-label: Database
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
    internal-label: Templates
  - id: 412786a7-b8da-5b9d-8c3f-2539a3faad9f
    internal-label: Sales Insight Actions
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 90%
---
# ユーザアクセスの詳細 {#user-access-details}

管理者と管理者以外のユーザは何にアクセスできますか？

## 管理者ユーザーの権限 {#admin-user-permissions}

管理者は[すべてのテンプレートを表示](/help/marketo/product-docs/marketo-sales-connect/templates/view-template-list-as-another-user.md)できます。

![](assets/user-access-details-1.png)

管理者は[すべてのキャンペーンを表示](/help/marketo/product-docs/marketo-sales-connect/campaigns/view-campaigns-list-as-another-user.md)できます。

![](assets/user-access-details-2.png)

管理者は、すべてのメールアクティビティを表示できます。

![](assets/user-access-details-3.png)

管理者は、実行中のキャンペーンが適用されているすべての人を表示できます。

![](assets/user-access-details-4.png)

管理者は、「[!UICONTROL 次のユーザとして表示]」ドロップダウンで、ユーザのキャンペーンおよびキャンペーンカテゴリを表示できます。

![](assets/user-access-details-5.png)

管理者は、ユーザの代わりにキャンペーンを停止できます。

## 管理者以外のユーザー権限 {#non-admin-user-permissions}

* 分析：

  * ユーザはチームの分析を表示できます。
  * ユーザは所属するチームのみの詳細を表示できます
  * ユーザは自分の分析を表示できます

* [!UICONTROL 人物]ページ：

  * ユーザは全員とグループを共有できます
  * ユーザは、所属するチームとのみグループを共有できます
  * ユーザは、アクションデータベース内のすべての人物を表示できます
  * ユーザーが削除されると、そのユーザーの共有取引先責任者の所有権は、そのユーザーを削除したマスター管理者に移転されます

* [!UICONTROL チーム]管理ページ：

  * 表示できません

* [!UICONTROL テンプレート]ページ：

  * ユーザは全員とテンプレートを共有できます
  * ユーザは、管理者が許可するカテゴリにテンプレートを共有できます。
  * ユーザーがチームから削除されると、そのユーザーのテンプレートはそのチームと共有されなくなります。
  * ユーザーがチームから削除されると、そのユーザーのテンプレートの所有権が、そのユーザーを削除したマスター管理者に移転されます。
