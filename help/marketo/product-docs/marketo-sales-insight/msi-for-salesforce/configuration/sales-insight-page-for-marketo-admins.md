---
unique-page-id: 42762409
description: Marketo管理者向けのSales Insight ページについて説明します。 アクション設定とMSI設定にアクセスします。
title: Marketo 管理者向けセールスインサイトページ
exl-id: d98bc9d8-1a72-405f-b1d7-b71ad88c8493
feature: Marketo Sales Insights
TQID: 'https://experienceleague.adobe.com/FTOgWRDvY14tovIUclyWrED5DBXcHXH8APcprG-DlK4'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
    internal-label: Configuration
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
    internal-label: Templates
  - id: 62f69a42-2389-532a-9af6-0e08fdaa397f
    internal-label: Marketo Sales Insights
topic_v2:
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 96%
---
# Marketo 管理者向け [!DNL Sales Insight] ページ {#sales-insight-page-for-marketo-admins}

Marketo 管理者には、[!DNL Sales Insight] に関する特定の権限があります。 それらについて説明します。

## SOAP API 設定 {#soap-api-configuration}

[!DNL Salesforce] で MSI を使用するには、これらの資格情報を使用して [!DNL Salesforce] アカウントを Marketo インスタンスに接続します。

![](assets/one-1.png)

## Rest API 設定 {#rest-api-configuration}

[!DNL Salesforce] で MSI Insights ダッシュボードを使用するには、これらの資格情報を使用して [!DNL Salesforce] アカウントを Marketo インスタンスに接続します。

![](assets/two-1.png)

## 人物スコア設定 {#person-score-settings}

* **[!UICONTROL 星]**：星は、他のリードと比較した合計リードスコアを表します。
* **[!UICONTROL 炎]**：炎は緊急度を表し、リードのスコアが最近どの程度変化したかを示します。

デフォルトでは、[!DNL Marketo Sales Insight] は「リードスコア」フィールドを使用して星と炎を計算します。 別のフィールドを選択する場合は、次の方法を使用できます。

1. Marketo の&#x200B;**[!UICONTROL 管理者]**&#x200B;領域で、「**[!UICONTROL セールスインサイト]**」をクリックします。

   ![](assets/four.png)

1. 「[!UICONTROL リードスコアリング設定]」で、「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/five.png)

1. 星に使用するフィールドを選択します。

   ![](assets/six.png)

1. 炎に使用するフィールドを選択します。

   ![](assets/seven.png)

1. 「**[!UICONTROL 保存]**」をクリックします。 セールスインサイトの再計算には時間がかかります。 後で CRM をチェックして星と炎を確認できます。

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

[!UICONTROL テンプレートなし]、[!UICONTROL 標準メール]、[!UICONTROL オペレーショナルメール]に対して、次の登録解除設定から選択できます。

* [!UICONTROL 登録解除設定を優先]
* [!UICONTROL 1 人以上の受信者の場合に登録解除設定を優先]
* [!UICONTROL 受信者が 5 人以上の場合に登録解除設定を優先]
* [!UICONTROL 登録解除設定を無視]

**テンプレートをロックする機能を有効化：**

有効にすると、[!DNL Salesforce] からメールを送信する際に、MSI ユーザはテンプレートを編集できなくなります

**RSS フィードの有効化：**

有効にすると、MSI ユーザは（[!DNL Salesforce] のリードフィードに加えて）RSS フィードでリードフィードを表示できます。 RSS フィードは、「[!UICONTROL トークンの有効期限]」機能が無効な場合にのみ機能します。

**トークンの有効期限：**

トークンの有効期限は、機能マネージャーで制御します。 有効／無効を切り替えるには、[Marketo サポート](https://nation.marketo.com/t5/Support/ct-p/Support)にお問い合わせください。 有効にすると、すべての Marketo トークンは 10 分以内に期限切れになります。 無効にすると、Marketo トークンは期限切れになりません。

トークンの有効期限機能を有効にする前に生成されたトークンには、有効期限が設定されていないため、この機能が現在有効であっても期限切れになりません。

トークンの有効期限機能を有効にした後に生成されたトークンには 10 分の有効期限が設定されるため、この機能を無効にした後でも 10 分で期限切れになります。

トークンの動作は、現在の機能ステータスではなく、そのトークンが生成された時点でトークンの有効期限機能が有効か無効かに基づきます。
