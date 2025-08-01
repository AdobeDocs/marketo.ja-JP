---
description: '[!DNL Dynamic Chat] アクティビティ - Marketo ドキュメント – 製品ドキュメント'
title: '[!DNL Dynamic Chat] アクティビティ'
exl-id: ef3bb1a3-6758-4798-92eb-fef28a5ff9c7
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 5%

---

# [!DNL Dynamic Chat] アクティビティ {#dynamic-chat-activities}

[!DNL Dynamic Chat] では、スマートリストで使用するためのいくつかのフィルターとトリガーを提供しています。

![](assets/dynamic-chat-activities-1.png)

## 定義 {#definitions}

<table>
<thead>
<tbody>
  <tr>
    <td style="width:25%"><b>トリガー起動</b></td>
    <td>トリガーイベントは、訪問者がダイアログまたは会話フローのターゲティング条件を満たし、ダイアログに表示されたときに発生します。
    <br> セッションごとに、訪問者ごとに 1 つのトリガーイベント。</td>
  </tr>
  <tr>
    <td style="width:25%"><b>会話フロー/ダイアログに関与</b></td>
    <td>エンゲージメントは、web 訪問者がダイアログまたは会話フローで、最初にプロンプトをクリックしたときに発生します（複数選択オプションのクリック、情報の送信、会議の予約、ドキュメントの開封など）。 訪問者がダイアログまたは会話フローを開いても、プロンプトをクリックしない場合、エンゲージメントは <b> 記録されません </b>。
    <br> セッションごとに、訪問者ごとに 1 つのエンゲージメントイベント。</td>
  </tr>
   <tr>
    <td style="width:25%"><b>エージェントとやり取りしました</b></td>
    <td>訪問者がライブチャットエージェントに正常に接続したときに発生します。
    <br> 訪問者ごとに、セッションごとに 1 人がエージェントイベントに関与しました。</td>
  </tr>
  <tr>
    <td style="width:25%"><b> ドキュメントを操作済み</b></td>
    <td>訪問者がドキュメント カードのドキュメントをクリックすると発生します。
    <br> 訪問者ごとに、セッションごとに複数のドキュメントインタラクションが存在する可能性があります。</td>
  </tr>
  <tr>
    <td style="width:25%"><b>目標に到達しました</b></td>
    <td>訪問者が目標に到達したときに発生します。 <br> セッションごとに、訪問者ごとに複数の目標達成イベントがある可能性があります。</td>
  </tr>
  <tr>
    <td style="width:25%"><b> ミーティングをスケジュール済み</b></td>
    <td>訪問者がDynamic Chat エージェントとのミーティングを予約すると発生します。
    <br> セッションごとに、訪問者ごとに複数の会議予約イベントが存在する可能性があります。</td>
  </tr>
</tbody>
</table>

## 注意事項 {#things-to-note}

* 条件は、[!DNL Dynamic Chat] のフローステップでサポートされています
* [!DNL Dynamic Chat] アクティビティは [[!DNL Marketo Sales Insight]](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md){target="_blank"} に同期できます
* 個々の [!DNL Dynamic Chat] アクティビティは、人物レコードのアクティビティログに表示できます
