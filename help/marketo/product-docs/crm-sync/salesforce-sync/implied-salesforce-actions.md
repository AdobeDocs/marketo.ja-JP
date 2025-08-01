---
unique-page-id: 4719304
description: 暗黙的な Salesforce アクション - Marketo ドキュメント - 製品ドキュメント
title: 暗黙的な Salesforce アクション
exl-id: 88533588-77f2-465e-9644-a4f95b87f99d
feature: Salesforce Integration
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '141'
ht-degree: 63%

---

# 暗黙的な Salesforce アクション {#implied-salesforce-actions}

[!DNL Salesforce] 固有のフローステップを実行する場合は、追加のステップが自動的に実行されることがあります。 ルールは次のとおりです。

これらの規則は、人物が現在 [Salesforce.com](https://Salesforce.com){target="_blank"} に連絡先またはリードとして存在していない場合に適用されます。

<table>
 <thead>
  <tr>
   <th>Marketo フローステップ</th>
   <th>自動アクション</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>SFDC キャンペーンに追加する</td>
   <td>個人を SFDC に同期する</td>
  </tr>
  <tr>
   <td>SFDC キャンペーン内のステータスを変更する</td>
   <td>個人を SFDC に同期する<br>SFDC キャンペーンに追加する</td>
  </tr>
  <tr>
   <td>所有者を変更する</td>
   <td><p>個人を SFDC に同期する</p></td>
  </tr>
  <tr>
   <td>個人をコンバージョンする</td>
   <td><p>個人を SFDC に同期する</p></td>
  </tr>
  <tr>
   <td>タスクを作成する</td>
   <td>個人を SFDC に同期する</td>
  </tr>
 </tbody>
</table>

演算子を「**[!UICONTROL not empty]**」に設定した [!UICONTROL SFDCタイプ ] フィルターを使用して、スマート・リスト内のSFDCレコードをフィルタで除外できます。 すべての SFDC レコードでこのフィールドの値が設定されます。

これらの自動アクションは、リードが現在 [Salesforce.com ](https://salesforce.com){target="_blank"} に存在しない場合にのみ発生します。
