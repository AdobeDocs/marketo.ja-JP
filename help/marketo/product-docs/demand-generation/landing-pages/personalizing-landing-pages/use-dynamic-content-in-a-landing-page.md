---
unique-page-id: 2359532
description: Marketoのランディングページで動的コンテンツを使用する方法を説明します。 セグメントや訪問者に合わせて異なるコンテンツを表示。
title: ランディングページでの動的コンテンツの使用
exl-id: 9f71473b-1805-43ab-b2d7-e4f9854f1944
feature: Landing Pages
TQID: 'https://experienceleague.adobe.com/RuwAISV2vhWpTHsJoE5ny6KRSJf8QA3J-JVrA-gF7oo'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
    internal-label: Personalization
  - id: c2dbad80-0f5c-4d96-a798-2a65f93b8721
    internal-label: Assets
subfeature_v2:
  - id: a1d50dda-6d94-4e16-8c30-5eb7181c4650
    internal-label: Segmentation
  - id: cdd4e0f6-e87e-453f-88ee-2ee54a7de272
    internal-label: Dynamic content
  - id: df8eb12b-4f82-491f-acbb-d74012ca5654
    internal-label: Snippets
  - id: edda586e-0147-48f2-b791-992622a00783
    internal-label: Landing pages
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
    internal-label: Personalization
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 81%
---
# ランディングページでの動的コンテンツの使用 {#use-dynamic-content-in-a-landing-page}

>[!PREREQUISITES]
>
>* [セグメント化の作成](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)
>* [フリーフォームランディングページの作成](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md)
>* [フリーフォームランディングページへの新しいフォームの追加](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/add-a-new-form-to-a-free-form-landing-page.md)

ランディングページで動的コンテンツを使用すると、ターゲットを絞った情報で人々を惹きつけることができます。

## セグメント化を追加 {#add-segmentation}

1. **[!UICONTROL マーケティングアクティビティ]**&#x200B;に移動します。

   ![](assets/login-marketing-activities.png)

   **[!UICONTROL ランディングページ]**&#x200B;をクリックしてから、「**[!UICONTROL ドラフトを編集]**」をクリックします。

   ![](assets/landingpageeditdraft.jpg)

   「**[!UICONTROL セグメント基準]**」をクリックします。

   ![](assets/image2015-5-21-12-3a31-3a20.png)

   「**[!UICONTROL セグメント化名]**」を入力して、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2014-9-16-14-3a50-3a5.png)

   セグメント化とそのセグメントは、右側の「**[!UICONTROL 動的]**」の下に表示されます。

   ![](assets/image2015-5-21-12-3a36-3a40.png)

   >[!NOTE]
   >
   >すべてのランディングページ要素は、デフォルトでは&#x200B;**[!UICONTROL 静的]**&#x200B;です。

## 要素を動的にする {#make-element-dynamic}

1. 「**[!UICONTROL 静的]**」から「**[!UICONTROL 動的]**」に要素をドラッグ＆ドロップします。

   ![](assets/image2014-9-16-14-3a50-3a27.png)

1. また、要素[!UICONTROL 設定]から、要素を[!UICONTROL 静的]または&#x200B;**[!UICONTROL 動的]**&#x200B;にすることもできます。

   ![](assets/image2015-5-21-12-3a39-3a41.png)

## 動的コンテンツを適用する {#apply-dynamic-content}

1. セグメントの下の要素を選択し、「**[!UICONTROL 編集]**」をクリックします。 各セグメントに対して繰り返します。

   ![](assets/image2015-5-21-12-3a42-3a11.png)

1. 緑色のチェックマークは、セグメントに固有のコンテンツを示します。 空白はデフォルトのセグメントコンテンツを示します。

   ![](assets/image2015-5-21-12-3a44-3a24.png)

   >[!CAUTION]
   >
   >デフォルトのセグメントコンテンツブロックに対する変更は、すべてのセグメントに適用されます。

   >[!TIP]
   >
   >様々なセグメントのコンテンツを変更する前に、デフォルトのランディングページを作成します。

これで、セグメントにターゲットコンテンツを送信できます。

>[!MORELIKETHIS]
>
>* [動的コンテンツを含むランディングページのプレビュー](/help/marketo/product-docs/demand-generation/landing-pages/landing-page-actions/preview-a-landing-page-with-dynamic-content.md)
>* [メールでの動的コンテンツの使用](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/using-dynamic-content-in-an-email.md)
