---
unique-page-id: 2360327
description: CRMから適切なユーザーのパーティションにユーザーをルーティングするための割り当てルールの設定方法。
title: 割り当てルールを使用した人物パーティションの割り当て
exl-id: 6b54dcb7-8da9-466b-b153-099ebcb96424
feature: Partitions
TQID: https://experienceleague.adobe.com/7e7A0wXFiKVttSm7BXEJYtVBnSW6qAah1ygNqO4qdr0
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 170
ht-degree: 84%

---

# 割り当てルールを使用した人物パーティションの割り当て {#assigning-person-partitions-with-assignment-rules}

>[!NOTE]
>
>**管理者権限が必要**

>[!PREREQUISITES]
>
>[人物パーティションの作成](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-person-partition.md)

人物パーティションを使用する場合、CRM から作成された人物をそれぞれのパーティションにルーティングする割り当てルールを設定します。

>[!NOTE]
>
>CRM から Marketo で作成され、SOAP API を介して作成された人物のみに割り当てルールが適用されます。

1. 「**[!UICONTROL 管理者]**」領域に移動します。

   ![](assets/assigning-person-partitions-with-assignment-rules-1.png)

1. 「**[!UICONTROL ワークスペースとパーティション]**」をクリックします。

   ![](assets/assigning-person-partitions-with-assignment-rules-2.png)

1. 「**[!UICONTROL 人物パーティション]**」タブで、「**[!UICONTROL 割り当てルール]**」をクリックします。

   ![](assets/assigning-person-partitions-with-assignment-rules-3.png)

1. 「**[!UICONTROL 選択肢を追加]**」をクリックして、人物パーティションに人物をルーティングする条件を追加します。

   ![](assets/assigning-person-partitions-with-assignment-rules-4.png)

1. 条件を作成するフィールドを選択します。

   ![](assets/assigning-person-partitions-with-assignment-rules-5.png)

1. 選択肢の演算子を選択して、値を入力します。

   ![](assets/assigning-person-partitions-with-assignment-rules-6.png)

1. 条件を満たす人物を対象にする人物パーティションを選択します。

   ![](assets/assigning-person-partitions-with-assignment-rules-7.png)

   >[!NOTE]
   >
   >選択肢は好きなだけ追加できます。

1. 「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/assigning-person-partitions-with-assignment-rules-8.png)

ユーザーのパーティションの割り当てルールが設定されました。

>[!NOTE]
>
>以前の条件が満たされない場合、デフォルトの選択肢が適用されます。
