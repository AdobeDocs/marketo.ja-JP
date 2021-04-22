---
unique-page-id: 4719294
description: アクティビティのカスタマイズの同期 —Marketoドキュメント — 製品ドキュメント
title: アクティビティの同期のカスタマイズ
exl-id: 938d83dc-b9b1-41d8-bf98-04548b074ec4
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 12%

---

# アクティビティ同期のカスタマイズ{#customize-activities-sync}

Marketo販売インサイトを使用しない場合、Marketoは特定のイベントに対してSalesforceアクティビティ履歴レコードを作成できます。 有効にする方法を次に示します。

1. **管理者**&#x200B;に移動します。

   ![](assets/admin.png)

1. 「**Salesforce**」をクリックし、「**同期オプションを編集**」をクリックします。

   ![](assets/two-1.png)

1. Salesforceに対してMarketoにプッシュさせるアクティビティの横のチェックボックスをオンにし、「**保存**」をクリックします。

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >一旦有効にすると、Marketoは3ヶ月分のアクティビティ履歴をプッシュします。 データの量によっては、__&#x200B;を完了するのに数日かかる場合があります。 最初のアクティビティのプッシュ中に発生する更新は、最初のアクティビティの同期が完了するまで遅延する可能性があります。

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <thead> 
  <tr> 
   <th>アクティビティタイプ</th> 
   <th>詳細</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>フォーム入力完了</td> 
   <td>任意のMarketoフォームに入力</td> 
  </tr> 
  <tr> 
   <td>リストに追加済み</td> 
   <td><p>フローステップ：静的リストに追加されました</p></td> 
  </tr> 
  <tr> 
   <td>メール送信済み</td> 
   <td>フローステップ：Eメールが送信されました</td> 
  </tr> 
  <tr> 
   <td>メール到着</td> 
   <td>電子メールを受信（バウンスなし）</td> 
  </tr> 
  <tr> 
   <td>メール開封済み</td> 
   <td>電子メールを開きました（画像をブロックしません）</td> 
  </tr> 
  <tr> 
   <td>メール内リンクをクリック済み
</td> 
   <td>Marketoから送信された電子メール内のリンクをクリックしました</td> 
  </tr> 
  <tr> 
   <td>リストから削除済み</td> 
   <td>フローステップ：静的リストから削除されました</td> 
  </tr> 
  <tr> 
   <td>フローから削除</td> 
   <td>フローステップ：フローから削除</td> 
  </tr> 
  <tr> 
   <td>セールスメール送信済み</td> 
   <td>Marketo販売インサイト経由で電子メールが送信されました。</td> 
  </tr> 
  <tr> 
   <td>セールスメール開封済み</td> 
   <td>Marketo・セールス・インサイト経由で送信される電子メールを開きました。</td> 
  </tr> 
  <tr> 
   <td>販売の電子メールのリンクをクリック</td> 
   <td>Marketo販売インサイト経由で送信された電子メール内のリンクをクリックしました</td> 
  </tr> 
  <tr> 
   <td>セールスメール受信済み</td> 
   <td>販売担当者がMSI Outlookプラグインで電子メールを受信し、ログに記録しました</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>&quot;受信した販売の電子メール&quot;が&#x200B;**配信されない**。 Sales Insight経由で送信された電子メールの配信ステータスはキャプチャされません。

>[!TIP]
>
>SalesforceにMarketoの情報をもっと入手したい場合は、[Marketoセールスインサイト](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)製品をご覧ください。
