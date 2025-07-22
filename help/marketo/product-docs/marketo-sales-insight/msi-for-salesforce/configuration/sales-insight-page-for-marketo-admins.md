---
unique-page-id: 42762409
description: Marketo 管理者向け Sales Insight ページ - Marketo ドキュメント - 製品ドキュメント
title: Marketo 管理者向け Sales Insight ページ
exl-id: d98bc9d8-1a72-405f-b1d7-b71ad88c8493
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 62%

---

# Marketo管理者向けの [!DNL Sales Insight] ページ {#sales-insight-page-for-marketo-admins}

Marketo管理者は、[!DNL Sales Insight] で特定の権限を持っています。 それらについて説明します。

## SOAP API 設定 {#soap-api-configuration}

これらの資格情報は、[!DNL Salesforce] で MSI を使用するために、[!DNL Salesforce] アカウントをMarketo インスタンスに接続するために使用されます。

![](assets/one-1.png)

## Rest API 設定 {#rest-api-configuration}

これらの資格情報は、[!DNL Salesforce] の MSI Insights Dashboard を使用するために、[!DNL Salesforce] アカウントをMarketo インスタンスに接続するために使用されます。

![](assets/two-1.png)

## 人物スコア設定 {#person-score-settings}

* **[!UICONTROL 星]**：星は、他のリードと比較した合計リードスコアを表します。
* **[!UICONTROL 炎]**：炎は緊急度を表し、リードのスコアが最近どの程度変化したかを示します。

デフォルトでは、[!DNL Marketo Sales Insight] は「リードスコア」フィールドを使用して星と炎を計算します。 別のフィールドを選択する場合は、次の方法を使用できます。

1. Marketo の&#x200B;**[!UICONTROL 管理者]**&#x200B;領域で、「**[!UICONTROL Sales Insight]**」をクリックします。

   ![](assets/four.png)

1. [!UICONTROL &#x200B; リードスコアリング設定 &#x200B;] で、「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/five.png)

1. 星に使用するフィールドを選択します。

   ![](assets/six.png)

1. 炎に使用するフィールドを選択します。

   ![](assets/seven.png)

1. 「**[!UICONTROL 保存]**」をクリックします。Sales Insight の再計算には時間がかかります。後で CRM をチェックして星と炎を確認できます。

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

[!UICONTROL &#x200B; テンプレートなし &#x200B;]、[!UICONTROL &#x200B; 標準メール &#x200B;] および [!UICONTROL &#x200B; 運用メール &#x200B;] に対して、次の購読解除設定から選択できます

* [!UICONTROL &#x200B; 購読解除設定に従う &#x200B;]
* [!UICONTROL &#x200B; 複数の受信者の場合は購読解除設定に従う &#x200B;]
* [!UICONTROL 5 人を超える受信者が登録した場合は購読解除の設定に従う &#x200B;]
* [!UICONTROL &#x200B; 購読解除設定を無視 &#x200B;]

**テンプレートをロックする機能を有効化：**

有効化すると、MSI ユーザーは [!DNL Salesforce] からのメールの送信中にテンプレートを編集できなくなります

**RSS フィードの有効化：**

有効化すると、MSI ユーザーは、[!DNL Salesforce] のリードフィードに加えて、RSS フィードでリードフィードを表示できます。 「[!UICONTROL &#x200B; トークンの有効期限 &#x200B;]」機能が無効になっている場合にのみ、RSS フィードが機能します。

**トークンの有効期限：**

トークンの有効期限は、機能マネージャーで制御します。有効／無効を切り替えるには、[Marketo サポート](https://nation.marketo.com/t5/Support/ct-p/Support)にお問い合わせください。有効にすると、すべての Marketo トークンは 10 分以内に期限切れになります。無効にすると、Marketo トークンは期限切れになりません。

トークンの有効期限を有効にする前に生成されたトークンについては、認証の有効期限がないため、この機能が現在有効である場合でも期限切れになりません。

トークンの有効期限を有効にした後に生成されたトークンについては、有効期限が 10 分となり、この機能が無効になった後も 10 分で有効期限切れになります。

トークンの動作は、現在の機能のステータスではなく、生成された時点のトークンの有効期限機能が有効／無効であるかに基づきます。
