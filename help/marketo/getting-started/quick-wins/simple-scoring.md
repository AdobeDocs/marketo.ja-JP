---
unique-page-id: 2359414
description: シンプルスコアリング — Marketto Docs — 製品ドキュメント
title: 単純スコア
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 0%

---


# 単純スコア {#simple-scoring}

>[!PREREQUISITES]
>
>* [設定と追加人](get-set-up-and-add-a-person.md)
>* [フォームとのランディングページ](landing-page-with-a-form.md)


## 手順1:スコアリングキャンペーンの作成 {#step-create-a-scoring-campaign}

1. 「 **マーケティングアクティビティ** 」領域に移動します。

   ![](assets/ma-1.png)

1. [ **学習** ]フォルダを右クリックし、[ **新規キャンペーンフォルダ**]をクリックします。

   ![](assets/two-2.png)

1. キャンペーンフォルダーに「スコアリング」という名前を付けます。

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >既にスコアリングフォルダーがある場合は、このフォルダーに別の名前を付けます（スコアリング1など）。 フォルダー名は一意にする必要があります。

1. 次に、新しい **スコアリングキャンペーンーを右クリックし、「** 新しいスマートフォルダー ****」を選択します。

   ![](assets/four.png)

1. **キャンペーンに** 「スコアを変更」という名前を付け、「 **作成**」をクリックします。

   ![](assets/five-1.png)

1. 「 **スマートリスト** 」タブをクリックします。

   ![](assets/six-1.png)

   お客様が **体験版請求フォームに記入するたびに、このキャンペーンを実行してもらいたいと考えています**。

1. 「 **Fills Out Form** 」トリガーを探し、左のカンバスにドラッグします。

   ![](assets/image2014-9-24-11-3a43-3a35.png)

1. 「 **マイフォーム**」を選択します。

   >[!NOTE]
   >
   >フォームのクイックウィンドウで [ランディングページを完了した場合は](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md) 、フォームが必要です。 フォームに別の名前を使用した場合は、その名前を選択します。

   ![](assets/image2014-9-24-11-3a44-3a16.png)

1. 「 **フロー** 」タブをクリックします。

   ![](assets/image2014-9-24-11-3a44-3a33.png)

1. 「スコア **の** 変更」フローアクションを左のキャンバスにドラッグします。

   ![](assets/image2014-9-24-11-3a44-3a45.png)

1. ユーザーのスコアに追加する値を入力できます。 「 **変更** 」フィールドに「+5」と入力します。

   ![](assets/eleven-1.png)

   >[!TIP]
   >
   >良いスコアキャンペーンは、高品質の人をセールスに送るための重要な要素です。 リードスコア [**の最終的なガイドを読み**](https://www.marketo.com/definitive-guides/lead-scoring/)ます。

1. 「 **スケジュール** 」タブをクリックし、「 **アクティブ化** 」ボタンをクリックします。

   ![](assets/twelve-1.png)

1. 確認画面で「 **アクティブ化** 」をクリックします。

   ![](assets/thirteen-1.png)

>[!NOTE]
>
>アクティブにすると、ユーザーがフォームに入力するたびに、このキャンペーンが実行されます。 キャンペーンは、非アクティブ化されるまで実行を続けます。

## 手順2:フォームの入力 {#step-fill-out-the-form}

1. フォーム [のクイックウィンドウが表示された](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md) ランディングページで作成したランディングページを選択します。

   ![](assets/fourteen-1.png)

1. 「 **表示が承認したページ**」をクリックします。 ランディングページが新しいタブで開きます。

   ![](assets/image2014-9-24-11-3a47-3a51.png)

1. 名、姓、電子メールアドレスをフォームに入力し、「 **送信**」をクリックします。

   ![](assets/image2014-9-24-11-3a47-3a59.png)

   >[!NOTE]
   >
   >「+5」スコアの増加を適用するために、自分を最初に個人として入力したときと同じ名前と電子メールアドレスを使用します。

## 手順3:個人情報の表示 {#step-view-the-person-info}

1. 「Database」領域に移動します。

   ![](assets/db-2.png)

1. フォームの入力時に使用した電子メールアドレスを検索します。

   ![](assets/eighteen.png)

1. 重複を押しながら、自分の人をクリックします。

   ![](assets/nineteen.png)

ユーザーの詳細が新しいタブまたはウィンドウで開きます。 フォームの入力に対するスコアが5ポイント上昇した様子をご覧ください。

![](assets/twenty.png)

**おめでとう！** スコアリングキャンペーンを作成しました。
[エスケアミッション2:フォームとのランディングページ](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)

[ミッション4:電子メールの自動応答ï¿](/help/marketo/getting-started/quick-wins/email-auto-response.md)
