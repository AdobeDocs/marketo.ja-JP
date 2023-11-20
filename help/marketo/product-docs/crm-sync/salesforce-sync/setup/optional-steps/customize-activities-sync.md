---
unique-page-id: 4719294
description: アクティビティ同期のカスタマイズ - Marketo ドキュメント - 製品ドキュメント
title: アクティビティ同期のカスタマイズ
exl-id: 938d83dc-b9b1-41d8-bf98-04548b074ec4
feature: Salesforce Integration
source-git-commit: 756a38ba87dd5af9ee783e9709056d444d4f415b
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 93%

---

# アクティビティ同期のカスタマイズ {#customize-activities-sync}

Marketo Sales Insight を使用しない場合、Marketo Engageは特定のイベントに対して Salesforce アクティビティ履歴レコードを作成できます。 有効にする方法は、以下のとおりです。

1. 「**[!UICONTROL 管理]**」に移動します。

   ![](assets/admin.png)

1. **[!DNL Salesforce]**／**[!UICONTROL 同期オプションの編集]**&#x200B;をクリックします。

   ![](assets/two-1.png)

1. Marketo で Salesforce にプッシュするアクティビティの横にあるチェックボックスをオンにして、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >有効化すると、Marketo は 3 か月分のアクティビティ履歴をプッシュします。データの量に応じて、_これには数日かかる場合があります_。アクティビティの初回プッシュ中に発生したアップデートは、アクティビティの初回同期が完了するまで遅延する場合があります。

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <thead> 
  <tr> 
   <th>アクティビティのタイプ</th> 
   <th>説明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>フォーム入力完了</td> 
   <td>任意の Marketo フォームに入力しました</td> 
  </tr> 
  <tr> 
   <td>リストに追加済み</td> 
   <td><p>フローステップ：静的リストに追加されました</p></td> 
  </tr> 
  <tr> 
   <td>メール送信済み</td> 
   <td>フローステップ：メールが送信されました</td> 
  </tr> 
  <tr> 
   <td>メール到着</td> 
   <td>メールを受信しました（バウンスなし）</td> 
  </tr> 
  <tr> 
   <td>メール開封済み</td> 
   <td>メールを開きました（画像ブロックなし）</td> 
  </tr> 
  <tr> 
   <td>メール内リンクをクリック済み
</td> 
   <td>Marketo から送信されたメール内のリンクをクリックしました</td> 
  </tr> 
  <tr> 
   <td>リストから削除済み</td> 
   <td>フローステップ：静的リストから削除されました</td> 
  </tr> 
  <tr> 
   <td>フローからの削除み</td> 
   <td>フローステップ：フローから削除されました</td> 
  </tr> 
  <tr> 
   <td>セールスメール送信済み</td> 
   <td>Marketo Sales Insight 経由でメールを送信されました</td> 
  </tr> 
  <tr> 
   <td>セールスメール開封済み</td> 
   <td>Marketo Sales Insight 経由で送信したメールを開封しました</td> 
  </tr> 
  <tr> 
   <td>セールスメール内のリンクをクリック</td> 
   <td>Marketo Sales Insight を通じて送信されたメール内のリンクをクリックしました</td> 
  </tr> 
  <tr> 
   <td>セールスメール受信済み</td> 
   <td>MSI Outlook プラグインでセールス担当者がメールを受信し、ログに記録しました</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>「セールスメール受信済み」は、配達済みとは&#x200B;_違います_。Sales Insight 経由で送信されたメールの配信ステータスはキャプチャされません。

>[!TIP]
>
>Marketo の情報を更に Salesforce に追加することに関心がある場合は、[Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"} 製品をご確認ください。
