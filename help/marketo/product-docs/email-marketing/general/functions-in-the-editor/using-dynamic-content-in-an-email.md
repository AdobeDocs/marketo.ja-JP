---
unique-page-id: 2950617
description: 電子メールでの動的コンテンツの使用 —Marketoドキュメント — 製品ドキュメント
title: 電子メールでの動的コンテンツの使用
exl-id: a1178f76-6760-4a4a-9510-f129ee6a9032
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 0%

---

# 電子メールでの動的コンテンツの使用{#using-dynamic-content-in-an-email}

>[!PREREQUISITES]
>
>[セグメントの作成](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)

電子メールの動的コンテンツを使用して、リードのターゲット設定情報を送信します。

## 追加セグメント{#add-segmentation}

1. 「マーケティングアクティビティ」に移動します。

   ![](assets/login-marketing-activities.png)

1. 電子メールを選択し、「ドラフトを編集」をクリックします。

   ![](assets/1.2.png)

1. この例では、件名行を動的にします。 「件名」フィールドをクリックし、「**動的にする**」ボタンをクリックします。

   ![](assets/1.3.png)

   >[!NOTE]
   >
   >電子メール内の要素を動的にすることもできます。 これを行うには、領域を選択し、歯車アイコンをクリックし、「**動的に**」（または[スニペット](/help/marketo/product-docs/personalization/segmentation-and-snippets/snippets/create-a-snippet.md)で置き換える）を選択します。

1. セグメント名を入力し、選択して、「**保存**」をクリックします。

   ![](assets/1.4.png)

   セグメントとそのセグメントが右側の「動的」タブに表示されます。

   ![](assets/1.5.png)

## 動的コンテンツの適用{#apply-dynamic-content}

>[!CAUTION]
>
>使用できる動的コンテンツ要素の数に制限はありません。 具体的な数の制限はありません（コンテンツの組み合わせによって異なる場合があります）が、動的なコンテンツを過度に使用すると、電子メールのパフォーマンスに悪影響を与える可能性があります。 電子メールあたり20未満に抑えるために使用する動的コンテンツ要素の量を維持することをお勧めします。

1. セグメントをクリックし、件名を追加します。

![](assets/2.1.png)

1. 各セグメントに対して同じ手順を繰り返します。

   ![](assets/2.2.png)

>[!TIP]
>
>コンテンツを様々なセグメントに適用する前に、デフォルトの電子メールを作成します。

>[!CAUTION]
>
>デフォルトのセグメントコンテンツブロックに対する変更は、すべてのセグメントに適用されます。

甘い！ これで、ターゲットオーディエンスに柔軟な電子メールを送信できます。

>[!MORELIKETHIS]
>
>* [動的コンテンツを使用した電子メールのプレビュー](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/preview-an-email-with-dynamic-content.md)
>* [ランディングページでの動的コンテンツの使用](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/use-dynamic-content-in-a-free-form-landing-page.md)

