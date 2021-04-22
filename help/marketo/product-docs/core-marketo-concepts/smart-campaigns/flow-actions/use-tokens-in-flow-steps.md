---
unique-page-id: 1146995
description: フローステップ —Marketoドキュメント — 製品ドキュメントでのトークンの使用
title: フローステップでのトークンの使用
exl-id: 9b4c3d57-5906-4d7c-8215-4ba2271be3f8
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 8%

---

# フローステップでのトークンの使用{#use-tokens-in-flow-steps}

>[!AVAILABILITY]
>
>この機能を購入していないお客様もいます。  詳細は、営業取引先責任者にお問い合わせください。

>[!PREREQUISITES]
>
>[スマ追加ートキャンペーンへのフローステップ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)

トークンは変数です。 電子メール、ランディングページ、スマートキャンペーンで使用すると、生活が楽になります。 [マイトークン](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md)（カスタムトークン）は、フローステップ、Webフック、電子メール、ランディングページで使用できます。 トークンを使用して、次のフロー手順に変数の内容を含めることができます。

* データ値の変更
* プログラムメンバーの変更
* 注目のアクション
* Salesforceキャンペーン手順（追加、削除、ステータスの変更）
* タスクの作成
* アラートの送信(トリガーキャンペーンのみ)

1. フローステップで、開始が`{{`を入力して、トークンカテゴリを取得します。![](assets/image2014-9-22-14-3a3-3a17.png)

   >[!NOTE]
   >
   >[Tokens Overview](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md)をチェックし、使用可能なトークンのリストを確認します。

1. 目的のトークンが見つかるまで入力を続け、をクリックして選択します。

   ![](assets/image2014-9-22-14-3a3-3a48.png)

   >[!TIP]
   >
   >複数のトークンは、注目の瞬間、タスクの作成、アラートの送信の各フローステップで使用できます。

   >[!NOTE]
   >
   >プログラムメンバのカスタムフィールドトークンは、次の場所で使用できます。タスクの作成、Microsoftでのタスクの作成、おもしろい瞬間、データ値のフローの変更、Webhook

   クール！ スマートキャンペーンの実行時に、データがトークンから取得されます。

   >[!MORELIKETHIS]
   >
   >* [マイトークンの管理](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md)
   >* [プログラム内のマイトークンについて](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md)

