---
unique-page-id: 1147031
description: SFDC から顧客を削除 - Marketo ドキュメント - 製品ドキュメント
title: SFDC からの顧客の削除
exl-id: 8245de35-f374-4241-946e-b4c4b87cc85e
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '133'
ht-degree: 81%

---

# SFDC からの顧客の削除 {#delete-person-from-sfdc}

特定のリードのセットを Marketo Engage に人物として残しつつ、Salesforce から削除したい場合は、「SFDC から顧客を削除」フローアクションを使用できます。

>[!NOTE]
>
>[!DNL Salesforce] と統合されている場合にのみ使用できます。

1. データベースで、Salesforce から削除するリードをクリックします。「**[!UICONTROL 人物のアクション]**」をクリックし、「**[!DNL Salesforce]**」を選択します。

   ![](assets/delete-person-from-sfdc-1.png)

1. 「**[!UICONTROL SFDC から顧客を削除]**」を選択します。

   ![](assets/delete-person-from-sfdc-2.png)

1. 「**[!UICONTROL Marketo 内で削除]**」設定が **[!UICONTROL false]** になっていることを確認したら、「**[!UICONTROL 実行]**」をクリックします。

   ![](assets/delete-person-from-sfdc-3.png)

   フローステップが実行されると、そのユーザーは [!DNL Salesforce] ではリードではなくなり、Marketoには残ります。

   >[!CAUTION]
   >
   >「**[!UICONTROL Marketo 内で削除]**」を **[!UICONTROL true]** に設定して、Salesforce と Marketo の両方からリードを削除すると、リードデータは完全に失われ、元に戻すことはできません。このアクションをやり直すことはできません。
