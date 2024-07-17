---
unique-page-id: 1147031
description: SFDC から顧客を削除 - Marketo ドキュメント - 製品ドキュメント
title: SFDC から顧客を削除
exl-id: 8245de35-f374-4241-946e-b4c4b87cc85e
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 934bb5f197f801e48cf8e7554335eb2d07289037
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 73%

---

# SFDC から顧客を削除 {#delete-person-from-sfdc}

Salesforce から特定のリードセットを削除する必要があるが、Marketo Engage内のユーザーとして残す必要がある場合は、「SFDC からユーザーを削除」フローアクションを使用できます。

>[!NOTE]
>
>Salesforce との連携時にのみ有効です。

1. データベースで、Salesforce から削除するリードをクリックします。次に、「**[!UICONTROL 人物アクション]** をクリックし、**[!DNL Salesforce]** を選択します。

   ![](assets/delete-person-from-sfdc-1.png)

1. 「**[!UICONTROL SFDC から顧客を削除]**」を選択します。

   ![](assets/delete-person-from-sfdc-2.png)

1. 「**[!UICONTROL Marketo 内で削除]**」設定が **[!UICONTROL false]** になっていることを確認したら、「**[!UICONTROL 実行]**」をクリックします。

   ![](assets/delete-person-from-sfdc-3.png)

   フローステップが実行され、リードデータは Salesforce から削除されますが、Marketo には残ります。

   >[!CAUTION]
   >
   >「**[!UICONTROL Marketo 内で削除]**」を **[!UICONTROL true]** に設定して、Salesforce と Marketo の両方からリードを削除すると、リードデータは完全に失われ、元に戻すことはできません。このアクションをやり直すことはできません。
