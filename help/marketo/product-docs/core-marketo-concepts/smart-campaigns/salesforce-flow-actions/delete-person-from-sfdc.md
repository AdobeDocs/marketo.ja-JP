---
unique-page-id: 1147031
description: SFDC から顧客を削除 - Marketo ドキュメント - 製品ドキュメント
title: SFDC から顧客を削除
exl-id: 8245de35-f374-4241-946e-b4c4b87cc85e
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 4bae0126d6b36720e170bea7b6b973508c855633
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 77%

---

# SFDC から顧客を削除 {#delete-person-from-sfdc}

特定のリードセットを Salesforce から削除し、Marketo Engageの担当者として残す必要がある場合は、「SFDC からの担当者の削除」フローアクションを使用できます。

>[!NOTE]
>
>Salesforce との連携時にのみ有効です。

1. データベースで、Salesforce から削除するリードをクリックします。「**[!UICONTROL リードアクション]**」、「**[!DNL Salesforce]**」の順にクリックします。

   ![](assets/person-actions-salesforce.png)

1. 「**[!UICONTROL SFDC から顧客を削除]**」を選択します。

   ![](assets/delete-person-from-sfdc.png)

1. 「**[!UICONTROL Marketo 内で削除]**」設定が **[!UICONTROL false]** になっていることを確認したら、「**[!UICONTROL 実行]**」をクリックします。

   ![](assets/run-action-delete-lead-from-sfdc.png)

   フローステップが実行され、リードデータは Salesforce から削除されますが、Marketo には残ります。

   >[!CAUTION]
   >
   >「**[!UICONTROL Marketo 内で削除]**」を **[!UICONTROL true]** に設定して、Salesforce と Marketo の両方からリードを削除すると、リードデータは完全に失われ、元に戻すことはできません。このアクションをやり直すことはできません。
