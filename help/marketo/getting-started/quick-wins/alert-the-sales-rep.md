---
unique-page-id: 2359424
description: セールス担当者にアラート - Marketo ドキュメント - 製品ドキュメント
title: セールス担当者にアラート
exl-id: 4ad7d7b8-ee1e-4605-b4e0-e72a7e573c05
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '401'
ht-degree: 100%

---

# セールス担当者にアラート {#alert-the-sales-rep}

## ミッション：人物が web サイトのフォームに入力したときにセールス担当者にアラートする {#mission-alert-the-sales-rep-when-a-person-fills-out-a-form-on-your-web-site}

セールス担当者にアラートメールを自動的に送信するには、アラートメールとメールキャンペーンが必要です。その方法を説明しましょう。

>[!PREREQUISITES]
>
>[フォームを含むランディングページ](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)

## 手順 1：アラートメールを作成する {#step-create-an-alert-email}

1. **マーケティングアクティビティ**&#x200B;領域に移動します。

   ![](assets/one-5.png)

1. クイックウィン&#x200B;**フォームを含むランディングページ**&#x200B;に作成した[マイプログラム](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)を選択、次に「**新規**」で、「**新規ローカルアセット**」をクリックします。

   ![](assets/two-6.png)

1. 「**メール**」をクリックします。

   ![](assets/three-5.png)

1. メールに「マイメールアラート」という&#x200B;**名前を付け**、テンプレートを選択し、「**作成**」をクリックします。

   ![](assets/four-4.png)

1. セールスチームが確認できるように、「**送信者名**」、「**送信元メール**」、「**返信先**」、「**件名**」を入力します。

   ![](assets/five-5.png)

1. ダブルクリックしてメールのテキストを編集します。

   ![](assets/six-5.png)

1. メールの内容を入力します。

   ![](assets/seven-6.png)

1. 人物の連絡先情報を挿入する場所にカーソルを置き、「**トークンの挿入**」アイコンをクリックします。

   ![](assets/eight-4.png)

1. `{{SP_Send_Alert_Info}}` **トークン**&#x200B;を検索して選択し、「**挿入**」をクリックします。

   ![](assets/image2014-9-24-13-3a10-3a0.png)

   >[!NOTE]
   >
   >{{SP_Send_Alert_Info}} は、アラートメール用の特別なトークンです。詳しくは、[アラート情報トークンの送信の使用](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md)を参照してください。

1. 「**保存**」をクリックします。

   ![](assets/ten-5.png)

1. 「メールエディター」タブ／ウィンドウを閉じます。

   ![](assets/eleven-5.png)

1. 「**メールアクション**」で「**承認**」をクリックします。

   ![](assets/twelve-4.png)

## 手順 2：アラートトリガーキャンペーンを作成する {#step-create-an-alert-trigger-campaign}

1. 以前に作成した「**マイプログラム**」を選択し、「**新規**」で、「**新規スマートキャンペーン**」をクリックします。

   ![](assets/image2014-9-24-13-3a14-3a17.png)

1. キャンペーンに「マイアラートキャンペーン」という&#x200B;**名前を付け**、「**作成**」をクリックします。

   ![](assets/image2014-9-24-13-3a14-3a28.png)

1. 「**スマートリスト**」タブで、「**フォームの入力**」トリガーを検索して、キャンバスにドラッグします。

   ![](assets/image2014-9-24-13-3a14-3a43.png)

1. 先ほど作成したフォームを選択します。

   ![](assets/image2014-9-24-13-3a14-3a58.png)

1. 「**フロー**」タブで、「**アラートを送信**」フローアクションを検索してキャンバスにドラッグします。

   ![](assets/image2014-9-24-13-3a15-3a10.png)

1. 先ほど作成した「**マイアラートメール**」を選択し、「**送信先**」を「**営業所有者**」とします。

   ![](assets/eighteen-1.png)

1. 自分のメールアドレスを「**他のメールへ**」フィールドに入力します。

   ![](assets/nineteen-2.png)

1. 「**スケジュール**」タブに移動し、「**アクティブ化**」ボタンをクリックします。

   ![](assets/twenty-2.png)

   >[!TIP]
   >
   >「**クオリフィケーションルール**」を「**毎回**」（スマートキャンペーンを編集する）に設定し、同じ人物が複数回アラートをトリガーできるようにします。

1. 確認画面の「**アクティブ化**」をクリックします。

   ![](assets/twenty-one-1.png)

## 手順 3：テストする {#step-test-it-out}

1. ランディングページを選択し、「**承認済みページを表示**」をクリックします。

   ![](assets/image2014-9-24-13-3a17-3a8.png)

   >[!NOTE]
   >
   >忘れずにランディングページを承認してください。承認されないと本番稼働しません。

1. フォームに入力し、「**送信**」をクリックします。

   ![](assets/image2014-9-24-13-3a17-3a41.png)

1. すぐにメールが届きます。すべて正常に動作することを確認したら、アラート送信フローからメールアドレスを削除します（上記の手順 2.7 を参照）。

   >[!NOTE]
   >
   >Marketo の「**人物情報**」タブをクリックして、連絡先情報を表示します。

## ミッション完了です。 {#mission-complete}

<br>

[◄ ミッション 7：メールのパーソナライズ](personalize-an-email.md)

[ミッション 9：リードデータの更新 ►](update-person-data.md)
