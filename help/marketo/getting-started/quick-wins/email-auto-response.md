---
unique-page-id: 2359416
description: 電子メールの自動応答 — Marketto Docs — 製品ドキュメント
title: 電子メールの自動応答
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---


# 電子メールの自動応答 {#email-auto-response}

## ミッション：ユーザーがフォームに記入する際に、お礼の電子メールを送信する {#mission-send-out-a-thank-you-email-when-a-person-fills-out-a-form}

>[!PREREQUISITES]
>
>* [設定と追加人](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md)
>* [フォームとのランディングページ](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)


## 手順1:電子メールの作成 {#step-create-an-email}

1. 「マーケティングアクティビティ」領域に移動します。

   ![](assets/one-2.png)

1. 左のメニューで「マイプログラム」を選択し、「新規」ドロップダウンをクリックして、「新規ローカルアセット」を選択します。

   ![](assets/two-3.png)

1. 「電子メール」をクリックします。

   ![](assets/three-2.png)

1. 電子メールに「Auto Response Email」という名前を付け、テンプレートを選択し、「Create」をクリックします。

   ![](assets/four-1.png)

   電子メールエディターが新しいウィンドウまたはタブで開きます。 ポップアップがブロックされている場合は、アセット概要ページの「ドラフトを **編集** 」をクリックして電子メールにアクセスします。

1. 件名を入力し、重複キーを押しながら電子メールの編集可能な領域をクリックします。

   ![](assets/five-2.png)

   _電子メールエディターの上部にリッチテキストエディターが開きます。_

1. 既存の電子メールコンテンツを強調表示します。

   ![](assets/six-2.png)

1. 電子メールの内容を入力し、「保存」をクリックします。

   ![](assets/seven-2.png)

1. 変更が自動保存されます。 「電子メールエディタ」タブまたはウィンドウを閉じます。

   ![](assets/eight-1.png)

1. 新しい電子メールを選択します。 「電子メールアクション」で、「承認」をクリックします。

   ![](assets/image2014-9-24-11-3a55-3a16.png)

## 手順2:スマートキャンペーンの作成 {#step-create-a-smart-campaign}

1. 「 **マイプログラム** 」を右クリックし、「 **新規スマートキャンペーン**」をクリックします。

   ![](assets/image2014-9-24-11-3a56-3a13.png)

1. **スマートキャンペーンに** 「自動応答キャンペーン」という名前を付け、「 **作成**」をクリックします。

   ![](assets/image2014-9-24-11-3a56-3a25.png)

1. 「 **スマートリスト** 」タブに移動します。

   ![](assets/image2014-9-24-11-3a56-3a38.png)

   このキャンペーンは、 [**ランディングページで作成したフォームにフォームを入力するたびに実行されるように設定しています**](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)。

1. 「 **Fills Out Form** 」トリガーを探し、左のカンバスにドラッグします。

   ![](assets/image2014-9-24-11-3a57-3a18.png)

1. ドロップダウン **から** 「マイフォーム」を選択します。 「 **フロー** 」タブをクリックします。

   ![](assets/image2014-9-24-11-3a57-3a29.png)

1. 「 **電子メールの** 送信」フローアクションを左のキャンバスにドラッグします。

   ![](assets/image2014-9-24-11-3a57-3a41.png)

1. 「 **自動応答電子メール** 」を選択し、「 **スケジュール** 」タブに移動します。

   ![](assets/image2014-9-24-11-3a57-3a53.png)

1. 「 **編集**」をクリックします。

   ![](assets/8.png)

1. [ **毎回]を選択し** 、[ **保存**]をクリックします。

   ![](assets/9.png)

1. 「 **アクティブ化**」をクリックします。

   ![](assets/10.png)

1. 確認画面で「 **アクティブ化** 」をクリックします。

   ![](assets/11.png)

>[!NOTE]
>
>アクティブにすると、指定したフォームにユーザーが入力するたびに、このキャンペーンが実行されます。 キャンペーンは、非アクティブ化されるまで実行を続けます。

## 手順3:フォームの入力 {#step-fill-out-the-form}

1. 「 **マイページ**」を選択します。 これは、 [ランディングページでForm](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md) Quick Winと共に作成されました。

   ![](assets/image2014-9-24-12-3a0-3a8.png)

1. 「 **表示が承認したページ**」をクリックします。

   ![](assets/image2014-9-24-12-3a0-3a18.png)

   「無償体験版」ランディングページが新しいタブに開きます。

1. 名、姓、電子メールアドレスをフォームに入力し、「 **送信**」をクリックします。

   ![](assets/image2014-9-24-12-3a0-3a28.png)

>[!NOTE]
>
>電子メールを取得できるように、実際の電子メールアドレスを使用してください。

## ミッション完了 {#mission-complete}

数分以内に、受信トレイに自動応答の電子メールが表示されます。 素晴らしい仕事！

<br> 

[エスケアミッション3:単純スコア](/help/marketo/getting-started/quick-wins/simple-scoring.md)

[ミッション5:リードのリストのインポート…](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md)
