---
unique-page-id: 1147082
description: フローステップを使用してデータベースからユーザーを削除する方法を説明します。 Marketoから条件を満たすユーザーを削除します。
title: 人物の削除
exl-id: 40039444-9b2a-4b80-93bc-7da3d6e9475c
feature: Smart Campaigns
TQID: https://experienceleague.adobe.com/89EPt9SVBCuluSojdqLE4BawaPGGbzHLSmYHV9w6Uko
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
subfeature_v2:
  - id: ad89fb33-8541-4339-afe7-bb13d1633714
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 127
ht-degree: 84%

---

# 人物の削除 {#delete-person}

誤った人物がデータベースに格納されることがあります。 人物を削除フローステップで削除できます。

![](assets/delete-person-1.png)

>[!CAUTION]
>
>人物を削除すると、その人物の履歴 RCE データもすべて削除されます。 これは元に戻せません。

1. フローステップにドラッグすると、CRM からも自動的に削除されるように設定されます。

   ![](assets/delete-person-2.png)

1. 次のように、CRM ではなく Marketo Engage から削除できます。

   ![](assets/delete-person-3.png)

>[!NOTE]
>
>CRM からの人物の削除は、_[!DNL Salesforce]_ でのみ機能します。 人物を Marketo から削除し、[!DNL Salesforce] で保持することにした場合、[!DNL Salesforce] のレコードが更新された場合は、Marketo で再作成されます。
