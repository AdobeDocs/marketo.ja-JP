---
unique-page-id: 7515133
description: SFDC 同期 - リード／取引先責任者／人物の結合 - Marketo ドキュメント - 製品ドキュメント
title: SFDC 同期 - リード／取引先責任者／人物の結合
exl-id: 0e755c80-27cd-4ba3-b540-d7918264c5f6
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '190'
ht-degree: 100%

---

# SFDC 同期：リード／取引先責任者／人物の結合 {#sfdc-sync-merging-a-lead-contact-person}

場合によっては、ルールをリストするのが最適なこともあります。ここでは、次の手順をおこないます。

* **Salesforce** で 2 つのリードを結合すると、通常の同期は Marketo に通知され、リードは Marketo のユーザーとして自動的に結合されます。
* **Marketo** で 2 人の人物を結合しても、Salesforce のリードと同じプロセスが実行されます。この場合も自動的に処理されます。
* また、**リード（人物）を取引先責任者**&#x200B;に結合する方法も同様です。最終的には両方に 1 つの取引先責任者が存在することになります。
* 結合時には、デフォルトのスコアが合計されます。

>[!NOTE]
>
>スコアが 10 の 3 件のリード（人物）を結合すると、結果として 1 件のリード（人物）とスコア 30 が生成されます。

* 競合するフィールド値は、「勝者レコード」から取得されます。（レコード = 結果のリードまたは取引先責任者）
* 「敗者レコード」（消えるレコード）に値があり、勝者レコードに値がない場合は、敗者レコードが保持されます。つまり、「値は少なくてもないよりは良い」ということです。
* すべてのアクティビティログ項目が結合されます。

>[!NOTE]
>
>[Marketo での人物の結合](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md)に関する詳細をご覧ください。
