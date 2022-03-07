---
description: ダイアログ - Marketo ドキュメント - 製品ドキュメント
title: ダイアログ
exl-id: 5ec17ad0-6d56-4c06-a6ac-4c5771b2d91d
source-git-commit: 8aaa6f5225f7965228c3472c0cf6beb2259f3642
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# ダイアログ {#dialogues}

ダイアログは個々のチャットの会話です。視覚的にカスタマイズする方法、表示するページを決定する方法、表示するページを決定する方法、言い回しと表示するユーザーを決定する方法を説明します。

## ダイアログの新規作成 {#create-a-new-dialogue}

1. 「**ダイアログ**」をクリックします。

   ![](assets/dialogues-1.png)

1. 「**新規作成**」ボタンをクリックします。

   ![](assets/dialogues-2.png)

1. 名前を入力して（説明はオプション）優先度レベルを設定し、「**保存**」をクリックします。

   ![](assets/dialogues-3.png)

>[!NOTE]
>
>優先度は、訪問者が複数のダイアログに同時に振り分けた場合に、どのダイアログを訪問者に表示するかを決定します。

## オーディエンス条件 {#audience-criteria}

Marketo スマートリストと同様に、オーディエンス条件属性を使用すると、ターゲットオーディエンスを定義できます。推測される人、人、会社の属性（またはその組み合わせ）を使用して、既知の人または不明な人をターゲットに設定できます。

**認識済み担当者**

_多数の_&#x200B;属性の組み合わせから選択できます。この例では、50 人以上の従業員を持つ会社で働くカリフォルニア州のすべての&#x200B;**認識済みユーザー**&#x200B;をターゲットにしています。

1. **Person State** 属性を選択し、右にドラッグします。

   ![](assets/dialogues-4.png)

1. _Is_ はデフォルトで設定されています。「値を選択」フィールドに「CA」と入力します（ドロップダウンをクリックして、リストから選択することもできます）。

   ![](assets/dialogues-5.png)

1. **Company Size** 属性を選択し、_ここに属性をドラッグ＆ドロップ_&#x200B;と書かれた場所にドラッグします。

   ![](assets/dialogues-6.png)

   >[!NOTE]
   >
   >属性の **+** アイコンをクリックして選択することもできます。

1. 演算子のドロップダウンをクリックし、「**Greater Than**」を選択します。 

   ![](assets/dialogues-7.png)

1. 「50」と入力し、画面の別の場所をクリックして保存します。

   ![](assets/dialogues-8.png)

これで完了です。

**匿名担当者**

まだデータベース内にいない人を特定してターゲット設定するのは簡単です。この例では、ニューヨーク地区にいるすべての&#x200B;**匿名ユーザー**&#x200B;をターゲットに設定しています。

1. **Person Email** 属性を選択し、右にドラッグします。

   ![](assets/dialogues-9.png)

1. 演算子のドロップダウンをクリックし、「**Is Empty**」を選択します。

   ![](assets/dialogues-10.png)

1. **Inferred State** 属性を選択し、_ここに属性をドラッグ＆ドロップ_&#x200B;と書かれた場所にドラッグします。 

   ![](assets/dialogues-11.png)

   >[!NOTE]
   >
   >ユーザーが Web サイトが訪問すると、[Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) cookie が作成されてシステムに格納されます。IP は特別なデータベースで調べられ、あらゆる情報が推測されます。

1. _Is_ はデフォルトで設定されています。「値を選択」フィールドに「NY」と入力します（ドロップダウンをクリックして、リストから選択することもできます）。

   ![](assets/dialogues-12.png)

## グループを追加 {#add-groups}

すべての特定の属性を別の属性の「すべてまたは任意」と共に持つ場合に備えて、属性をグループ化することもできます。複数のグループを追加できます。

![](assets/dialogues-13.png)

![](assets/dialogues-14.png)

## ターゲット {#target}

特定のダイアログを表示する URL を入力する場所です。

使用可能な形式：

* `http://website.com`
* `https://*.website.com`
* `http://website.com/folder/*`
* `https://*.website.com/folder/*`

>[!NOTE]
>
>アスタリスクを使用すると包括的なワイルドカードとして機能します。`https://*.website.com` はサブドメイン（例：`support.website.com`）を含み、ダイアログをサイトのすべてのページに配置します。また、`https://website.com/folder/*` は後続のフォルダー内のすべての HTML ページにダイアログを配置します（例：フォルダーが「sports」の場合、website.com/sports/baseball.html、website.com/sports/football.html などになります）。

## ストリームデザイナー {#stream-designer}

ストリームデザイナーには、チャット会話を形成するために追加できる様々なカードが含まれています。

<table>
 <tr>
  <td><strong>メッセージ</strong></td>
  <td>応答を必要としない文を作成する場合に使用します（例：「こんにちは。コード「SAVE25」を使用すると、今日は全品が 25% オフです）。
</td>
 </tr>
 <tr>
  <td><strong>質問</strong></td>
  <td>複数選択の質問に対して、利用可能な回答を提供する場合に使用します（例：どのような車に興味がありますか？応答 = SUV、コンパクト、トラックなど）。</td>
 </tr>
 <tr>
  <td><strong>情報取得</strong></td>
  <td>情報を収集する場合に使用します。選択できる 3 つのフィールドは、「電子メールアドレス」、「電話番号」、「テキスト」（訪問者が独自のメッセージを書き込むことができる）です。</td>
 </tr>
 <tr>
  <td><strong>予定スケジューラー</strong></td>
  <td>訪問者に、フォローアップをスケジュールするために使用可能な日付のカレンダーを提供します。カレンダーの可用性は<a href="/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md#routing">次のエージェント</a>を反映します。</td>
 </tr>
 <tr>
  <td><strong>ゴール</strong></td>
  <td>訪問者に表示されないカードはこれだけです。特定のチャット内で目標を達成した時点を決定する必要があります（例：訪問者のメールを収集することが目標の場合は、ストリームの情報キャプチャの直後に目標カードを配置します）。</td>
 </tr>
</table>

**ストリームの作成**

_多数の_&#x200B;可能なストリームの組み合わせがあります。[この記事で](/help/marketo/product-docs/demand-generation/dynamic-chat/create-a-stream.md)例を見てみましょう。

## レポート {#reports}

「レポート」タブでは、過去 90 日間のデータを確認できます。各カテゴリは以下で定義します。

<table>
 <tr>
  <td><strong>トリガーされた合計</strong></td>
  <td>訪問者がダイアログに資格を与えるたびに、または表示されるたびに増分されます。
</td>
 </tr>
 <tr>
  <td><strong>エンゲージ済</strong></td>
  <td>訪問者がチャットボットのアンカーをクリックしてダイアログを開くたびに増分します。</td>
 </tr>
 <tr>
  <td><strong>完了</strong></td>
  <td>訪問者がダイアログのブランチの終わりに達するたびに増分されます。</td>
 </tr>
 <tr>
  <td><strong>キャプチャ済みユーザー</strong></td>
  <td>訪問者がダイアログフローで有効な電子メールアドレスを指定するたびに増分されます。</td>
 </tr>
 <tr>
  <td><strong>予約済みの会議</strong></td>
  <td>訪問者がチャットボット経由で予定のスケジュールを正常に設定するたびに増分します。</td>
 </tr>
 <tr>
  <td><strong>達した目標</strong></td>
  <td>訪問者がダイアログフローの目標に達するたびに増分します。</td>
 </tr>
</table>

>[!MORELIKETHIS]
>
>[ストリームの作成](/help/marketo/product-docs/demand-generation/dynamic-chat/create-a-stream.md)
