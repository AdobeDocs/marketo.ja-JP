---
description: Dynamic Chat の概要 — Marketo ドキュメント — 製品ドキュメント
title: Dynamic Chat の概要
exl-id: 73ab651e-bb11-459d-aa6a-39d9e208d512
source-git-commit: a437f39ccc5b1937c34ce43e7aedad82b22cf532
workflow-type: tm+mt
source-wordcount: '916'
ht-degree: 58%

---

# Dynamic Chat の概要 {#dynamic-chat-overview}

Dynamic Chat では、使いやすいインターフェイスを利用して、Web サイトを訪問するユーザーとアカウントの両方をターゲットに設定できます。名前、連絡先情報、フリーテキストなど、関連するコンテンツを収集します。サイト訪問者は、セールスチームとのミーティングを予約することもできます。Dynamic Chat のアクティビティとエンゲージメントデータを使用して、Marketo プログラムにメンバーを追加し、クロスチャネルアクティビティをトリガーすることができます。

>[!NOTE]
>
>Dynamic Chat は徐々に展開される過程にあり、現在は可用性が限られています。このページは、一般提供（GA）の詳細が利用可能になり次第、更新されます。

>[!TIP]
>
>[](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/dynamic-chat/dynamic-chat-overview.html)

## 統合 {#integrations}

Dynamic Chat の主要な要素は、Marketo サブスクリプションとネイティブにインターフェイスする機能です。この統合の全機能を活用するには、まずデータ同期を開始する必要があります。Marketo データベースのサイズによっては、最初の [1 回限りの同期](/help/marketo/product-docs/demand-generation/dynamic-chat/connect-dynamic-chat-to-marketo.md)が完了するまでに最大 24 時間かかる場合があります。

以下が同期されます。

* ユーザーフィールドデータ
* 会社フィールドデータ
* アクティビティデータ

## ダイアログ {#dialogues}

ダイアログは、単一のチャットエンゲージメントを表します。Web サイト訪問者に対して魅力的なチャットダイアログを開くのに必要なすべての要素を含むコンテナと考えてください。各ダイアログで、ダイアログを表示するページ、表示するページ、ダイアログ自体の内容とフローを指定できます。さらに、指標を見つけて、ダイアログのパフォーマンスを確認できます。[](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/dialogue-overview.md)

## 設定 {#configuration}

「設定」タブで、様々なダイアログの外観をカスタマイズします。フォント、色、応答時間などを変更します。[設定の詳細を表示](/help/marketo/product-docs/demand-generation/dynamic-chat/configuration.md)

## カレンダー {#calendar}

「カレンダー」タブで、（Outlook または Gmail）のカレンダーを接続して、Chatbot での予定スケジュールに使用します。ユーザーのカレンダーが Dynamic Chat に接続されると、そのユーザーはキューに追加され、Web サイトの訪問者が予定をスケジュールする際に使用できるようになります。

また、訪問者がユーザーのカレンダーに予定をスケジュールする際に訪問者に送信する招待の本文をカスタマイズすることもできます。

## 会議 {#meetings}

Web サイトの訪問者が様々なダイアログを使用してスケジュールしたすべての予定が表示されます。ここには、予約者のメールアドレス、予約したエージェント、予約の日時、会議があったかどうかが表示されます。

## ルーティング {#routing}

ここでは、カレンダーに関連付けられたすべてのエージェントのリストと、Web サイトの訪問者に表示される順序を確認できます。会議はラウンドロビン方式でおこなわれます。エージェントが 5 人いてエージェント 3 が最後の会議に出席した場合、エージェント 4 が次の会議に出席し、次にエージェント 5 がその次の会議に出席し、その後はエージェント 1 に戻ります。

## よくある質問 {#faq}

****

The Dynamic Chat JavaScript snippet can be installed on any website as well as Marketo landing pages.

**レポート用のデータはどのくらいの期間保存されますか？**

[](#limits-in-dynamic-chat)

**Dynamic Chat はライブチャットを許可していますか？**

いいえ、事前に決定された応答のみを利用します。

****

はい。Dynamic Chat supports the following languages: French, German, Japanese, Spanish, Italian, Brazilian Portuguese, Korean, Simplified Chinese, and Traditional Chinese. [](#changing-the-language)

**AI／NLP 機能はサポートしていますか？**

AI／NLP 機能はサポートしていません。

**匿名ユーザーをターゲットにするにはどうすればよいですか？**

ダイアログで、_Person Email is Empty_ 属性を使用します。

## Changing the Language {#changing-the-language}

Follow these steps to change your Dynamic Chat language.

>[!IMPORTANT]
>
>__

1. ****

   ![](assets/dynamic-chat-overview-1.png)

1. Click the current language under your email address.

   ![](assets/dynamic-chat-overview-2.png)

1. ****

   ![](assets/dynamic-chat-overview-3.png)

   >[!NOTE]
   >
   >There are a few dozen languages to choose from, however, Dynamic Chat only supports the following: English, French, German, Japanese, Spanish, Italian, Brazilian Portuguese, Korean, Simplified Chinese, and Traditional Chinese.

When you update the language, everything in the app itself changes except for the words you&#39;ve personally populated (e.g., stream responses).

## Limits in Dynamic Chat {#limits-in-dynamic-chat}

<table>
  <th>パラメーター</th>
  <th>説明</th>
  <th>制限</th>
 <tr>
  <td>Total Dialogues</td>
  <td>Total number of Dialogues (published and draft)</td>
  <td>500</td>
 </tr>
 <tr>
  <td>Published Dialogues</td>
  <td>Number of published Dialogues saved</td>
  <td>100</td>
 </tr>
 <tr>
  <td>Target URLs per Dialogue</td>
  <td>Number of Target URLs that can be added to a single Dialogue</td>
  <td>20</td>
 </tr>
 <tr>
  <td>Attributes per Dialogue</td>
  <td>Number of attributes that can be added to audience criteria for a single Dialogue</td>
  <td>100</td>
 </tr>
 <tr>
  <td>グループ</td>
  <td>Number of groups that can be added to a single Dialogue</td>
  <td>10</td>
 </tr>
 <tr>
  <td>Attributes per Group</td>
  <td>Number of attributes that can be added to a group</td>
  <td>10</td>
 </tr>
 <tr>
  <td>Cards</td>
  <td>Number of cards that can be added to the canvas per Dialogue</td>
  <td>500</td>
 </tr>
 <tr>
  <td>Anonymous Lead Data Retention Period</td>
  <td>Duration for how long information of an anonymous lead without any engagement will be retained</td>
  <td>90 日間</td>
 </tr>
 <tr>
  <td>Goal Activity Retention Period</td>
  <td>Amount of time goal activity data is retained</td>
  <td>24 か月</td>
 </tr>
 <tr>
  <td>Document Activity Retention Period</td>
  <td>Amount of time document activity data is retained</td>
  <td>24 か月</td>
 </tr>
 <tr>
  <td>Interacted w/ Dialogue Activity Retention Period</td>
  <td>Amount of time interacted with Dialogue activity data is retained</td>
  <td>90 日間</td>
 </tr>
 <tr>
  <td>Meeting Booking Activity Retention Period</td>
  <td>Amount of time meeting booking activity will be stored in Dynamic Chat</td>
  <td>24 か月</td>
 </tr>
</table>
