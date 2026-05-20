---
unique-page-id: 1147031
description: フローステップを使用してSalesforceからユーザーを削除する方法を説明します。 SFDCからリードまたは連絡先がフローに入ったときに削除します。
title: SFDC からの顧客の削除
exl-id: 8245de35-f374-4241-946e-b4c4b87cc85e
feature: Smart Campaigns, Salesforce Integration
TQID: https://experienceleague.adobe.com/f-Zvc4glfCtAagE314vrZjiWIcD3vaGIKmKGeZO18v0
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 149
ht-degree: 83%

---

# SFDC からの顧客の削除 {#delete-person-from-sfdc}

特定のリードのセットを Marketo Engage に人物として残しつつ、Salesforce から削除したい場合は、「SFDC から顧客を削除」フローアクションを使用できます。

>[!NOTE]
>
>[!DNL Salesforce] と統合されている場合にのみ使用できます。

1. データベースで、Salesforce から削除する人物をクリックします。 「**[!UICONTROL 人物のアクション]**」をクリックし、「**[!DNL Salesforce]**」を選択します。

   ![](assets/delete-person-from-sfdc-1.png)

1. 「**[!UICONTROL SFDC から顧客を削除]**」を選択します。

   ![](assets/delete-person-from-sfdc-2.png)

1. 「**[!UICONTROL Marketo 内で削除]**」設定が **[!UICONTROL false]** になっていることを確認したら、「**[!UICONTROL 実行]**」をクリックします。

   ![](assets/delete-person-from-sfdc-3.png)

   フローステップが実行され、人物は [!DNL Salesforce] でリードではなくなりますが、Marketo には残ります。

   >[!CAUTION]
   >
   >「**[!UICONTROL Marketo 内で削除]**」を **[!UICONTROL true]** に設定して、Salesforce と Marketo の両方からリードを削除すると、リードデータは完全に失われ、元に戻すことはできません。 このアクションをやり直すことはできません。
