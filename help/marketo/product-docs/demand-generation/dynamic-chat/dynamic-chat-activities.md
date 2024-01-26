---
description: Dynamic Chat のアクティビティ - Marketo ドキュメント - 製品ドキュメント
title: Dynamic Chat のアクティビティ
feature: Dynamic Chat
exl-id: ef3bb1a3-6758-4798-92eb-fef28a5ff9c7
source-git-commit: b1101617ec670d42aed8c35044b656ba5fa0f9f5
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 19%

---

# Dynamic Chat のアクティビティ {#dynamic-chat-activities}

Dynamic Chatは、スマートリストで使用する複数のフィルターとトリガーを提供します。

![](assets/dynamic-chat-activities-1.png)

## 定義 {#definitions}

<table>
<thead>
<tbody>
  <tr>
    <td><b>トリガー起動</b></td>
    <td>トリガーイベントは、訪問者がダイアログまたは対話フローのターゲット条件を満たし、ダイアログが表示されたときに発生します。
    <br>訪問者ごとに 1 つのトリガーイベント、セッションごとに 1 つ。</td>
  </tr>
  <tr>
    <td><b>会話のフロー/ダイアログに関与しました</b></td>
    <td>エンゲージメントは、Web 訪問者がダイアログまたは対話フローのプロンプト（複数選択オプションのクリック、情報の送信、会議の予約、ドキュメントの開封など）を初めてクリックしたときに発生します。 訪問者がダイアログまたは対話型フローを開いたが、プロンプトをクリックしなかった場合、エンゲージメントは <b>not</b> ログに記録されました。 
    <br>訪問者ごとに、セッションごとに 1 つのエンゲージメントイベント。</td>
  </tr>
   <tr>
    <td><b>代理人とエンゲージ済み</b></td>
    <td>訪問者がライブチャットエージェントに正常に接続されたときに発生します。
    <br>訪問者ごとに、セッションごとに、エージェントイベントに関与したユーザーが 1 人。</td>
  </tr>
  <tr>
    <td><b>ドキュメントとのやり取り</b></td>
    <td>訪問者がドキュメントカード内のドキュメントをクリックすると発生します。
    <br>訪問者ごとに、セッションごとに複数のドキュメントの操作が可能です。</td>
  </tr>
  <tr>
    <td><b>目標に達しました</b></td>
    <td>訪問者が目標に達したときに発生します。 <br>セッションごとに、訪問者ごとに複数の目標到達イベントを設定できます。</td>
  </tr>
  <tr>
    <td><b>予定されている会議</b></td>
    <td>訪問者がDynamic Chatエージェントとの会議を予約すると発生します。
    <br>訪問者ごとに、セッションごとに、複数の会議を予約したイベントを設定できます。</td>
  </tr>
</tbody>
</table>

## 注意事項 {#things-to-note}

* 条件は、Dynamic Chat のフローステップでサポートされます
* Dynamic Chat のアクティビティは、[Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md){target="_blank"} と同期されます
* 人物レコードのアクティビティログで、個々の Dynamic Chat アクティビティを表示できます
