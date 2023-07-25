---
unique-page-id: 42762409
description: Marketo 管理者向け Sales Insight ページ - Marketo ドキュメント - 製品ドキュメント
title: Marketo 管理者向け Sales Insight ページ
exl-id: d98bc9d8-1a72-405f-b1d7-b71ad88c8493
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 100%

---

# Marketo 管理者向け Sales Insight ページ {#sales-insight-page-for-marketo-admins}

Marketo 管理者には、Sales Insight に関する特定の権限があります。それらについて説明します。

## SOAP API 設定 {#soap-api-configuration}

Salesforce で MSI を使用するために、これらの資格情報を使用して Salesforce アカウントを Marketo インスタンスに接続します。

![](assets/one-1.png)

## Rest API 設定 {#rest-api-configuration}

Salesforce で MSI Insights ダッシュボードを使用するために、これらの資格情報を使用して Salesforce アカウントを Marketo インスタンスに接続します。

![](assets/two-1.png)

## 人物スコア設定 {#person-score-settings}

* **星**：星は、他のリードと比較した合計リードスコアを表します。
* **炎**：炎は緊急度を表し、リードのスコアが最近どの程度変化したかを示します。

デフォルトでは、Marketo Sales Insight は「リードスコア」フィールドを使用して星と炎を計算します。別のフィールドを選択する場合は、次の方法を使用できます。

1. Marketo の&#x200B;**管理者**&#x200B;領域で、「**Sales Insight**」をクリックします。

   ![](assets/four.png)

1. 「リードスコアリング設定」で、「**編集**」をクリックします。

   ![](assets/five.png)

1. 星に使用するフィールドを選択します。

   ![](assets/six.png)

1. 炎に使用するフィールドを選択します。

   ![](assets/seven.png)

1. 「**保存**」をクリックします。Sales Insight の再計算には時間がかかります。後で CRM をチェックして星と炎を確認できます。

   ![](assets/eight.png)

   >[!TIP]
   >
   >カスタムスコアフィールドがまだない場合は、こちらを参照して[作成します](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)。

   >[!MORELIKETHIS]
   >
   >[星と炎](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/customize-stars-and-flames.md)

## 設定 {#settings}

![](assets/nine.png)

**配信停止設定：**

テンプレートなし、標準メール、オペレーショナルメールに対して、次の配信停止設定から選択できます

* 配信停止設定を優先
* 1 人以上の受信者の場合に配信停止設定を優先
* 受信者が 5 人以上の場合に配信停止設定を優先
* 配信停止設定を無視

**テンプレートをロックする機能を有効化：**

有効にすると、Salesforce からメールを送信する際に、MSI ユーザーはテンプレートを編集できなくなります

**RSS フィードの有効化：**

有効にすると、MSI ユーザーは（Salesforce のリードフィードに加えて）RSS フィードでリードフィードを表示できます。RSS フィードは、「トークンの有効期限」機能が無効な場合にのみ機能します。

**トークンの有効期限：**

トークンの有効期限は、機能マネージャーで制御します。有効／無効を切り替えるには、[Marketo サポート](https://nation.marketo.com/t5/Support/ct-p/Support)にお問い合わせください。有効にすると、すべての Marketo トークンは 10 分以内に期限切れになります。無効にすると、Marketo トークンは期限切れになりません。

トークンの有効期限を有効にする前に生成されたトークンについては、認証の有効期限がないため、この機能が現在有効である場合でも期限切れになりません。

トークンの有効期限を有効にした後に生成されたトークンについては、有効期限が 10 分となり、この機能が無効になった後も 10 分で有効期限切れになります。

トークンの動作は、現在の機能のステータスではなく、生成された時点のトークンの有効期限機能が有効／無効であるかに基づきます。
