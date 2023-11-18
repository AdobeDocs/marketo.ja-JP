---
unique-page-id: 4719304
description: 暗黙的な Salesforce アクション - Marketo ドキュメント - 製品ドキュメント
title: 暗黙的な Salesforce アクション
exl-id: 88533588-77f2-465e-9644-a4f95b87f99d
feature: Salesforce Integration
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '143'
ht-degree: 100%

---

# 暗黙的な Salesforce アクション {#implied-salesforce-actions}

Salesforce 固有のフローステップが実行されると、追加の手順が自動的に実行される場合があります。ルールは次のとおりです。

これらのルールは、個人が現在 [Salesforce.com ](https://Salesforce.com){target="_blank"}に連絡先またはリードとして存在しない場合に適用されます。

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

**[!UICONTROL SFDC Type]** フィルターを演算子を「空でない」に設定して使用すると、スマートリスト内の SFDC レコードを除外できます。すべての SFDC レコードでこのフィールドの値が設定されます。

これらの自動アクションは、リードが現在 [Salesforce.com ](https://salesforce.com) に存在しない場合にのみ発生します。{target="_blank"}
