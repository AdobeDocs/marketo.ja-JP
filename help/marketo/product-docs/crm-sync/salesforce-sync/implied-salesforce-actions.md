---
unique-page-id: 4719304
description: 黙示的なSalesforceアクション — Marketto Docs — 製品ドキュメント
title: 黙示的なSalesforceアクション
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '149'
ht-degree: 0%

---


# 黙示的なSalesforceアクション{#implied-salesforce-actions}

Salesforce固有のフローステップが実行される場合、追加のステップが自動的に実行されることがあります。 次にルールを示します。

[Salesforce.com](http://Salesforce.com)*に現在連絡先またはリードがいない場合、*&#x200B;ルールが適用されます。

<table> 
 <thead> 
  <tr> 
   <th>マーケティングフローの手順</th> 
   <th>自動アクション</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>SFDC追加キャンペーン</td> 
   <td>担当者をSFDCに同期</td> 
  </tr> 
  <tr> 
   <td>SFDCキャンペーンのステータスの変更</td> 
   <td>担当者をSFDC<br>追加とSFDCキャンペーンに同期</td> 
  </tr> 
  <tr> 
   <td>所有者の変更</td> 
   <td><p>担当者をSFDCに同期</p></td> 
  </tr> 
  <tr> 
   <td>人をコンバージョン</td> 
   <td><p>担当者をSFDCに同期</p></td> 
  </tr> 
  <tr> 
   <td>タスクの作成</td> 
   <td>担当者をSFDCに同期</td> 
  </tr> 
 </tbody> 
</table>

**SFDC Type** Filterを使用して、スマートリスト内のSFDCレコードをフィルターで除外できます。演算子は「空ではありません」に設定します。 すべてのSFDCレコードは、このフィールドに値を持ちます。

これらの自動アクションは、リードが現在[Salesforce.com](http://Salesforce.com)にない場合にのみ発生します。

セールスフォースの同期はかっこいいでしょ？
