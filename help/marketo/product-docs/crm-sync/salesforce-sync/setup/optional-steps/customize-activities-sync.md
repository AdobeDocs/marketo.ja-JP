---
unique-page-id: 4719294
description: アクティビティの同期のカスタマイズ — Marketto Docs — 製品ドキュメント
title: アクティビティの同期のカスタマイズ
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---


# アクティビティの同期のカスタマイズ {#customize-activities-sync}

Sales Insightを使用しない場合は、 [](http://docs.marketo.com/display/DOCS/Marketo+Sales+Insight)Marketorは特定のイベントに対してSalesforceアクティビティ履歴レコードを作成できます。 有効にする方法を次に示します。

1. **Adminに移動します。 **

   ![](assets/admin.png)

1. 「 **Salesforce**」をクリックし、「 **同期オプションの編集**」をクリックします。

   ![](assets/two-1.png)

1. Salesforceにプッシュするアクティビティの横のチェックボックスをオンにし、「 **保存**」をクリックします。

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >有効になると、Marketoは3か月分のアクティビティ履歴をプッシュします。 データ量によっては、完了までに数日かか *る場合があります*。 最初のアクティビティのプッシュ中に発生する更新は、最初のアクティビティの同期が完了するまで遅延する可能性があります。

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <thead> 
  <tr> 
   <th>アクティビティタイプ</th> 
   <th>説明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>記入済みのフォーム</td> 
   <td>任意のマーケティングフォームへの入力</td> 
  </tr> 
  <tr> 
   <td>リストに追加</td> 
   <td><p>フローステップ：静的リストに追加されました</p></td> 
  </tr> 
  <tr> 
   <td>電子メール送信</td> 
   <td>フローステップ：Eメールが送信されました</td> 
  </tr> 
  <tr> 
   <td>電子メール配信</td> 
   <td>電子メールを受信（バウンスなし）</td> 
  </tr> 
  <tr> 
   <td>開封済み電子メール</td> 
   <td>電子メールを開きました（画像をブロックしません）</td> 
  </tr> 
  <tr> 
   <td>電子メール内のクリックされたリンク</td> 
   <td>Marketorが送信した電子メール内のリンクをクリック</td> 
  </tr> 
  <tr> 
   <td>リストから削除</td> 
   <td>フローステップ：静的リストから削除されました</td> 
  </tr> 
  <tr> 
   <td>フローから削除</td> 
   <td>フローステップ：フローから削除</td> 
  </tr> 
  <tr> 
   <td>送信された販売の電子メール</td> 
   <td>Marketor Sales Insight経由で電子メールが送信された</td> 
  </tr> 
  <tr> 
   <td>開封済みの販売電子メール</td> 
   <td>Marketor Sales Insight経由で送信される電子メールを開きました。</td> 
  </tr> 
  <tr> 
   <td>販売の電子メールのリンクをクリック</td> 
   <td>Marketor Sales Insight経由で送信される電子メール内のリンクをクリックしました</td> 
  </tr> 
  <tr> 
   <td>受信した販売の電子メール</td> 
   <td>販売担当者がMSI Outlookプラグインで電子メールを受信し、ログに記録しました</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>**Reminder**
>
>
>「受信した販売の電子メール」が配信され **たとは限りません** 。 Sales Insight経由で送信された電子メールの配信ステータスはキャプチャされません。

>[!TIP]
>
>Salesforceに対するより多くのマーケティング情報の取り込みに関心がある場合は、 [Marketo Sales Insight](../../../../../product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) 製品をご覧ください。

