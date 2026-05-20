---
unique-page-id: 2359500
description: セグメント化の順序の優先順位と、そのセグメントが個人の属するセグメントを決定する方法について説明します。 セグメントの評価を制御するために、データベースでセグメントの順序を編集します。
title: セグメント化の順序の優先度
exl-id: c20d07c8-5e53-4f54-a7a3-2e1aa4fb0cdd
feature: Segmentation
TQID: https://experienceleague.adobe.com/wDvufJzxu0BFCSov4etUpEMxaol3-R5CePqllYyDeSc
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
subfeature_v2:
  - id: a1d50dda-6d94-4e16-8c30-5eb7181c4650
  - id: cdd4e0f6-e87e-453f-88ee-2ee54a7de272
  - id: df8eb12b-4f82-491f-acbb-d74012ca5654
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 144
ht-degree: 80%

---

# セグメント化の順序の優先度 {#segmentation-order-priority}

**順序**&#x200B;が、セグメント化での顧客の評価の優先度をどのように設定するかを理解することが重要です。

>[!PREREQUISITES]
>
>[&#x200B; セグメントの作成](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)
>[セグメントルールの定義](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/define-segment-rules.md)

>[!NOTE]
>
>編集できるのは、ドラフトモードのセグメント化のみです。

1. **データベース**&#x200B;に移動します。

   ![](assets/segmentation-order-priority-1.png)

1. 目的の&#x200B;**セグメント化**&#x200B;を選択します。 **[!UICONTROL セグメント化アクション]**&#x200B;で「**[!UICONTROL セグメントを編集]**」をクリックします。

   ![](assets/segmentation-order-priority-2.png)

   この画面で、セグメントの順序を確認または編集できます。

   ![](assets/segmentation-order-priority-3.png)

>[!NOTE]
>
>* セグメントは相互に排他的です。 ユーザーは一度に 1 つのセグメントのみのメンバーになることができます。
>* ユーザーが 2 つのセグメントに該当する場合、そのユーザーはリストの最初のセグメントにのみ属します。
>* どのセグメントにも該当しないユーザーは、デフォルトセグメントのメンバーになります。
