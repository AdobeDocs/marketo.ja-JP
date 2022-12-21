---
unique-page-id: 2360337
description: 連結文字列（数式）フィールドの作成と使用 - Marketo Docs - 製品ドキュメント
title: 連結文字列（数式）フィールドの作成と使用
exl-id: 779fbc56-a913-422a-a778-d86cc3ed7d48
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 100%

---

# 連結文字列（数式）フィールドの作成と使用 {#create-and-use-a-concatenated-string-formula-field}

複数のフィールドの値を組み合わせたり、Marketo の数式フィールドを使用して条件付き値を作成したりできます。

1. 「**管理者**」に移動し、「**フィールド管理**」をクリックします。

   ![](assets/image2014-9-19-9-3a44-3a58.png)

1. 「**新規カスタムフィールド**」をクリックします。

   ![](assets/image2014-9-19-9-3a45-3a8.png)

1. **タイプ**&#x200B;には「**数式**」を選択します。

   ![](assets/image2014-9-19-9-3a45-3a17.png)

1. フィールドの「**名前**」を入力し、「**作成**」をクリックします。

   ![](assets/image2014-9-19-9-3a46-3a0.png)

1. 数式フィールドを検索して選択し、「**ルールを編集**」をクリックします。

   ![](assets/image2014-9-19-9-3a46-3a13.png)

1. 以下のスクリーンショットのように、2 つの選択肢を追加し、定義します。

   ![](assets/image2014-9-19-9-3a46-3a25.png)

   >[!TIP]
   >
   >詳しくは、[フローステップのトークン](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md)を参照してください。

1. これで、数式フィールドをトークンとしてメールに追加できます。

   ![](assets/seven.png)

>[!NOTE]
>
>数式フィールドは、ランディングページ、メール、スマートリスト列で使用できます（エクスポートされません）。数式フィールドを含むメールは、バッチキャンペーンを使用して送信することは&#x200B;**できません**。このシナリオでは、[メールスクリプトトークン](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md)を使用してください。

これで完了です。性別に基づいて敬称を含めるスマートフィールドが作成されました。楽しみながらクリエイティブになりましょう。
