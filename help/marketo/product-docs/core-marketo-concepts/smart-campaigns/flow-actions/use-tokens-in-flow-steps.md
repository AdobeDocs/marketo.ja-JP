---
unique-page-id: 1146995
description: フローステップでトークンを使用する方法を説明します。 フローステップのコンテンツとメールに動的な値を挿入します。
title: フローステップでのトークンの使用
exl-id: 9b4c3d57-5906-4d7c-8215-4ba2271be3f8
feature: Smart Campaigns
TQID: https://experienceleague.adobe.com/0b1iseuF-rKtBcS2qPRdwnPPRYJxUNG9hzlJQxNJQdI
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
subfeature_v2:
  - id: ad89fb33-8541-4339-afe7-bb13d1633714
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 200
ht-degree: 91%

---

# フローステップでのトークンの使用 {#use-tokens-in-flow-steps}

>[!PREREQUISITES]
>
>[スマートキャンペーンへのフローステップの追加](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md){target="_blank"}

トークンは変数です。 メール、ランディングページ、スマートキャンペーンで使用することで、作業が手軽になります。 フローステップ、web フック、メール、ランディングページで[マイトークン](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md){target="_blank"}（カスタムトークン）を使用できます。 トークンを使用して、次のフローステップに変数コンテンツを含めることができます。

* データ値の変更
* プログラムメンバーの変更
* 注目のアクション
* [!DNL Salesforce] キャンペーン手順（追加、削除、ステータスの変更）
* タスクの作成
* アラートの送信（トリガーキャンペーンのみ）

1. フローステップで、`{{` と入力し始めると、トークンのカテゴリが表示されます。

   ![](assets/use-tokens-in-flow-steps-1.png)

   >[!NOTE]
   >
   >使用可能なトークンについて、[トークンの概要](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md){target="_blank"}でいくつかリストアップしています。

1. 目的のトークンが見つかるまで入力し続け、クリックして選択します。

   ![](assets/use-tokens-in-flow-steps-2.png)

   >[!TIP]
   >
   >注目のアクション、タスクの作成、アラートの送信の各フローステップでは、複数のトークンを使用できます。

   >[!NOTE]
   >
   >プログラムメンバーカスタムフィールドトークンは、次の場所で使用できます。タスクの作成、Microsoft でのタスクの作成、注目のアクション、データ値の変更フローアクション、web フック。

   スマートキャンペーンが実行されると、データがトークンから取り出されます。

   >[!MORELIKETHIS]
   >
   >* [マイトークンの管理](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md){target="_blank"}
   >* [プログラム内のマイトークンの理解](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md){target="_blank"}
