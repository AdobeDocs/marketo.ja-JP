---
description: 動的チャットの概要 - Marketo ドキュメント - 製品ドキュメント
title: 動的チャットの概要
exl-id: 73ab651e-bb11-459d-aa6a-39d9e208d512
source-git-commit: 5cd5873132e38d7adea02739da39aebeb3979124
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 59%

---

# 動的チャットの概要 {#dynamic-chat-overview}

動的チャットでは、使いやすいインターフェイスを利用して、web サイトを訪問するリードと取引先の両方をターゲットに設定できます。名前、取引先責任者情報、フリーテキストなど、関連するコンテンツを収集します。サイト訪問者は、セールスチームとのミーティングを予約することもできます。動的チャットのアクティビティとエンゲージメントデータを使用して、Marketo プログラムにメンバーを追加し、クロスチャネルアクティビティをトリガーできます。

>[!NOTE]
>
>動的チャットは徐々に展開されている段階にあり、現在は限定で使用可能です。このページは、一般提供（GA）の詳細が利用可能になり次第、更新されます。

>[!TIP]
>
>[このページ](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/dynamic-chat/dynamic-chat-overview.html?lang=ja)を参照して、動的チャットのチュートリアルビデオを表示します。

## 統合 {#integrations}

動的チャットの主要な要素は、Marketo サブスクリプションとネイティブにインターフェイスする機能です。この統合の全機能を活用するには、まずデータ同期を開始する必要があります。 Marketo データベースのサイズによっては、最初の [1 回限りの同期](/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/connect-dynamic-chat-to-marketo.md)が完了するまでに最大 24 時間かかる場合があります。

以下が同期されます。

* リードフィールドデータ
* 会社フィールドデータ
* アクティビティデータ

## ダイアログ {#dialogues}

ダイアログは、単一のチャットエンゲージメントを表します。Web サイト訪問者に対して魅力的なチャットダイアログを開くのに必要なすべての要素を含むコンテナと考えてください。各ダイアログで、ダイアログを表示するページ、表示するページ、ダイアログ自体の内容とフローを指定できます。 さらに、指標を見つけて、ダイアログのパフォーマンスを確認できます。[ダイアログの詳細](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/dialogue-overview.md){target="_blank"}.

## 設定 {#configuration}

「設定」タブで、様々なダイアログの外観をカスタマイズします。フォント、色、応答時間などを変更します。[設定の詳細を表示](/help/marketo/product-docs/demand-generation/dynamic-chat/configuration.md){target="_blank"}

## カレンダー {#calendar}

Chatbot の予定スケジュールに使用する Outlook または Gmail の予定表に接続します。 [カレンダーの詳細を表示](/help/marketo/product-docs/demand-generation/dynamic-chat/appointment-scheduling/calendar.md){target="_blank"}

## 会議 {#meetings}

Web サイトの訪問者が様々なダイアログを使用してスケジュールしたすべての予定が表示されます。[会議の詳細を表示](/help/marketo/product-docs/demand-generation/dynamic-chat/appointment-scheduling/meetings.md){target="_blank"}

## ルーティング {#routing}

ここでは、カレンダーに関連付けられたすべてのエージェントのリスト、Web サイト訪問者に表示される順序、カスタムルーティングルールの作成を確認できます。 [ルーティングの詳細](/help/marketo/product-docs/demand-generation/dynamic-chat/appointment-scheduling/routing.md){target="_blank"}

## よくある質問 {#faq}

**Dynamic Chat は、会社の Web サイトの任意の場所にインストールできますか。それとも、Marketoのランディングページでのみ機能しますか。**

Dynamic Chat の JavaScript スニペットは、任意の Web サイトおよびMarketoのランディングページにインストールできます。

**レポート用のデータはどのくらいの期間保存されますか？**

