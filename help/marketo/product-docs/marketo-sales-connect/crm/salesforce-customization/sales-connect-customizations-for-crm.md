---
unique-page-id: 14745793
description: CRM用のSales Connectのカスタマイズ — Marketto Docs — 製品ドキュメント
title: CRM向けの販売接続のカスタマイズ
translation-type: tm+mt
source-git-commit: 07ae1b3f3ee3e9d7f35373eea039d336bd786f97
workflow-type: tm+mt
source-wordcount: '641'
ht-degree: 0%

---


# CRM用のSales Connectのカスタマイズ{#sales-connect-customizations-for-crm}

以下のフィールドとボタンは、Salesforce CRMのメタデータAPIによって作成されます。 フィールドを作成したら、管理者はCRMにページレイアウトを設定して、それらを公開する必要があります。 説明は[ここ](http://docs.marketo.com/display/docs/assets/marketo-sales-engage-for-salesforce-installation-and-success-guide.pdf)にあります。

>[!NOTE]
>
>これは、ToutAppとSales Connectの両方のお客様に影響を与えます。

## Salesforceでのカスタマイズのインストール方法{#how-to-install-customizations-in-salesforce}

1. 「Sales Connect」で、歯車アイコンをクリックし、「**設定**」を選択します。

   ![](assets/one.png)

1. 「管理設定」で、「**Salesforce**」を選択します。

   ![](assets/two.png)

1. **Marketto Sales Connect Customizations**&#x200B;をクリックします。

   ![](assets/three.png)

1. **Salesforce**&#x200B;に接続をクリックします。

   ![](assets/four.png)

1. Salesforceにログインします。

   ![](assets/five.png)

## カスタムアクティビティフィールド{#custom-activity-fields}

Marketorは、新しいフィールドの作成を検出し、1回限りのデータのバックフィル、再マッピング、および&#x200B;**新しい**&#x200B;フィールドへの値の継続的な同期を実行します。 古いフィールドは更新されません。

| **フィールド名** | **説明** |
|---|---|
| MSE Call Local Presence ID | ユーザーは、MSE Phoneからの呼び出し時に、「ローカルプレゼンス」をオプションとして選択できます。 着信呼び出しは、受信者のローカル番号を表示します。 |
| MSE呼び出し記録URL | 呼び出しを記録し、記録のリンクをここに記録できます。 |
| MSEキャンペーン | 連絡先/リードが属するMSEキャンペーンの名前をログに記録します。 |
| MSEキャンペーンURL | MSEで作成されたキャンペーンのURLをログに記録します。 これをクリックすると、MSE Webアプリでキャンペーンが開きます。 |
| MSEキャンペーンの現在の手順 | 連絡先/リードがキャンペーンの一部である場合、このフィールドには、リード/担当者が現在オンにしているステップの名前が記録されます。 |
| MSE電子メール添付ファイルの表示 | 電子メールが添付ファイルと共に送信され、添付ファイルが受信者によって表示された場合に、データをログに記録します。 |
| MSE電子メールがクリックされました | 受信者が電子メール内のリンクをクリックしたときにチェックマークを記録します。 |
| MSE電子メール返信済み | 受信者が電子メールに返信したときにチェックマークを記録します。 |
| MSE電子メールの状態 | 電子メールが送信、処理中、またはバウンス済みかどうかを表示します(バウンスされた電子メールの追跡は、使用する配信のチャネルに応じて異なります)。 |
| MSE電子メールテンプレート | リード/連絡先に送信された電子メールで使用されたMSEテンプレートのログ名です。 |
| MSE電子メールテンプレートURL | MSEで作成されたテンプレートのURLをログに記録します。 これをクリックすると、MSE Webアプリでテンプレートが開きます。 |
| MSE電子メールURL | このURLをクリックすると、MSEのコマンドセンターが開き、[人物の詳細表示の履歴]タブが展開され、送信された電子メールが表示されます。 |
| MSE電子メールの表示 | 受信者が電子メールを表示したときにチェックマークを記録します。 |

## ロールアップログのフィールド{#roll-up-logging-fields}

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>フィールド名</strong></td> 
   <td><strong>説明</strong></td> 
  </tr> 
  <tr> 
   <td>MSE — 最後のマーケティングエンゲージメント</td> 
   <td>マーケティングからの最後の着信エンゲージメント。 </td> 
  </tr> 
  <tr> 
   <td>MSE — 最終マーケティングエンゲージメント日</td> 
   <td>マーケティングからのエンゲージメントのタイムスタンプ。</td> 
  </tr> 
  <tr> 
   <td>MSE — 最後のマーケティングエンゲージメントの説明</td> 
   <td>エンゲージメントの説明。</td> 
  </tr> 
  <tr> 
   <td>MSE — 最後のマーケティングエンゲージメントソース</td> 
   <td>マーケティングエンゲージメントのソース。</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE — 最後のマーケティングエンゲージメントのタイプ</td> 
   <td colspan="1">アクションのタイプ。</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE — 販売別最終アクティビティ<br></td> 
   <td colspan="1">営業チームが実行した最後の発信アクティビティ。</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE — 最後の返信</td> 
   <td colspan="1">販売の電子メールに対する最後の電子メールの返信</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE — 現在の販売キャンペーン</td> 
   <td colspan="1">リード/連絡先が所属するMSEキャンペーンの名前をログに記録します。</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE — 最終販売エンゲージメント</td> 
   <td colspan="1">販売からの最後の関与。 </td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE -オプトアウト</td> 
   <td colspan="1">オプトアウトフィールド。</td> 
  </tr> 
 </tbody> 
</table>

## ボタン{#buttons}

| **ボタン名** | **説明** |
|---|---|
| MSE電子メールの送信 | Salesforceから販売の電子メールを送信します。 |
| MSE追加キャンペーン | をSalesforceの追加MSEキャンペーンに送信します。 |
| MSEにプッシュ | SalesforceからMSEに連絡を取る。 |
| MSEでの通話 | Salesforceからの販売呼び出し。 |

## バルクアクションボタン{#bulk-action-buttons}

| **ボタン名** | **説明** |
|---|---|
| MSE追加キャンペーン | をSalesforceの追加MSEキャンペーンに送信します。 |
| MSEにプッシュ | SalesforceからMSEに連絡を取る。 |

## ユーザーガイド{#user-guides}

[SalesforceのMSEカスタムレポート](http://docs.marketo.com/display/docs/assets/mse-custom-reports-in-sf.docx)

[Salesforce用MSE](http://docs.marketo.com/display/docs/assets/mse-for-sf-classic.pdf)

[Salesforce Lightning用MSE](http://s3.amazonaws.com/tout-user-store/salesforce/assets/SF+Guide+for+Lightning.pdf)

## 関連ビデオ{#related-videos}

**Salesforce**
`<iframe width="630" height="470" src="//play.vidyard.com/YEPWYBfFEa4nKCo2F6bKKc.html?v=3.1.1" frameborder="0" allowfullscreen></iframe>` **でのカスタマイズのインストール方法Salesforce**でのカスタマイズを使用する利点 
`<iframe width="630" height="470" src="//play.vidyard.com/4PzSDb6o8Qg8WbvBsq8wJD.html?v=3.1.1" frameborder="0" allowfullscreen></iframe>`