---
unique-page-id: 2359416
description: メールの自動応答 - Marketo ドキュメント - 製品ドキュメント
title: メールの自動応答
exl-id: c9c0a154-65ec-4845-97a0-a2100223cb13
source-git-commit: 0da33dfa840dd1e5a5618fcd762b482f7a2e0789
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 86%

---

# メールの自動応答 {#email-auto-response}

## ミッション：フォームに入力されたときにお礼メールを送信する {#mission-send-out-a-thank-you-email-when-a-person-fills-out-a-form}

>[!PREREQUISITES]
>
>* [セットアップと人物の追加](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target=&quot;_blank&quot;}
>* [フォームを含むランディングページ](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;}


## 手順 1：メールを作成する {#step-create-an-email}

1. マーケティングアクティビティ領域に移動します。

   ![](assets/one-2.png)

1. 左側のメニューで「マイプログラム」を選択し、「新規」ドロップダウンをクリックして、「新規ローカルアセット」を選択します。

   ![](assets/two-3.png)

1. 「メール」をクリックします。

   ![](assets/three-2.png)

1. メールに「自動応答メール」という名前を付け、テンプレートを選択し、「作成」をクリックします。

   ![](assets/four-1.png)

   新しいウィンドウまたはタブでメールエディターが開きます。ポップアップがブロックされている場合は、アセットの概要ページの「**下書きの編集**」をクリックして、メールにアクセスします。

1. 件名を入力し、メールの編集可能な領域をダブルクリックします。

   ![](assets/five-2.png)

   _リッチテキストエディターが、メールエディターの上に開きます。_

1. 既存のメールコンテンツをハイライトします。

   ![](assets/six-2.png)

1. メールの内容を入力し、「保存」をクリックします。

   ![](assets/seven-2.png)

1. 変更内容は自動保存されます。「メールエディター」タブ／ウィンドウを閉じます。

   ![](assets/eight-1.png)

1. 新規メールを選択します。「メールアクション」で「承認」をクリックします。

   ![](assets/image2014-9-24-11-3a55-3a16.png)

## 手順 2：アラースマートキャンペーンを作成する {#step-create-a-smart-campaign}

1. 「**マイプログラム**」を右クリックし、「**新規スマートキャンペーン**」をクリックします。

   ![](assets/image2014-9-24-11-3a56-3a13.png)

1. スマートキャンペーンに「自動応答キャンペーン」という&#x200B;**名前を付け**、「**作成**」をクリックします。

   ![](assets/image2014-9-24-11-3a56-3a25.png)

1. 「**スマートリスト**」タブに移動します。

   ![](assets/image2014-9-24-11-3a56-3a38.png)

   担当者が作成したフォームに入力するたびにこのキャンペーンを実行するように設定しています。 [**フォームを含むランディングページ**](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;}。

1. 「**フォームの入力**」トリガーを検索して、左側のキャンバスにドラッグします。

   ![](assets/image2014-9-24-11-3a57-3a18.png)

1. ドロップダウンから「**マイフォーム**」を選択します。「**フロー**」タブをクリックします。

   ![](assets/image2014-9-24-11-3a57-3a29.png)

1. 「**メールを送信**」フローアクションを左のキャンバスにドラッグします。

   ![](assets/image2014-9-24-11-3a57-3a41.png)

1. 「**自動応答メール**」を選択し、「**スケジュール**」タブをクリックします。

   ![](assets/image2014-9-24-11-3a57-3a53.png)

1. 「**編集**」をクリックします。

   ![](assets/8.png)

1. 「**毎回**」を選択して、「**保存**」をクリックします。

   ![](assets/9.png)

1. 「**アクティブ化**」をクリックします。

   ![](assets/10.png)

1. 確認画面の「**アクティブ化**」をクリックします。

   ![](assets/11.png)

>[!NOTE]
>
>アクティブにすると、指定したフォームに入力されるたびに、このキャンペーンが実行されます。キャンペーンは、無効にされるまで実行を続けます。

## 手順 3:フォームを入力する {#step-fill-out-the-form}

1. 「**マイページ**」を選択します。これは、 [フォームを含むランディングページ](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;} クイックウィンドウ。

   ![](assets/image2014-9-24-12-3a0-3a8.png)

1. 「**承認済みページを表示**」をクリックします。

   ![](assets/image2014-9-24-12-3a0-3a18.png)

   「無料体験版」ランディングページが新しいタブで開きます。

1. 氏名、メールアドレスを使用してフォームに入力し、「**送信**」をクリックします。

   ![](assets/image2014-9-24-12-3a0-3a28.png)

>[!NOTE]
>
>メールを受信するには、実際のメールアドレスを使用してください。

## ミッション完了 {#mission-complete}

数分以内に、インボックスに自動応答のメールが表示されます。これで完了です。

<br> 

[◄ ミッション 3：単純スコア](/help/marketo/getting-started/quick-wins/simple-scoring.md)

[ミッション 5:人物のリストをインポート►](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md)
