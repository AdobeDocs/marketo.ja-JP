---
unique-page-id: 1900581
description: メール内の「友達に転送」リンク - Marketo ドキュメント - 製品ドキュメント
title: メール内の「友達に転送」リンク
exl-id: 7addac65-4207-419f-845c-d6b2d08d299c
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '703'
ht-degree: 100%

---

# メール内の「友達に転送」リンク {#forward-to-a-friend-link-in-emails}

「友達に転送」リンクをメールに追加すると、このリンクから転送されたメールを受信したリードを追跡し、データベースにまだ存在しない場合は新しいリードとして自動的に追加できます。

例えば、Keith が「友達に転送」リンクを使用して、不明な人物 Mark にメールを転送したとします。Mark は新しいリードとして自動的に追加され、独自の Cookie が割り当てられて、そのメールと web アクティビティのすべてがリンクされます。ただし、Keith がメールクライアントで「転送」ボタンを使用している場合、Mark は誤って Keith として Cookie を取得し、そのアクティビティは Keith のものとして記録されます。

## メールテンプレートへのリンクの追加 {#add-the-link-to-an-email-template}

1. **Design Studio** に移動します。

   ![](assets/one-8.png)

1. リンクを追加するメールテンプレートを見つけて選択します。「**ドラフトを編集**」をクリックします。

   ![](assets/two-7.png)

1. 「友達に転送」リンクを表示する場所に、次の HTML コードを貼り付けます（この部分に関するヘルプが必要な場合は、web デベロッパーにお問い合わせください）。

   `<pre data-theme="Confluence"><a href="{{system.forwardToFriendLink}}">Forward to Friend</a></pre>`

   ![](assets/three-7.png)

   >[!TIP]
   >
   >
   >リンクにスタイルを追加すると、見た目を改善することができます。例：
   >
   >`<a href="{{system.forwardToFriendLink}}" style="font-family:arial, sans-serif; padding:10px; position:absolute; right:0px;">Forward to Friend</a>`

   >[!CAUTION]
   >
   >メールテンプレート内での **position:relative**  スタイル設定の使用はお勧めしません「友達に転送」ボックスの位置と表示に問題が生じる可能性があります。

1. 「**ドラフトをプレビュー**」を使用して、テンプレートが希望どおりに表示されることを確認します。

   ![](assets/four-5.png)

   >[!NOTE]
   >
   >変更を適用するには、忘れずにテンプレートのドラフトを承認してください。

   そのテンプレートを使用するすべてのメールに「友達に転送」リンクが表示されるようになります。メール受信者がクリックすると、「友達に転送」ボックスが付いた web バージョンのメールが届きます。

   ![](assets/f2afbox.png)

## 個々のメールへのリンクの追加 {#add-the-link-to-an-individual-email}

「友達に転送」リンクはメールに直接追加することもできます。

1. リンクを含めるメールを開き、編集可能な領域でダブルクリックします。

   ![](assets/five-4.png)

1. リンクを表示する場所にカーソルを置き、「**トークンを挿入**」ボタンをクリックします。

   ![](assets/six-2.png)

1. **`{{system.forwardToFriendLink}}`** トークンを選択します。

   ![](assets/seven-1.png)

   >[!NOTE]
   >
   >このトークンは、「友達に転送」ボックスが付いたメールの web バージョンの URL です。

1. リンクの表示テキストを書き出します（例：「友達に転送」）。

   ![](assets/seven-1.png)

1. Ctrl + X（Windows）または Command + X（Mac）を使用して **`{{system.forwardToFriendLink}}`** トークンを切り取ります。「友達に転送」をハイライト表示し、「**リンクを挿入／編集**」ボタンをクリックします。

   ![](assets/eight-1.png)

1. Ctrl/Cmd+V キーを使用して **`{{system.forwardToFriendLink}}`** トークンを **URL** ボックスに貼り付け、「**挿入**」をクリックします。

   ![](assets/nine.png)

1. 編集を保存し、新しいリンクをプレビューします。

   ![](assets/ten-1.png)

   >[!NOTE]
   >
   >「友達に転送」のメールを受信して新しく追加されたリードのマーケティングメールへの登録はデフォルトで解除されています。

## 転送アクティビティを表示 {#view-forwarding-activity}

リードのアクティビティログで、誰がメールを転送および受信したかを確認できます。

1. **`Database`** に移動します。

   ![](assets/db.png)

1. アクティビティを表示するリードをダブルクリックします。

   ![](assets/fourteen.png)

1. 「**アクティビティログ**」タブに移動します。「**友達への転送メールを受信**」または「**友達への転送メールを送信**」をダブルクリックして詳細を確認します。

   ![](assets/fifteen.png)

   >[!NOTE]
   >
   >**定義**
   >
   >「友達への転送メールを受信」の場合、「リード ID」はメールを転送したリードです。
   >
   >「友達への転送メールを送信」の場合、「リード ID」はメールを受信したリードです。

   ![](assets/sixteen.png)

1. ID でリードを表示するには、**リード ID** を URL の末尾に追加します（この URL の先頭は、Marketo インスタンスに依存します）。

   `<pre data-theme="Confluence">...marketo.com/Database/loadPersonDetail?personId=</pre>`

   >[!NOTE]
   >
   >**リード ID** をクリック可能にして、今後のパッチのリードに直接リンクします。

   ![](assets/seventeen.png)

   >[!NOTE]
   >
   >転送を受け取った友達が不明なリードの場合、新しいリードが作成され、「友だちに転送」がリードの&#x200B;**ソース**に指定されます。
   >メールがプログラムのローカルアセットである場合、プログラムはリードの&#x200B;**獲得プログラム**&#x200B;に指定されます。

## トリガーまたは転送アクティビティを使用したフィルター {#trigger-or-filter-using-forwarding-activity}

「友達に転送」アクティビティを送受信し、フローアクションをトリガーしたり、「友達に転送」アクティビティで顧客をフィルタリングするのに使用できるトリガー／フィルターは 6 つあります。

スマートキャンペーンのスマートリストで「転送」を検索すると、使用可能なトリガーとフィルターが表示されます。

![](assets/nineteen.png)

## 友達に転送のテスト {#test-forward-to-friend}

「友達に転送」をテストするには、自分に転送リンクを含むメールを送信します。必ず、**メールを送信**&#x200B;フローステップで送信してください。**テストメールを送信**&#x200B;は&#x200B;*使用しない*&#x200B;でください。
