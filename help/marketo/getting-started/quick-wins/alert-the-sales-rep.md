---
unique-page-id: 2359424
description: 販売担当者に警告 — Marketto Docs — 製品ドキュメント
title: 販売担当者に警告する
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 0%

---


# セールス担当者に警告{#alert-the-sales-rep}

## ミッション：訪問者がWebサイトのフォームに入力したときに販売担当者に警告する{#mission-alert-the-sales-rep-when-a-person-fills-out-a-form-on-your-web-site}

セールス担当者にアラート電子メールを自動的に送信するには、アラート電子メールと電子メールキャンペーンが必要です。 その方法を次に示します。

>[!PREREQUISITES]
>
>[フォームとのランディングページ](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)

## 手順1:アラート電子メールの作成{#step-create-an-alert-email}

1. **マーケティングアクティビティ**&#x200B;エリアに移動します。

   ![](assets/one-5.png)

1. **ランディングページーで作成したマイプログラム**&#x200B;をフォーム[のクイックウィンドウで選択し、](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)新規&#x200B;**の下の「**&#x200B;新しいローカルアセット&#x200B;**」をクリックします。**

   ![](assets/two-6.png)

1. 「**電子メール**」をクリックします。

   ![](assets/three-5.png)

1. **電子メールの** 名前「My Email Alert」を指定し、テンプレートを選択して「 **Create**」をクリックします。

   ![](assets/four-4.png)

1. 営業チームに表示する&#x200B;**差出人**、**電子メール**&#x200B;から、**返信**、**件名**&#x200B;を入力します。

   ![](assets/five-5.png)

1. 重複キーを押しながらクリックして、電子メールのテキストを編集します。

   ![](assets/six-5.png)

1. 電子メールの内容を入力します。

   ![](assets/seven-6.png)

1. ユーザーの連絡先情報を挿入する場所にカーソルを置き、**トークンを挿入**&#x200B;アイコンをクリックします。

   ![](assets/eight-4.png)

1. `{{SP_Send_Alert_Info}}` **トークン**&#x200B;を探して選択し、**挿入**&#x200B;をクリックします。

   ![](assets/image2014-9-24-13-3a10-3a0.png)

   >[!NOTE]
   >
   >{{SP_Send_Alert_Info}}は、アラート電子メール用の特別なトークンです。 詳しくは、[「アラート情報トークンの送信](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md)」を参照してください。

1. 「**保存**」をクリックします。

   ![](assets/ten-5.png)

1. 「電子メールエディタ」タブまたはウィンドウを閉じます。

   ![](assets/eleven-5.png)

1. 「**電子メールアクション**」で、「**承認**」をクリックします。

   ![](assets/twelve-4.png)

## 手順2:アラートトリガーキャンペーンの作成{#step-create-an-alert-trigger-campaign}

1. 「**以前に作成したプログラム**」を選択し、「**新しい**」で「**新しいスマートキャンペーン**」をクリックします。

   ![](assets/image2014-9-24-13-3a14-3a17.png)

1. **「アラートキャンペーン」** というキャンペーン名を付け、「 **作成**」をクリックします。

   ![](assets/image2014-9-24-13-3a14-3a28.png)

1. 「**スマートリスト**」タブで、**Fills Out Form**&#x200B;トリガーを探し、キャンバスにドラッグします。

   ![](assets/image2014-9-24-13-3a14-3a43.png)

1. 前に作成したフォームを選択します。

   ![](assets/image2014-9-24-13-3a14-3a58.png)

1. 「**フロー**」タブで、**警告**&#x200B;の送信フローアクションを探し、キャンバスにドラッグします。

   ![](assets/image2014-9-24-13-3a15-3a10.png)

1. **作成済みの警告メール**&#x200B;を選択し、**送信先**&#x200B;は&#x200B;**販売所有者**&#x200B;のままにします。

   ![](assets/eighteen-1.png)

1. [**その他の電子メール**&#x200B;へ]フィールドに電子メールアドレスを入力します。

   ![](assets/nineteen-2.png)

1. 「**スケジュール**」タブに移動し、「**アクティブ化**」ボタンをクリックします。

   ![](assets/twenty-2.png)

   >[!TIP]
   >
   >**クオリフィケーションルール**&#x200B;を&#x200B;**毎回**&#x200B;に設定し(スマートキャンペーンを編集)、同じ人が複数回アラートをトリガーできるようにします。

1. 確認画面で「**アクティブ化**」をクリックします。

   ![](assets/twenty-one-1.png)

## 手順3:試してみろ！{#step-test-it-out}

1. ランディングページを選択し、**表示が承認したページ**&#x200B;をクリックします。

   ![](assets/image2014-9-24-13-3a17-3a8.png)

   >[!NOTE]
   >
   >ランディングページを認めるのを忘れないで。彼らは承認されるまで生きていかない。

1. フォームに入力し、「**送信**」をクリックします。

   ![](assets/image2014-9-24-13-3a17-3a41.png)

1. まもなくメールを受け取るはずです。 すべて正常に動作することを確認したら、アラートの送信フローから電子メールアドレスを削除します（上記の手順2.7を参照）。

   >[!NOTE]
   >
   >連絡先情報を表示するには、マーケティングの「**人物情報**」タブをクリックします。

## ミッション完了！{#mission-complete}

<br> 

[etchaミッション7:電子メールのパーソナライズ](personalize-an-email.md)

[ミッション9:リードデータの更新…](update-person-data.md)
