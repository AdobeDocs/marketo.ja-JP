---
unique-page-id: 1146995
description: フローステップ — Marketto Docs — 製品ドキュメントでのトークンの使用
title: フローステップでのトークンの使用
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 0%

---


# フローステップでのトークンの使用 {#use-tokens-in-flow-steps}

>[!PREREQUISITES]
>
>* [スマ追加ートキャンペーンへのフローステップ](add-a-flow-step-to-a-smart-campaign.md)


トークンは変数です。 これを [電子メール](https://docs.marketo.com/pages/viewpage.action?pageId=557076)、 [ランディングページ](https://docs.marketo.com/pages/viewpage.action?pageId=2359689)、 [](https://docs.marketo.com/display/DOCS/Smart+Lists+and+Lists) スマートキャンペーンで使用すると、生活が楽になります。 フローステップ、Webフック、電子メール、ランディングページで [マイトークン](../../../../product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md) （カスタムトークン）を使用できます。  トークンを使用して、次のフロー手順に変数の内容を含めることができます。

* データ値の変更
* 面白い瞬間
* Salesforceキャンペーン手順（追加、削除、ステータスの変更）
* タスクの作成
* アラートの送信(トリガーキャンペーンのみ)

>[!NOTE]
>
>**可用性**
>
>この機能を購入していないお客様もいます。 詳細については、セールス担当者にお問い合わせください。

1. フロー手順で、開始入力を行ってトークンカテゴリ `{{` を取得します。 ![](assets/image2014-9-22-14-3a3-3a17.png)>

   >[!NOTE]
   >
   >**ディープダイブ**
   >
   >使用可能な複数のトークンのリストについては、 [Tokens Overview](../../../../product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) （トークンの概要）をチェックアウトします。

1. 目的のトークンが見つかるまで入力を続け、をクリックして選択します。

   ![](assets/image2014-9-22-14-3a3-3a48.png)

   >[!TIP]
   >
   >複数のトークンは、注目の瞬間、タスクの作成、アラートの送信の各フローステップで使用できます。

   >[!NOTE]
   >
   >**関連記事**
   >
   >* [マイトークンの管理](../../../../product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md)
   >* [プログラム内のマイトークンについて](../../../../product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md)


クール！ スマートキャンペーンの実行時に、データがトークンから取得されます。