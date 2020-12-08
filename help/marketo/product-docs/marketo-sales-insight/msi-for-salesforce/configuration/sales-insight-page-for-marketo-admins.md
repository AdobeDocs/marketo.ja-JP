---
unique-page-id: 42762409
description: マーケティング担当者向けのSales Insightページ — Marketto Docs — 製品ドキュメント
title: マーケティング担当者向けのSales Insightページ
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---


# マーケティング担当者向けのSales Insightページ {#sales-insight-page-for-marketo-admins}

マーケティング担当者の管理者は、Sales Insightの特定の権限を持っています。 以下の内容を学びます。

## Soap APIの設定 {#soap-api-configuration}

これらの資格情報は、SalesforceのMSIを使用するために、SalesforceアカウントをMarketoのインスタンスに接続するために使用されます。

![](assets/one-1.png)

## REST APIの設定 {#rest-api-configuration}

これらの資格情報は、SalesforceのMSI Insightsダッシュボードを使用するために、SalesforceアカウントをMarketoのインスタンスに接続するために使用されます。

![](assets/two-1.png)

SFDCでRest API証明書を削除し、Soap APIのみを使用するように選択できます。 これにより、インサイトダッシュボードが無効になります

![](assets/three-1.png)

## 人物スコアの設定 {#person-score-settings}

| **星：** | 星は、他のリードと比較したリードスコアの合計を表します。 |
|---|---|
| **炎：** | 炎は緊急性を表し、最近リードのスコアがどの程度変更されたかを示します。 |

デフォルトでは、Marketo Sales Insightは、「Lead Score」フィールドを使用して星と炎を計算します。 しかし、別のフィールドを選択する場合は、次のようにします。

1. Marketorの **管理者** 領域で、「 **Sales Insight**」をクリックします。

   ![](assets/four.png)

1. 「リードスコアリング設定」で、「 **編集**」をクリックします。

   ![](assets/five.png)

1. 星に使用するフィールドを選択します。

   ![](assets/six.png)

1. 炎に使用するフィールドを選択します。

   ![](assets/seven.png)

1. 「 **保存**」をクリックします。 販売インサイトの再計算には、多少時間がかかります。 CRMを後で確認して、星や炎を確認できます。

   ![](assets/eight.png)

   >[!TIP]
   >
   >カスタムスコアフィールドをまだ持っていない場合は、次の方法で [作成します](http://docs.marketo.com/x/3wMk)。

   >[!NOTE]
   >
   >**関連記事**
   >
   >
   >[星と炎](http://docs.marketo.com/x/qgU6Ag)

## 設定 {#settings}

![](assets/nine.png)

**登録解除設定：**

テンプレートなし、標準電子メール、および運用電子メールに対する次の登録解除設定から選択できます

* 登録解除設定を優先
* 2つ以上の受信者の場合に登録解除設定を適用
* 5受信者以上の場合に登録解除設定を適用
* 登録解除設定を無視

**テンプレートのロック機能を有効にする：**

有効にすると、MSIユーザーはSalesforceからの電子メールの送信中にテンプレートを編集できなくなります

**RSSフィードを有効にする：**

有効にすると、MSIユーザーは（Salesforceのリードフィードに加えて）RSSフィードにリードフィードを表示できます&#x200B;**。**
