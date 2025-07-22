---
description: セールスアクティビティ属性の Salesforce へのログ - Marketo ドキュメント - 製品ドキュメント
title: セールスアクティビティ属性の Salesforce へのログ
exl-id: fdefe53b-eb99-48ce-a04e-3666be33fea4
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 62%

---

# 販売アクティビティ属性の [!DNL Salesforce] へのロギング {#logging-sales-activity-attributes-to-salesforce}

Salesforce管理者は、カスタムアクティビティフィールドを [!DNL Salesforce] に手動で追加できます。

1. [!DNL Salesforce] アカウントで、「設定 **[!UICONTROL をクリック]** します。

1. クイック検索フィールドで「アクティビティのカスタムフィールド」を検索し、クリックします。

1. 「**[!UICONTROL 新規]**」をクリックします。

1. 以下のテーブルに基づいて、追加するフィールドに対応するデータタイプを選択し、「**[!UICONTROL 次へ]**」をクリックします。

1. 追加するフィールドに対応するフィールド名とラベルを入力します。

次の表では各列を説明します。

* **フィールドラベル**:UI に表示されるフィールド名（この名前は、チームが読みやすいようにカスタマイズできます）
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
  <td>[!UICONTROL 呼び出しの結果 &#x200B;]</td>
  <td>mktosales_call_outcome</td>
  <td>mktosales_call_outcome__c</td>
  <td>テキスト</td>
  <td>50</td>
 </tr>
 <tr>
  <td>[!UICONTROL 呼び出しの理由 &#x200B;]</td>
  <td>mktosales_call_reason</td>
  <td>mktosales_call_reason__c</td>
  <td>テキスト</td>
  <td>50</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Call Local Presence ID]</td>
  <td>MSE_Call_Local_Presence_ID</td>
  <td>MSE_Call_Local_Presence_ID__c</td>
  <td>テキスト</td>
  <td>255</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo セールス コール録画 URL]</td>
  <td>MSE_Call_Recording</td>
  <td>MSE_Call_Recording__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketoセールス・キャンペーン &#x200B;]</td>
  <td>MSE_Campaign</td>
  <td>MSE_Campaign__c</td>
  <td>テキスト</td>
  <td>255</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Campaign の現在の手順 &#x200B;]</td>
  <td>MSE_Current_Campaign_Step</td>
  <td>MSE_Current_Campaign_Step__c</td>
  <td>テキスト</td>
  <td>255</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo販売キャンペーン URL]</td>
  <td>MSE_Campaign_Details_Link</td>
  <td>MSE_Campaign_Details_Link__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo営業向けメール添付ファイルを表示 &#x200B;]</td>
  <td>MSE_Presentation_Viewed</td>
  <td>MSE_Presentation_Viewed__c</td>
  <td>チェックボックス</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Email Clicked]</td>
  <td>MSE_Clicked</td>
  <td>MSE_Clicked__c</td>
  <td>チェックボックス</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo営業メール返信 &#x200B;]</td>
  <td>MSE_Replied</td>
  <td>MSE_Replied__c</td>
  <td>チェックボックス</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo営業電子メールのステータス &#x200B;]</td>
  <td>MSE_Email_Status</td>
  <td>MSE_Email_Status__c</td>
  <td>テキスト</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo営業メールテンプレート &#x200B;]</td>
  <td>MSE_Template</td>
  <td>MSE_Template__c</td>
  <td>テキスト</td>
  <td>255</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo営業メールテンプレート URL]</td>
  <td>MSE_Template_Details</td>
  <td>MSE_Template_Details__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo営業メール URL]</td>
  <td>MSE_Details</td>
  <td>MSE_Details__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketoの営業メールが表示されました &#x200B;]</td>
  <td>MSE_Viewed</td>
  <td>MSE_Viewed__c</td>
  <td>チェックボックス</td>
  <td></td>
 </tr>
</table>
