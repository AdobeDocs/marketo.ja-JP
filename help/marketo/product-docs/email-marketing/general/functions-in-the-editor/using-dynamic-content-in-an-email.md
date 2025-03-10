---
unique-page-id: 2950617
description: メールでの動的コンテンツの使用 - Marketo ドキュメント - 製品ドキュメント
title: メールでの動的コンテンツの使用
exl-id: a1178f76-6760-4a4a-9510-f129ee6a9032
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 100%

---

# メールでの動的コンテンツの使用 {#using-dynamic-content-in-an-email}

>[!PREREQUISITES]
>
>[セグメント化の作成](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)

メール内の動的コンテンツを使用して、リードのターゲット情報を送信します。

>[!NOTE]
>
>メール内での動的コンテンツ内での変数の使用は、トリガーキャンペーンの使用時にのみサポートされます。これは、バッチキャンペーンを使用する場合にはサポート&#x200B;**されません**。

## セグメント化を追加 {#add-segmentation}

1. 「**マーケティングアクティビティ**」に移動します。

   ![](assets/login-marketing-activities.png)

1. メールを選択して、「**ドラフトの編集**」をクリックします。

   ![](assets/1.2.png)

1. この例では、件名を動的にします。件名フィールドをクリックし、「**動的にする**」ボタンをクリックします。

   ![](assets/1.3.png)

   >[!NOTE]
   >
   >また、メール内の要素を動的にすることもできます。それには、領域を選択し、歯車アイコンをクリックして、「**動的にする**」（または実行内容に応じて「[スニペットに置換](/help/marketo/product-docs/personalization/segmentation-and-snippets/snippets/create-a-snippet.md)」）をクリックします。

1. セグメント名を入力して選択し、「**保存**」をクリックします。

   ![](assets/1.4.png)

   セグメント化とそのセグメントが右側の「動的」タブに表示されます。

   ![](assets/1.5.png)

## 動的コンテンツの適用 {#apply-dynamic-content}

>[!CAUTION]
>
>使用できる動的コンテンツ要素の数に制限はありません。具体的な数の制限はありませんが（コンテンツの組み合わせによって異なる場合があります）、動的コンテンツを過剰に使用すると、メールのパフォーマンスに悪影響を与える可能性があります。従来の動的コンテンツ要素の量は、メールあたり 20 未満にすることをお勧めします。

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

できましたね。これで、ターゲットオーディエンスに適応したメールを送信できます。

>[!MORELIKETHIS]
>
>* [動的コンテンツを含むメールのプレビュー](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/preview-an-email-with-dynamic-content.md)
>* [ランディングページでの動的コンテンツの使用](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/use-dynamic-content-in-a-free-form-landing-page.md)
