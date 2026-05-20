---
unique-page-id: 2360301
description: Sales Insightで星と炎のスコアフィールドを設定する方法を説明します。 Marketo スコアフィールドをSalesforceのMSI表示にマッピングします。
title: セールスインサイトで星と炎に使用するスコアフィールドの設定
exl-id: 640f6d53-71ee-4a6d-b28a-82f3825b8f8e
feature: Marketo Sales Insights
TQID: https://experienceleague.adobe.com/ShowS2zjGEHvU9BRJNIlX6XdY127funYi-sjsE9YTNU
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2:
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 169
ht-degree: 86%

---

# [!DNL Sales Insight] で[!UICONTROL 星]と[!UICONTROL 炎]に使用するスコアフィールドの設定 {#set-score-fields-to-be-used-for-stars-and-flames-in-sales-insight}

>[!NOTE]
>
>**管理者権限が必要**

デフォルトでは、[!DNL Marketo Sales Insight] は「**[!UICONTROL リードスコア]**」フィールドを使用して星と炎を計算します。 別のフィールドを選択する場合は、次をおこないます。

>[!TIP]
>
>カスタムスコアフィールドがまだない場合は、[作成](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)します。

>[!NOTE]
>
>**定義**
>
>* **[!UICONTROL 星]**：星は、他のリードと比較した合計リードスコアを表します。
>* **[!UICONTROL 炎]**：炎は緊急度を表し、リードのスコアが最近どの程度変化したかを示します。
>

1. 「**[!UICONTROL 管理者]**」で、「**[!UICONTROL セールスインサイト]**」をクリックします。

   ![](assets/image2014-9-16-13-3a27-3a19.png)

1. **[!UICONTROL リードスコア設定]**&#x200B;で、「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/image2014-9-16-13-3a27-3a33.png)

1. **[!UICONTROL 星]**&#x200B;で使用するフィールドを選択します。

   ![](assets/image2014-9-16-13-3a27-3a45.png)

1. **[!UICONTROL 炎]**&#x200B;で使用するフィールドを選択します。

   ![](assets/image2014-9-16-13-3a28-3a1.png)

1. 「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2014-9-16-13-3a28-3a18.png)

   >[!NOTE]
   >
   >[!DNL Sales insight] の再計算には時間がかかります。 後で CRM をチェックして星と炎を確認できます。

   >[!MORELIKETHIS]
   >
   >[優先度、緊急度、相対スコア、最有望見込客](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md)
