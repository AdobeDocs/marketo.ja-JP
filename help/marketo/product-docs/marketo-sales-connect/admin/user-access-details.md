---
unique-page-id: 14352623
description: Sales Connectの管理者権限と管理者以外のユーザー権限について説明します。 テンプレート、キャンペーン、人物に対して各役割が何にアクセスできるかを把握します。
title: ユーザアクセスの詳細
exl-id: 6a61176c-acbd-4684-983f-1c5af0ca6187
feature: Marketo Sales Connect
TQID: 'https://experienceleague.adobe.com/R6ZtthzpNCoE7mMQX3NxjBcrpMBRPCDILsVz5-aGWRY'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
    internal-label: Templates
  - id: ab9cc269-26ac-5c58-b645-e0736aefe9f3
    internal-label: Marketo Sales Connect
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 91%
---
# ユーザアクセスの詳細 {#user-access-details}

管理者と管理者以外のユーザは何にアクセスできますか？

## 管理者ユーザーの権限 {#admin-user-permissions}

管理者は[すべてのテンプレートを表示](/help/marketo/product-docs/marketo-sales-connect/templates/view-template-list-as-another-user.md)できます。

![](assets/templates.jpg)

管理者は[すべてのキャンペーンを表示](/help/marketo/product-docs/marketo-sales-connect/campaigns/view-campaigns-list-as-another-user.md)できます。

![](assets/campaigns.jpg)

管理者は、すべてのメールアクティビティを表示できます。

![](assets/user-access-details-3.png)

管理者は、実行中のキャンペーンに含まれるすべての人物を表示できます。

![](assets/running.jpg)

すべての人物レコードは、「全員」グループからアクセスできます。

![](assets/viewed.jpg)

管理者は、ユーザの代わりにキャンペーンを停止できます。

## 管理者以外のユーザー権限 {#non-admin-user-permissions}

* 分析：

  * ユーザはチームの分析を表示できます。
  * ユーザは所属するチームのみの詳細を表示できます
  * ユーザは自分の分析を表示できます

* 関係ページ：

  * ユーザは全員とグループを共有できます
  * ユーザは、所属するチームとのみグループを共有できます
  * ユーザーが削除されると、そのユーザーの共有取引先責任者の所有権は、そのユーザーを削除したマスター管理者に移転されます

* Sales Beat - 次とライブフィード：

  * ユーザは「全員」ビューを表示できます
  * ユーザは所属するチームでフィルターできます
  * ユーザーは全員と投稿を共有できます。
  * ユーザは、所属するチームとのみ投稿を共有できます。

* チーム管理ページ：

  * 表示できません

* テンプレートページ：

  * ユーザは全員とテンプレートを共有できます。
  * ユーザは、管理者が許可するカテゴリにテンプレートを共有できます。
  * ユーザーがチームから削除されると、そのユーザーのテンプレートはそのチームと共有されなくなります。
  * ユーザーがチームから削除されると、そのユーザーのテンプレートの所有権が、そのユーザーを削除したマスター管理者に移転されます。
