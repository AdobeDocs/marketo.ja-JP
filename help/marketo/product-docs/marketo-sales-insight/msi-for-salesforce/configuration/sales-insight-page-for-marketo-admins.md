---
unique-page-id: 42762409
description: Marketo管理者向けのSales Insightページ —Marketoドキュメント — 製品ドキュメント
title: Marketo管理者向けのSales Insightページ
exl-id: d98bc9d8-1a72-405f-b1d7-b71ad88c8493
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 3%

---

# Marketo管理者向けのSales Insightページ{#sales-insight-page-for-marketo-admins}

Marketo管理者は、Sales Insightの特定の権限を持っています。 以下の内容を学びます。

## SOAP API設定{#soap-api-configuration}

これらの資格情報は、SalesforceのMSIを使用するために、SalesforceアカウントをMarketoインスタンスに接続するために使用されます。

![](assets/one-1.png)

## REST APIの設定{#rest-api-configuration}

これらの資格情報は、SalesforceでMSI Insightsダッシュボードを使用するために、SalesforceアカウントをMarketoインスタンスに接続するために使用されます。

![](assets/two-1.png)

SFDCでRest API証明書を削除し、Soap APIのみを使用するように選択できます。 これにより、インサイトダッシュボードが無効になります

![](assets/three-1.png)

## 人物スコアの設定{#person-score-settings}

* **星**:星は、他のリードと比較したリードスコアの合計を表します。
* **炎**:炎は緊急性を表し、最近リードのスコアがどの程度変更されたかを示します。

デフォルトでは、Marketo販売インサイトは、「リードスコア」フィールドを使用して星と炎を計算します。 しかし、別のフィールドを選択する場合は、次のようにします。

1. Marketoの&#x200B;**管理者**&#x200B;領域で、**販売インサイト**&#x200B;をクリックします。

   ![](assets/four.png)

1. 「リードスコアリング設定」で、「**編集**」をクリックします。

   ![](assets/five.png)

1. 星に使用するフィールドを選択します。

   ![](assets/six.png)

1. 炎に使用するフィールドを選択します。

   ![](assets/seven.png)

1. 「**保存**」をクリックします。 販売インサイトの再計算には、多少時間がかかります。 CRMを後で確認して、星や炎を確認できます。

   ![](assets/eight.png)

   >[!TIP]
   >
   >カスタムスコアフィールドをまだ持っていない場合は、次のようにして[作成します](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)。

   >[!MORELIKETHIS]
   >
   >[星と炎](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/customize-stars-and-flames.md)

## 設定 {#settings}

![](assets/nine.png)

**配信停止設定:**

テンプレートなし、標準電子メール、および運用電子メールに対する次の登録解除設定から選択できます

* 登録解除設定を優先
* 1つ以上の受信者の場合に登録解除設定を適用
* 5受信者以上の場合に登録解除設定を適用
* 配信停止設定を無視

**テンプレートをロックする機能を有効化:**

有効にすると、MSIユーザーはSalesforceからの電子メールの送信中にテンプレートを編集できなくなります

**RSS フィードの有効化:**

有効にすると、MSIユーザーは（Salesforceのリードフィードに加えて）RSSフィードにリードフィードを表示できます。 RSSフィードは、「トークン有効期限」機能が無効になっている場合にのみ機能します。

**トークンの有効期限:**

トークンの有効期限は、機能マネージャで制御します。 有効/無効にするには、[Marketoサポート](https://nation.marketo.com/t5/Support/ct-p/Support)にご連絡ください。 有効にすると、すべてのMarketoトークンは10分以内に期限切れになります。 無効にすると、Marketoトークンは期限切れになりません。

トークンの有効期限を有効にする前に生成されたトークンには、検証の有効期限がないので、その機能が現在有効になっている場合でも期限は切れません。

トークンの有効期限を有効にした後に生成されるトークンの有効期限は10分なので、この機能を無効にした後も10分で期限が切れます。

トークンの動作は、生成されたタイミング（トークンの有効期限機能が有効/無効になった場合）に基づき、現在の機能のステータスではなくなります。
