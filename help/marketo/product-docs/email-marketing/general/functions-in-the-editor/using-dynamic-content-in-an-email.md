---
unique-page-id: 2950617
description: メールで動的コンテンツを使用する方法を説明します。 ルールと属性にもとづいて、異なるセグメントに異なるコンテンツを表示します。
title: メールでの動的コンテンツの使用
exl-id: a1178f76-6760-4a4a-9510-f129ee6a9032
feature: Email Editor
source-git-commit: 240b78561db11e169188698880d4707a5c1f64de
workflow-type: tm+mt
source-wordcount: '271'
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
   >また、メール内の要素を動的にすることもできます。 これを行うには、領域を選択し、歯車アイコンをクリックして、**動的にする** （または[実行している内容に応じてスニペット ](/help/marketo/product-docs/personalization/segmentation-and-snippets/snippets/create-a-snippet.md)に置き換える）を選択します。

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
