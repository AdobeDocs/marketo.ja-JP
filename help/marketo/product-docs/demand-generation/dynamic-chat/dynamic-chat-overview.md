---
description: Dynamic Chat の概要 - Marketo ドキュメント - 製品ドキュメント
title: Dynamic Chat の概要
feature: Dynamic Chat
source-git-commit: 0bc016e63626c880238316ff2130f12a31fdd717
workflow-type: tm+mt
source-wordcount: '696'
ht-degree: 82%

---

# Dynamic Chat の概要 {#dynamic-chat-overview}

Dynamic Chat では、使いやすいインターフェイスを利用して、web サイトを訪問するリードと取引先の両方をターゲットに設定できます。名前、取引先責任者情報、フリーテキストなど、関連するコンテンツを収集します。サイト訪問者は、ライブエージェントとチャットしたり、セールスチームとのミーティングを予約したりすることもできます。 Dynamic Chat のアクティビティとエンゲージメントデータを使用して、Marketo プログラムにメンバーを追加し、クロスチャネルアクティビティをトリガーできます。

>[!TIP]
>
>[このページ](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/dynamic-chat/dynamic-chat-overview.html?lang=ja)を参照して、Dynamic Chat のチュートリアルビデオを表示します。{target="_blank"}

## 統合 {#integrations}

Dynamic Chat の主要な要素は、Marketo サブスクリプションとネイティブにインターフェイスする機能です。この統合の全機能を活用するには、まずデータ同期を開始する必要があります。Marketo データベースのサイズによっては、最初の [1 回限りの同期](/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/adobe-marketo-engage.md){target="_blank"}が完了するまでに最大 24 時間かかる場合があります。

以下が同期されます。

* リードフィールドデータ
* 会社フィールドデータ
* アクティビティデータ

## ダイアログ {#dialogues}

ダイアログは、単一のチャットエンゲージメントを表します。Web サイト訪問者に対して魅力的なチャットダイアログを開くのに必要なすべての要素を含むコンテナと考えてください。各ダイアログで、ダイアログを表示するページ、表示するページ、ダイアログ自体の内容とフローを指定できます。さらに、指標を見つけて、ダイアログのパフォーマンスを確認できます。[ダイアログの詳細](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/dialogue-overview.md){target="_blank"}。

## 設定 {#configuration}

「設定」タブで、様々なダイアログの外観をカスタマイズします。フォント、色、応答時間などを変更します。[設定の詳細](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/configuration.md){target="_blank"}。

## カレンダー {#calendar}

Outlook または Gmail のカレンダーを接続して、チャットボットでの予定スケジュールに使用します。[カレンダーの詳細](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-settings.md#connect-calendar){target="_blank"}

## 会議 {#meetings}

Web サイトの訪問者が様々なダイアログを使用してスケジュールしたすべての予定が表示されます。[ミーティングの詳細](/help/marketo/product-docs/demand-generation/dynamic-chat/meeting-list.md){target="_blank"}

## ルーティング {#routing}

ここでは、カレンダーに関連付けられたすべてのエージェントのリストと、web サイトの訪問者に表示される順序を確認でき、またカスタムのルーティングルールを作成できます。[ルーティングの詳細](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/routing.md){target="_blank"}

## ライブチャット {#live-chat}

を通じてセールス担当者と連携するための適格な Web 訪問者を提供する [ライブチャット](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/live-chat-overview.md){target="_blank"}.

## 対話フロー {#conversational-flow}

[会話のデザイン](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-overview.md){target="_blank"} 指定したアクション（フォームへの入力、リンクのクリックなど）に基づいて訪問者がトリガーできるもの。

## 言語の変更 {#changing-the-language}

Dynamic Chat の言語を変更するには、以下の手順に従います。

>[!IMPORTANT]
>
>プロファイルレベルで言語を変更すると、Dynamic Chat だけでなく、_すべて_&#x200B;の Experience Cloud アプリケーションの言語が変更されます。

1. Experience Cloud アカウントで、設定アイコンをクリックし、「**環境設定**」を選択します。

   ![](assets/dynamic-chat-overview-1.png)

1. メールアドレスの下の現在の言語をクリックします。

   ![](assets/dynamic-chat-overview-2.png)

1. 新しい言語（第 2 言語はオプション）を選択し、「**保存**」をクリックします。

   ![](assets/dynamic-chat-overview-3.png)

   >[!NOTE]
   >
   >数十の言語から選択できますが、Dynamic Chat では以下の言語のみをサポートしています。英語、フランス語、ドイツ語、日本語、スペイン語、イタリア語、ポルトガル語（ブラジル）、韓国語、簡体字中国語、繁体字中国語。

言語を更新すると、自身で入力した単語（ストリーム応答など）を除き、アプリ自体のすべての情報が変更されます。

## Dynamic Chatデータ保持の制限 {#dynamic-chat-data-retention-limits}

以下に、Dynamic Chat内の制限/パラメーターの一部を示します。 完全なリストについては、Marketo Engage [製品の説明ページ](https://helpx.adobe.com/legal/product-descriptions/adobe-marketo-engage-product-description.html){target="_blank"}.

<table>
  <th>データタイプ</th>
  <th>保持期間</th>
 <tr>
  <td>エンゲージメントのない匿名リード</td>
  <td>90 日間</td>
 </tr>
 <tr>
  <td>目標アクティビティ</td>
  <td>24 か月</td>
 </tr>
 <tr>
  <td>ドキュメントアクティビティ</td>
  <td>24 か月</td>
 </tr>
 <tr>
  <td>ダイアログアクティビティとのやり取り</td>
  <td>90 日間</td>
 </tr>
 <tr>
  <td>会議の予約アクティビティ</td>
  <td>24 か月</td>
 </tr>
</table>

## よくある質問 {#faq}

**Dynamic Chat は、会社の web サイトの任意の場所にインストールできますか？それとも、Marketo のランディングページでのみ機能しますか？**

Dynamic Chat の JavaScript スニペットは、任意の web サイトおよび Marketo のランディングページにインストールできます。

**レポート用のデータはどのくらいの期間保存されますか？**

90 日間. 制限/パラメーターの完全なリストについては、Marketo Engage [製品の説明ページ](https://helpx.adobe.com/legal/product-descriptions/adobe-marketo-engage-product-description.html){target="_blank"}.

**Dynamic Chat は英語以外の言語をサポートしていますか？**

あります。Dynamic Chat は、以下の言語をサポートしています。フランス語、ドイツ語、日本語、スペイン語、イタリア語、ポルトガル語（ブラジル）、韓国語、簡体字中国語、繁体字中国語。詳しくは、 [言語の変更](#changing-the-language).

**AI／NLP 機能はサポートしていますか？**

AI／NLP 機能はサポートしていません。

**匿名ユーザーをターゲットにするには、どうすればよいですか？**

ダイアログで、_Person Email is Empty_ 属性を使用します。
