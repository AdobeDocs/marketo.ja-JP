---
description: スマートリスト用のDynamic Chat フィルターとトリガーについて説明します。 トリガーされた、エンゲージメントされた、目標を達成したイベントを使用して、Marketoでセグメント化と自動化を行います。
title: '[!DNL Dynamic Chat] アクティビティ'
exl-id: ef3bb1a3-6758-4798-92eb-fef28a5ff9c7
source-git-commit: 031eb5f3ff8aac185ce496664f984a4c745c6e44
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 83%

---

# [!DNL Dynamic Chat] アクティビティ {#dynamic-chat-activities}

[!DNL Dynamic Chat] では、スマートリストで使用する複数のフィルターとトリガーを提供します。

![](assets/dynamic-chat-activities-1.png)

## 定義 {#definitions}

<table>
<thead>
<tbody>
  <tr>
    <td style="width:25%"><b>トリガー起動</b></td>
    <td>トリガーイベントは、訪問者がダイアログまたは対話型フローのターゲティング条件を満たし、ダイアログに表示された際に発生します。
    <br>訪問者 1 人あたり、セッションごとに 1 つのトリガーイベント。</td>
  </tr>
  <tr>
    <td style="width:25%"><b>対話型フロー／ダイアログでエンゲージ</b></td>
    <td>エンゲージメントは、web 訪問者がダイアログまたは対話型フロー内のプロンプト（複数選択オプションをクリックする、情報を送信する、会議を予約する、ドキュメントを開くなど）を最初にクリックした際に発生します。訪問者がダイアログまたは会話フローを開いても、プロンプトをクリックしない場合、エンゲージメントは <b> 記録されません </b>。
    <br>訪問者 1 人あたり、セッションごとに 1 つのエンゲージメントイベント。</td>
  </tr>
   <tr>
    <td style="width:25%"><b>エージェントとエンゲージしました</b></td>
    <td>訪問者がライブチャットエージェントに正常に接続された際に発生します。
    <br>訪問者 1 人あたり、セッションごとに 1 つのエージェントにエンゲージしたイベント。</td>
  </tr>
  <tr>
    <td style="width:25%"><b>ドキュメントを操作済み</b></td>
    <td>訪問者がドキュメントカード内のドキュメントをクリックした際に発生します。
    <br>訪問者 1 人あたり、セッションごとに複数のドキュメントへの操作が発生する場合があります。</td>
  </tr>
  <tr>
    <td style="width:25%"><b>目標に到達済み</b></td>
    <td>訪問者が目標に到達した際に発生します。<br>訪問者 1 人あたり、セッションごとに複数の目標に到達済みイベントが発生する場合があります。</td>
  </tr>
  <tr>
    <td style="width:25%"><b>ミーティングをスケジュール済み</b></td>
    <td>訪問者が Dynamic Chat エージェントとのミーティングを予約した際に発生します。
    <br>訪問者 1 人あたり、セッションごとに複数のミーティングを予約済みイベントが発生する場合があります。</td>
  </tr>
</tbody>
</table>

## 注意事項 {#things-to-note}

* 条件は、[!DNL Dynamic Chat] のフローステップでサポートされます。
* [!DNL Dynamic Chat] アクティビティは [[!DNL Marketo Sales Insight]](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md){target="_blank"} に同期できます。
* 人物レコードのアクティビティログで、個々の [!DNL Dynamic Chat] アクティビティを表示できます。