90 日です（制限の完全なリストは、[以下](#limits-in-dynamic-chat)を参照）。

**動的チャットはライブチャットを許可していますか？**

いいえ、事前に決定された応答のみを利用します。

**Dynamic Chat は英語以外の言語をサポートしていますか？**

あります。Dynamic Chat は、次の言語をサポートしています。フランス語、ドイツ語、日本語、スペイン語、イタリア語、ポルトガル語（ブラジル）、韓国語、簡体字中国語、繁体字中国語。 詳しくは、 [以下の節](#changing-the-language).

**AI／NLP 機能はサポートしていますか？**

AI／NLP 機能はサポートしていません。

**匿名ユーザをターゲットにするには、どうすればよいですか？**

ダイアログで、_Person Email is Empty_ 属性を使用します。

## 言語の変更 {#changing-the-language}

ダイナミックチャットの言語を変更するには、次の手順に従います。

>[!IMPORTANT]
>
>プロファイルレベルで言語を変更すると、の言語が変更されます _すべて_ Experience Cloudアプリケーションは、Dynamic Chat だけではありません。

1. Experience Cloudアカウントで、設定アイコンをクリックし、「 」を選択します。 **環境設定**.

   ![](assets/dynamic-chat-overview-1.png)

1. メールアドレスの下の現在の言語をクリックします。

   ![](assets/dynamic-chat-overview-2.png)

1. 新しい言語（第 2 言語はオプション）を選択し、 **保存**.

   ![](assets/dynamic-chat-overview-3.png)

   >[!NOTE]
   >
   >数十の言語から選択できますが、Dynamic Chat では次の言語のみをサポートしています。英語、フランス語、ドイツ語、日本語、スペイン語、イタリア語、ポルトガル語（ブラジル）、韓国語、簡体字中国語、繁体字中国語。

言語を更新すると、自身で入力した単語（ストリーム応答など）を除き、アプリ自体のすべての情報が変更されます。

## 動的チャットの制限 {#limits-in-dynamic-chat}

<table>
  <th>パラメーター</th>
  <th>説明</th>
  <th>制限</th>
 <tr>
  <td>ダイアログ総数</td>
  <td>ダイアログの数（公開および下書き）</td>
  <td>500</td>
 </tr>
 <tr>
  <td>合計カレンダー</td>
  <td>接続されているカレンダーの数</td>
  <td>25</td>
 </tr>
 <tr>
  <td>合計ユーザー数（管理者およびマーケティングユーザー）</td>
  <td>ダイナミックチャットインスタンスごとに許可される結合ユーザー数</td>
  <td>50</td>
 </tr>
 <tr>
  <td>公開済みダイアログ</td>
  <td>保存された公開済みダイアログの数</td>
  <td>100</td>
 </tr>
 <tr>
  <td>ダイアログごとのターゲット URL</td>
  <td>単一のダイアログに追加できるターゲット URL の数</td>
  <td>20</td>
 </tr>
 <tr>
  <td>ダイアログごとの属性</td>
  <td>単一のダイアログのオーディエンス条件に追加できる属性の数</td>
  <td>100</td>
 </tr>
 <tr>
  <td>グループ</td>
  <td>単一のダイアログに追加できるグループの数</td>
  <td>10</td>
 </tr>
 <tr>
  <td>グループごとの属性</td>
  <td>グループに追加できる属性の数</td>
  <td>10</td>
 </tr>
 <tr>
  <td>カード</td>
  <td>ダイアログごとにキャンバスに追加できるカードの数</td>
  <td>500</td>
 </tr>
 <tr>
  <td>匿名リードデータの保持期間</td>
  <td>エンゲージメントのない匿名リードの情報が保持される期間</td>
  <td>90 日間</td>
 </tr>
 <tr>
  <td>目標アクティビティの保持期間</td>
  <td>目標アクティビティデータの保持期間</td>
  <td>24 か月</td>
 </tr>
 <tr>
  <td>ドキュメントアクティビティの保持期間</td>
  <td>ドキュメントのアクティビティデータが保持される期間</td>
  <td>24 か月</td>
 </tr>
 <tr>
  <td>ダイアログアクティビティの保持期間に関するインタラクション</td>
  <td>ダイアログアクティビティデータとのやり取りの保持期間</td>
  <td>90 日間</td>
 </tr>
 <tr>
  <td>会議予約アクティビティの保持期間</td>
  <td>会議予約アクティビティが動的チャットに保存される時間</td>
  <td>24 か月</td>
 </tr>
 <tr>
  <td>関与した会話</td>
  <td>Web 訪問者が 1 ヶ月に関与できるチャット会話の数</td>
  <td>250</td>
 </tr>
 <tr>
  <td>トリガーされた会話</td>
  <td>Web 訪問者に 1 ヶ月に表示できるチャットの会話数</td>
  <td>25,000</td>
 </tr>
</table>
