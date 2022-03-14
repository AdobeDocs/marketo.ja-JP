---
unique-page-id: 2359414
description: シンプルなスコアリング - Marketo ドキュメント - 製品ドキュメント
title: シンプルなスコアリング
exl-id: 6129d46a-e6d2-4819-9b6c-ccbf37060712
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '374'
ht-degree: 100%

---

# シンプルなスコアリング {#simple-scoring}

>[!PREREQUISITES]
>
>* [セットアップと人物の追加](get-set-up-and-add-a-person.md)
>* [フォームを含むランディングページ](landing-page-with-a-form.md)


## 手順 1：スコアリングキャンペーンを作成する {#step-create-a-scoring-campaign}

1. **マーケティングアクティビティ**&#x200B;領域に移動します。

   ![](assets/ma-1.png)

1. 「**学習**」フォルダーを右クリックし、「**新規キャンペーンフォルダー**」をクリックします。

   ![](assets/two-2.png)

1. キャンペーンフォルダーに「スコアリング」と名前を付けます。

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >既に「スコアリング」フォルダーがある場合は、これに別の名前を付けます（例：スコアリング 1）。フォルダー名は一意である必要があります。

1. 次に、新しい「**スコアリング**」フォルダーを右クリックして、「**新規スマートキャンペーン**」を選択します。

   ![](assets/four.png)

1. キャンペーンに「スコアを変更」という&#x200B;**名前を付け**、「**作成**」をクリックします。

   ![](assets/five-1.png)

1. 「**スマートリスト**」タブをクリックします。

   ![](assets/six-1.png)

   **体験版リクエストフォーム**&#x200B;に入力されるたびに、このキャンペーンを実行するようにします。

1. 「**フォームの入力**」トリガーを検索して、左側のキャンバスにドラッグします。

   ![](assets/image2014-9-24-11-3a43-3a35.png)

1. 「**マイフォーム**」を選択します。

   >[!NOTE]
   >
   >[フォームを含むランディングページ](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)クイックウィンを完了している場合、このフォームがあります。フォームに別の名前を使用した場合は、その名前を選択します。

   ![](assets/image2014-9-24-11-3a44-3a16.png)

1. 「**フロー**」タブをクリックします。

   ![](assets/image2014-9-24-11-3a44-3a33.png)

1. 「**スコアを変更**」フローアクションを左のキャンバスにドラッグします。

   ![](assets/image2014-9-24-11-3a44-3a45.png)

1. 人物のスコアに追加する値を入力できます。「+5」を「**変更**」フィールドに入力します。

   ![](assets/eleven-1.png)

   >[!TIP]
   >
   >良いスコアリングキャンペーンは、高品質の人物をセールスに届けるうえで重要です。[**リードスコアリングの最終的なガイド**](https://www.marketo.com/definitive-guides/lead-scoring/)を参照してください。

1. 「**スケジュール**」タブをクリックし、「**アクティブ化**」ボタンをクリックします。

   ![](assets/twelve-1.png)

1. 確認画面の「**アクティブ化**」をクリックします。

   ![](assets/thirteen-1.png)

>[!NOTE]
>
>アクティブにすると、ユーザーがフォームに入力するたびにこのキャンペーンが実行されます。キャンペーンは、無効にされるまで実行を続けます。

## 手順 2:フォームを入力する {#step-fill-out-the-form}

1. [フォームを含むランディングページ](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)クイックウィンで作成したランディングページを選択します。

   ![](assets/fourteen-1.png)

1. 「**承認済みページを表示**」をクリックします。ランディングページが新しいタブで開きます。

   ![](assets/image2014-9-24-11-3a47-3a51.png)

1. 氏名、メールアドレスを使用してフォームに入力し、「**送信**」をクリックします。

   ![](assets/image2014-9-24-11-3a47-3a59.png)

   >[!NOTE]
   >
   >「+5」スコア増加を適用するために、最初に入力したときに使用したものと同じ名前とメールアドレスを使用します。

## 手順 3：人物情報の表示 {#step-view-the-person-info}

1. データベース領域に移動します。

   ![](assets/db-2.png)

1. フォームの入力時に使用したメールアドレスを検索します。

   ![](assets/eighteen.png)

1. 該当する人物をダブルクリックします。

   ![](assets/nineteen.png)

人物の詳細が新しいタブまたはウィンドウで開きます。フォームを入力したことで、スコアが 5 ポイント増加したことを確認できましたか？

![](assets/twenty.png)

**これで完了です。** スコアリングキャンペーンを作成しました。
[◄ ミッション 2：フォームを含むランディングページ](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)

[ミッション 4：メールの自動応答 ►](/help/marketo/getting-started/quick-wins/email-auto-response.md)
