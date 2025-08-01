---
unique-page-id: 4719294
description: アクティビティ同期のカスタマイズ - Marketo ドキュメント - 製品ドキュメント
title: アクティビティ同期のカスタマイズ
exl-id: 938d83dc-b9b1-41d8-bf98-04548b074ec4
feature: Salesforce Integration
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 84%

---

# アクティビティ同期のカスタマイズ {#customize-activities-sync}

Marketo Sales Insight を使用しない場合、Marketo Engage は特定のイベントに対して Salesforce のアクティビティ履歴レコードを作成できます。有効にする方法は、以下のとおりです。

>[!NOTE]
>
>Salesforce／Marketo Engage の同期では、ユーザが Salesforce にプッシュされる前に発生したアクティビティは Salesforce にプッシュされません。

1. 「**[!UICONTROL Admin]**」に移動します。

   ![](assets/customize-activities-sync-1.png)

1. **[!DNL Salesforce]** をクリックし、「**[!UICONTROL 同期オプションを編集]**」をクリックします。

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
   <td>[!UICONTROL 入力済みフォーム &#x200B;]</td>
   <td>任意の Marketo フォームに入力しました</td>
  </tr>
  <tr>
   <td>[!UICONTROL がリストに追加されました &#x200B;]</td>
   <td><p>フローステップ：静的リストに追加されました</p></td>
  </tr>
  <tr>
   <td>[!UICONTROL 送信済み電子メール &#x200B;]</td>
   <td>フローステップ：メールが送信されました</td>
  </tr>
  <tr>
   <td>[!UICONTROL Email delivered]</td>
   <td>メールを受信しました（バウンスなし）</td>
  </tr>
  <tr>
   <td>[!UICONTROL Email opened]</td>
   <td>メールを開きました（画像ブロックなし）</td>
  </tr>
  <tr>
   <td>[!UICONTROL メール内のクリックされたリンクを]</td>
   <td>Marketo から送信されたメール内のリンクをクリックしました</td>
  </tr>
  <tr>
   <td>[!UICONTROL がリストから削除されました &#x200B;]</td>
   <td>フローステップ：静的リストから削除されました</td>
  </tr>
  <tr>
   <td>[!UICONTROL フローから削除 &#x200B;]</td>
   <td>フローステップ：フローから削除されました</td>
  </tr>
  <tr>
   <td>[!UICONTROL 販売電子メールが送信されました &#x200B;]</td>
   <td>Marketo Sales Insight 経由でメールを送信されました</td>
  </tr>
  <tr>
   <td>[!UICONTROL 販売 E メール開封数 &#x200B;]</td>
   <td>Marketo Sales Insight 経由で送信したメールを開封しました</td>
  </tr>
  <tr>
   <td>[!UICONTROL 販売メール内のクリックリンク &#x200B;]</td>
   <td>Marketo Sales Insight を通じて送信されたメール内のリンクをクリックしました</td>
  </tr>
  <tr>
   <td>[!UICONTROL 販売電子メールを受信 &#x200B;]</td>
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
