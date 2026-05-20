---
unique-page-id: 2950617
description: メールで動的コンテンツを使用する方法を説明します。 ルールと属性にもとづいて、異なるセグメントに異なるコンテンツを表示します。
title: メールでの動的コンテンツの使用
exl-id: a1178f76-6760-4a4a-9510-f129ee6a9032
feature: Email Editor
TQID: https://experienceleague.adobe.com/NzTat-p-dgq9wtHv-hyJJzAwud27aOBvVTIS1Tn0lnc
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
subfeature_v2:
  - id: a1d50dda-6d94-4e16-8c30-5eb7181c4650
  - id: cdd4e0f6-e87e-453f-88ee-2ee54a7de272
  - id: df8eb12b-4f82-491f-acbb-d74012ca5654
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 271
ht-degree: 83%

---

# メールでの動的コンテンツの使用 {#using-dynamic-content-in-an-email}

>[!PREREQUISITES]
>
>[セグメント化の作成](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)

メール内の動的コンテンツを使用して、リードのターゲット情報を送信します。

>[!NOTE]
>
>メール内での動的コンテンツ内での変数の使用は、トリガーキャンペーンの使用時にのみサポートされます。 これは、バッチキャンペーンを使用する場合にはサポート&#x200B;**されません**。

## セグメント化を追加 {#add-segmentation}

1. **[!UICONTROL マーケティングアクティビティ]**&#x200B;に移動します。

   ![](assets/login-marketing-activities.png)

1. メールを選択して、「**[!UICONTROL ドラフトを編集]**」をクリックします。

   ![](assets/1.2.png)

1. この例では、件名を動的にします。 「[!UICONTROL 件名]」フィールドをクリックし、「**動的にする**」ボタンをクリックします。

   ![](assets/1.3.png)

   >[!NOTE]
   >
   >また、メール内の要素を動的にすることもできます。 これを行うには、領域を選択し、歯車アイコンをクリックして、**動的にする** （または[実行している内容に応じてスニペット &#x200B;](/help/marketo/product-docs/personalization/segmentation-and-snippets/snippets/create-a-snippet.md)に置き換える）を選択します。

1. セグメント名を入力して選択し、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/1.4.png)

   セグメント化とそのセグメントが右側の「[!UICONTROL 動的]」タブに表示されます。

   ![](assets/1.5.png)

## 動的コンテンツの適用 {#apply-dynamic-content}

>[!CAUTION]
>
>使用できる動的コンテンツ要素の数に制限はありません。 具体的な数の制限はありませんが（コンテンツの組み合わせによって異なる場合があります）、動的コンテンツを過剰に使用すると、メールのパフォーマンスに悪影響を与える可能性があります。 従来の動的コンテンツ要素の量は、メールあたり 20 未満にすることをお勧めします。

1. セグメントをクリックし、件名を追加します。

![](assets/2.1.png)

1. 各セグメントに対して繰り返します。

   ![](assets/2.2.png)

>[!TIP]
>
>様々なセグメントにコンテンツを適用する前に、デフォルトのメールを作成します。

>[!CAUTION]
>
>デフォルトのセグメントコンテンツブロックに対する変更は、すべてのセグメントに適用されます。

できましたね。 これで、ターゲットオーディエンスに適応したメールを送信できます。

>[!MORELIKETHIS]
>
>* [動的コンテンツを含むメールのプレビュー](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/preview-an-email-with-dynamic-content.md)
>* [ランディングページでの動的コンテンツの使用](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/use-dynamic-content-in-a-free-form-landing-page.md)
