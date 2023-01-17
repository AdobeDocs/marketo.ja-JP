---
unique-page-id: 2360337
description: 連結文字列（数式）フィールドの作成と使用 - Marketo Docs - 製品ドキュメント
title: 連結文字列（数式）フィールドの作成と使用
exl-id: 779fbc56-a913-422a-a778-d86cc3ed7d48
source-git-commit: b13360b009aea869bbd96a9cd0888bb121afdcd2
workflow-type: ht
source-wordcount: '173'
ht-degree: 100%

---

# 連結文字列（数式）フィールドの作成と使用 {#create-and-use-a-concatenated-string-formula-field}

複数のフィールドの値を組み合わせたり、Marketo の数式フィールドを使用して条件付き値を作成したりできます。

1. 「**管理者**」領域に移動します。

   ![](assets/create-and-use-a-concatenated-string-formula-field-1.png)

1. 「**フィールド管理**」をクリックします。

   ![](assets/create-and-use-a-concatenated-string-formula-field-2.png)

1. 「**新規カスタムフィールド**」をクリックします。

   ![](assets/create-and-use-a-concatenated-string-formula-field-3.png)

1. **タイプ**&#x200B;には「**数式**」を選択します。

   ![](assets/create-and-use-a-concatenated-string-formula-field-4.png)

1. フィールドの「**名前**」を入力し、「**作成**」をクリックします。

   ![](assets/create-and-use-a-concatenated-string-formula-field-5.png)

1. 数式フィールドを検索して選択し、「**ルールを編集**」をクリックします。

   ![](assets/create-and-use-a-concatenated-string-formula-field-6.png)

1. 以下のスクリーンショットのように、2 つの選択肢を追加し、定義します。

   ![](assets/create-and-use-a-concatenated-string-formula-field-7.png)

   >[!TIP]
   >
   >詳しくは、[フローステップのトークン](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md)を参照してください。

1. これで、数式フィールドをトークンとしてメールに追加できます。

   ![](assets/create-and-use-a-concatenated-string-formula-field-8.png)

>[!NOTE]
>
>数式フィールドは、ランディングページ、メール、スマートリスト列で使用できます（エクスポートされません）。数式フィールドを含むメールは、バッチキャンペーンを使用して送信することは&#x200B;**できません**。このシナリオでは、[メールスクリプトトークン](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md)を使用してください。

これで完了です。性別に基づいて敬称を含めるスマートフィールドが作成されました。楽しみながらクリエイティブになりましょう。
