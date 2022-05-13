---
description: セールスアクティビティ属性の Salesforce へのログ — Marketo ドキュメント — 製品ドキュメント
title: セールスアクティビティ属性の Salesforce へのログ
exl-id: fdefe53b-eb99-48ce-a04e-3666be33fea4
source-git-commit: 222b0692998be1fd15dc6465af1da627e1c32683
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 96%

---

# セールスアクティビティ属性の Salesforce へのログ {#logging-sales-activity-attributes-to-salesforce}

Salesforce 管理者は、カスタムアクティビティフィールドを Salesforce に手動で追加できます。

1. Salesforce アカウントで、「**設定**」をクリックします。

1. クイック検索フィールドで「アクティビティのカスタムフィールド」を検索し、クリックします。

1. 「**新規**」をクリックします。

1. 以下のテーブルに基づいて、追加するフィールドに対応するデータタイプを選択し、「**次へ**」をクリックします。

1. 追加するフィールドに対応するフィールド名とラベルを入力します。

次の表では各列を説明します。

* **フィールドラベル**：UI に表示されるフィールド名 （この名前は、チームが読みやすくするためにカスタマイズできます）
* **フィールド名**：フィールドの技術的な名前（入力したフィールド名が、下の表の「フィールド名」と一致していることを確認してください）
* **API 名**：API 用のフィールドの技術的な名前（入力した API 名が以下の表の API 名と一致していることを確認してください）
* **データタイプ**：フィールドのタイプ
* **サイズ**：テキストフィールドのサイズ

<table>
 <tr>
  <th>フィールドラベル</th>
  <th>フィールド名</th>
  <th>API 名</th>
  <th>データタイプ</th>
  <th>サイズ</th>
 </tr>
 <tr>
  <td>Marketo セールス電話ローカルプレゼンス ID</td>
  <td>MSE_Call_Local_Presence_ID</td>
  <td>MSE_Call_Local_Presence_ID__c</td>
  <td>テキスト</td>
  <td>255</td>
 </tr>
 <tr>
  <td>Marketo セールス電話録音 URL</td>
  <td>MSE_Call_Recording</td>
  <td>MSE_Call_Recording__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>Marketo セールスキャンペーン</td>
  <td>MSE_Campaign</td>
  <td>MSE_Campaign__c</td>
  <td>テキスト</td>
  <td>255</td>
 </tr>
 <tr>
  <td>Marketo セールスキャンペーンの最新ステップ</td>
  <td>MSE_Current_Campaign_Step</td>
  <td>MSE_Current_Campaign_Step__c</td>
  <td>テキスト</td>
  <td>255</td>
 </tr>
 <tr>
  <td>Marketo セールスキャンペーン URL</td>
  <td>MSE_Campaign_Details_Link</td>
  <td>MSE_Campaign_Details_Link__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>閲覧済みの Marketo セールスメール添付ファイル</td>
  <td>MSE_Presentation_Viewed</td>
  <td>MSE_Presentation_Viewed__c</td>
  <td>チェックボックス</td>
  <td></td>
 </tr>
 <tr>
  <td>クリック済みの Marketo セールスメール</td>
  <td>MSE_Clicked</td>
  <td>MSE_Clicked__c</td>
  <td>チェックボックス</td>
  <td></td>
 </tr>
 <tr>
  <td>返信済みの Marketo セールスメール</td>
  <td>MSE_Replied</td>
  <td>MSE_Replied__c</td>
  <td>チェックボックス</td>
  <td></td>
 </tr>
 <tr>
  <td>Marketo セールスメールステータス</td>
  <td>MSE_Email_Status</td>
  <td>MSE_Email_Status__c</td>
  <td>テキスト</td>
  <td></td>
 </tr>
 <tr>
  <td>Marketo セールスメールテンプレート</td>
  <td>MSE_Template</td>
  <td>MSE_Template__c</td>
  <td>テキスト</td>
  <td>255</td>
 </tr>
 <tr>
  <td>Marketo セールスメールテンプレート URL</td>
  <td>MSE_Template_Details</td>
  <td>MSE_Template_Details__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>Marketo セールスメール URL</td>
  <td>MSE_Details</td>
  <td>MSE_Details__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>閲覧済みの Marketo セールスメール</td>
  <td>MSE_Viewed</td>
  <td>MSE_Viewed__c</td>
  <td>チェックボックス</td>
  <td></td>
 </tr>
</table>
