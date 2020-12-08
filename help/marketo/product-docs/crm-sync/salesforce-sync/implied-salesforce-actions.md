---
unique-page-id: 4719304
description: 黙示的なSalesforceアクション — Marketto Docs — 製品ドキュメント
title: 黙示的なSalesforceアクション
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '200'
ht-degree: 0%

---


# 黙示的なSalesforceアクション {#implied-salesforce-actions}

>[!NOTE]
>
>**FYI**
>
>Marketoは現在、すべての購読で言語を標準化しているので、購読およびdocs.marketo.comの人物/人物にリード/リードを表示できます。 これらの用語は同じことを意味し、記事の説明には影響しません。 他にも変化がある。 [詳細情報](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

Salesforce固有のフローステップが実行される場合、追加のステップが自動的に実行されることがあります。 次にルールを示します。

これらのルールは、 *担当者が現在 [](http://Salesforce.com)* Salesforce.comに連絡先またはリードとしていない場合に適用されます。

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
   <td>担当者をSFDCキャンペーンに<br>SFDCddに同期</td> 
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

演算子を「is not empty」に設定し、 **SFDC Type** Filterを使用して、スマートリスト内のSFDCレコードをフィルタリングできます。 すべてのSFDCレコードは、このフィールドに値を持ちます。

これらの自動アクションは、現在 [Salesforce.comにリードがない場合にのみ発生します。](http://Salesforce.com)

セールスフォースの同期はかっこいいでしょ？
