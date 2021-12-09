---
description: ダイアログ — Marketoドキュメント — 製品ドキュメント
title: ダイアログ
hide: true
hidefromtoc: true
exl-id: 5ec17ad0-6d56-4c06-a6ac-4c5771b2d91d
source-git-commit: fda1bf51d4016a61c41be9acba4771db1797a552
workflow-type: tm+mt
source-wordcount: '745'
ht-degree: 1%

---

# ダイアログ {#dialogues}

ダイアログは個々のチャットの会話です。 視覚的にカスタマイズする方法、表示するページを決定する方法、表示するページを決定する方法、言い回しと表示するユーザーを決定する方法を説明します。

## 新しいダイアログを作成 {#create-a-new-dialogue}

1. クリック **ダイアログ**.

   ![](assets/dialogues-1.png)

1. 次をクリック： **新規作成** 」ボタンをクリックします。

   ![](assets/dialogues-2.png)

1. 名前を入力し（説明はオプション）、優先度レベルを設定し、 **保存**.

   ![](assets/dialogues-3.png)

>[!NOTE]
>
>優先度は、訪問者が複数のダイアログに同時に振り分けた場合に、どのダイアログを訪問者に表示するかを決定します。

## オーディエンス条件 {#audience-criteria}

Marketoスマートリストと同様に、オーディエンス条件属性を使用すると、ターゲットオーディエンスを定義できます。 推測される人、人、会社の属性（またはその組み合わせ）を使用して、既知の人または不明な人をターゲットに設定できます。

**認識済み担当者**

次のものがあります。 _多数の_ 属性の組み合わせから選択します。 この例では、すべてをターゲットにしています **既知の担当者** 50 人以上の従業員を持つ会社で働くカリフォルニア州。

1. を取得 **担当者の州** 属性を選択し、右にドラッグします。

   ![](assets/dialogues-4.png)

1. _次に該当_ はデフォルトで設定されています。 「値の選択」フィールドに「 CA 」と入力します（ドロップダウンをクリックして、リストから「 」を選択することもできます）。

   ![](assets/dialogues-5.png)

1. を取得 **会社規模** 属性を指定し、指定された場所にドラッグします。 _ここに属性をドラッグ&amp;ドロップ_.

   ![](assets/dialogues-6.png)

   >[!NOTE]
   >
   >属性を選択するには、 **+** アイコン

1. 演算子のドロップダウンをクリックし、「 」を選択します。 **より大きい**.

   ![](assets/dialogues-7.png)

1. 「 50 」と入力し、画面の別の場所をクリックして保存します。

   ![](assets/dialogues-8.png)

これで完了です。

**匿名担当者**

まだデータベース内にいない人を特定してターゲット設定するのは簡単です。 この例では、すべてをターゲットに設定しています **匿名の人** ニューヨーク地区に位置する

1. を取得 **担当者のメール** 属性を選択し、右にドラッグします。

   ![](assets/dialogues-9.png)

1. 演算子のドロップダウンをクリックし、「 」を選択します。 **空である**.

   ![](assets/dialogues-10.png)

1. を取得 **推測される状態** 属性を指定し、指定された場所にドラッグします。 _ここに属性をドラッグ&amp;ドロップ_.

   ![](assets/dialogues-11.png)

   >[!NOTE]
   >
   >誰かが Web サイトを訪問したとき、 [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) cookie を作成し、システムに格納します。 私たちは彼らの IP を特別なデータベースで調べ、あらゆる良い情報を推測します。

1. _次に該当_ はデフォルトで設定されています。 「値の選択」フィールドに「 NY 」と入力します（ドロップダウンをクリックして、リストからを選択することもできます）。

   ![](assets/dialogues-12.png)

## グループを追加 {#add-groups}

すべての特定の属性を別の属性の「すべてまたは任意」と共に持つ場合に備えて、属性をグループ化することもできます。 複数のグループを追加できます。

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
>アスタリスクを使用すると包括的なワイルドカードとして機能します。 そう `https://*.website.com` サブドメイン ( 例： `support.website.com`) をクリックします。 および `https://website.com/folder/*` 後続のフォルダー内のすべてのHTMLページにダイアログを配置します ( 例：この場合、フォルダーが「sports」だとします。そのため、次のようになります。website.com/sports/baseball.html、website.com/sports/football.htmlなど )。

## ストリームデザイナー {#stream-designer}

ストリームデザイナーには、チャット会話を形成するために追加できる様々なカードが含まれています。

<table>
 <tr>
  <td><strong>メッセージ
</strong></td>
  <td>応答を必要としない文を作成する場合に使用します ( 例：「やあ！ すべての項目は、コード SAVE25"を使用して、今日は 25%オフです。
</td>
 </tr>
 <tr>
  <td><strong>質問</strong></td>
  <td>複数選択の質問に対して、利用可能な回答を提供する場合に使用します ( 例：あなたはどのような車に興味がありますか？ 応答= SUV、コンパクト、トラックなど )。</td>
 </tr>
 <tr>
  <td><strong>情報取得</strong></td>
  <td>情報を収集する場合に使用します。 選択できる 3 つのフィールドは、「電子メールアドレス」、「電話番号」および「テキスト」（訪問者が独自のメッセージを書き込むことができます）です。</td>
 </tr>
 <tr>
  <td><strong>予定スケジューラ</strong></td>
  <td>訪問者に、フォローアップをスケジュールするために使用可能な日付のカレンダーを提供します。 カレンダーの可用性の反映 <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md#routing">次のエージェントが並んでいる</a>.</td>
 </tr>
 <tr>
  <td><strong>ゴール</strong></td>
  <td>訪問者に表示されないカードはこれだけです。 特定のチャット内で目標を達成した時点を決定する必要があります ( 例：訪問者の e メールを収集することが目標の場合は、ストリームの情報キャプチャの直後に目標カードを配置します )。</td>
 </tr>
</table>

**ストリームの作成**

次のものがあります。 _多数の_ 可能なストリームの組み合わせ。 例を見てみましょう [この記事では、](/help/marketo/product-docs/demand-generation/dynamic-chat/create-a-stream.md).

## レポート {#reports}

「レポート」タブで、過去 90 日間のデータを表示します。 各カテゴリは以下で定義します。

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
  <td><strong>完了済み</strong></td>
  <td>訪問者がダイアログのブランチの終わりに達するたびに増分されます。</td>
 </tr>
 <tr>
  <td><strong>キャプチャされた担当者</strong></td>
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
