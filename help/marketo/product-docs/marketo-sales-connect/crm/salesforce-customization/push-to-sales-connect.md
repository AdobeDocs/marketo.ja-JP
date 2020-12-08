---
unique-page-id: 14352477
description: Sales Connectへのプッシュ — Marketto Docs — 製品ドキュメント
title: Sales Connectにプッシュ
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---


# Sales Connectにプッシュ {#push-to-sales-connect}

「Push to Tout」ボタンを押すと、Salesforceのリード/連絡先のリストが表示され、Sales Connectのグループに表示されます。 その後、カスタマイズ可能なグループの電子メールと、トラッキング機能が付加された電子メールをすばやく送信できます。

## 要件 {#requirements}

* Sales Connect [Salesforceパッケージ](http://docs.marketo.com/x/C4PS) 。 `Salesforce Admin`

* `Push to Sales Connect`がリスト表示にインストールするボタン `Salesforce Admin`

* Sales ConnectでSalesforce接続が行われ、ユーザがプッシュを行う

## 使い方 {#how-to}

1. Salesforceの「 **Lead/Contact** 」タブをクリックします。
1. 「Go」ボタンの横の「Push to Sales Connect」にするリスト表示に切り替えます。
1. 「 **移動**」をクリックします。
1. プッシュしてトアウトするすべてのリード/連絡先を選択します。
1. 「 **MSEにプッシュ」を選択します**。
1. プッシュオーバーするリード/連絡先の数を確認する新しいウィンドウが表示されます。 「 **グループに進む**」を選択します。 Sales Connect SalesforceまたはSales Connectでマークされ `will not push over` ている連絡先 `Email Opt Out``Unsubscribed` を接続します。

   >[!NOTE]
   >
   >Sales Connectは、「SFDC-...」という名前のグループを追加します。 を [webアプリケーションのRelationshipsページに追加します](http://toutapp.com/login)。

1. 「 **グループ全体を電子メールで送信」を選択して** 、このグループの電子メールを送信します。

