---
unique-page-id: 1147031
description: SFDC から顧客を削除 - Marketo ドキュメント - 製品ドキュメント
title: SFDC から顧客を削除
exl-id: 8245de35-f374-4241-946e-b4c4b87cc85e
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 100%

---

# SFDC から顧客を削除 {#delete-person-from-sfdc}

特定のリードセットを Marketo に残しつつ、Salesforce から削除したい場合は、「SFDC から顧客を削除」フローアクションを使用できます。

>[!NOTE]
>
>Salesforce との連携時にのみ有効です。

1. データベースで、Salesforce から削除するリードをクリックします。「**リードアクション**」、「**Salesforce**」の順にクリックします。

   ![](assets/person-actions-salesforce.png)

1. 「**SFDC から顧客を削除**」を選択します。

   ![](assets/delete-person-from-sfdc.png)

1. 「**Marketo 内で削除**」設定が **false** になっていることを確認したら、「**実行**」をクリックします。

   ![](assets/run-action-delete-lead-from-sfdc.png)

   フローステップが実行され、リードデータは Salesforce から削除されますが、Marketo には残ります。

   >[!CAUTION]
   >
   >「**Marketo 内で削除**」を **true** に設定して、Salesforce と Marketo の両方からリードを削除すると、リードデータは完全に失われ、元に戻すことはできません。このアクションをやり直すことはできません。
