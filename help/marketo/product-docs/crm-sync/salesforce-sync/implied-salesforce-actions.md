---
unique-page-id: 4719304
description: 黙示的なSalesforceアクション —Marketoドキュメント — 製品ドキュメント
title: 黙示的なSalesforceアクション
exl-id: 88533588-77f2-465e-9644-a4f95b87f99d
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '143'
ht-degree: 21%

---

# 黙示的なSalesforceアクション{#implied-salesforce-actions}

Salesforce固有のフローステップが実行される場合、追加のステップが自動的に実行されることがあります。 次にルールを示します。

[Salesforce.com](https://Salesforce.com)_に現在連絡先またはリードがいない場合、_&#x200B;ルールが適用されます。

<table> 
 <thead> 
  <tr> 
   <th>Marketoフローステップ</th> 
   <th>自動アクション</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>SFDC キャンペーンに追加</td> 
   <td>担当者を SFDC に同期</td> 
  </tr> 
  <tr> 
   <td>SFDC キャンペーン内のステータスの変更</td> 
   <td>担当者をSFDC<br>追加とSFDCキャンペーンに同期</td> 
  </tr> 
  <tr> 
   <td>所有者の変更</td> 
   <td><p>担当者を SFDC に同期</p></td> 
  </tr> 
  <tr> 
   <td>担当者の変換</td> 
   <td><p>担当者を SFDC に同期</p></td> 
  </tr> 
  <tr> 
   <td>タスクの作成</td> 
   <td>担当者を SFDC に同期</td> 
  </tr> 
 </tbody> 
</table>

**SFDC Type** Filterを使用して、スマートリスト内のSFDCレコードをフィルターで除外できます。演算子は「空ではありません」に設定します。 すべてのSFDCレコードは、このフィールドに値を持ちます。

これらの自動アクションは、リードが現在[Salesforce.com](https://salesforce.com)にない場合にのみ発生します。
