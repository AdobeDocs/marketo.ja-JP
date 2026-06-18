---
unique-page-id: 7515133
description: SalesforceとMarketoでリード、コンタクト、人物を統合する方法を説明します。 スコア、フィールド値、アクティビティログの結合ルールについて説明します。
title: SFDC 同期 - リード／取引先責任者／人物の結合
exl-id: 0e755c80-27cd-4ba3-b540-d7918264c5f6
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/alPa6YMG0tgo08ruZAZlWhujV54iVcUMAAejXJbEQFw
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: 25bbf4409df3db38b849d936e2a90b48f859d089
workflow-type: tm+mt
source-wordcount: 267
ht-degree: 55%

---

# SFDC 同期：リード／取引先責任者／人物の結合 {#sfdc-sync-merging-a-lead-contact-person}

時には、ルールを書き出すのがベストです。 ここでは、次の手順をおこないます。

* **[!DNL Salesforce]** で 2 つのリードを結合すると、通常の同期は Marketo に通知され、リードは Marketo のユーザとして自動的に結合されます。
* **Marketo** で 2 人の人物を結合しても、[!DNL Salesforce] のリードと同じプロセスが実行されます。 この場合も自動的に処理されます。
* また、**リード（人物）を取引先責任者**&#x200B;に結合する方法も同様です。 最終的には両方に 1 つの取引先責任者が存在することになります。
* 結合時には、デフォルトのスコアが合計されます。

>[!NOTE]
>
>スコアが 10 の 3 件のリード（人物）を結合すると、結果として 1 件のリード（人物）とスコア 30 が生成されます。

* 競合するフィールド値は、「勝者レコード」から取得されます。 （レコード = 結果のリードまたは取引先責任者）
* 「失われたレコード」（消えているレコード）に値があり、勝者レコードに値がない（またはnull）場合、失われたレコードは保持されます。 つまり、「値は少なくてもないよりは良い」ということです。
* すべてのアクティビティログ項目が結合されます。

>[!NOTE]
>
>API マージでのブール型フィールドの動作は、&#39;26年3月リリースで変更されました。 ここで、False値は、そのフィールドの値を持つものとして正しく扱われます。 競合するフィールドを評価する場合、null値のみが「空」として扱われます。 詳しくは、[このコミュニティ投稿](https://experienceleaguecommunities.adobe.com/adobe-marketo-engage-27/api-merge-functionality-for-boolean-fields-251219){target="_blank"}を参照してください。

>[!MORELIKETHIS]
>
>[Marketo での人物の結合](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md)に関する詳細をご覧ください。
