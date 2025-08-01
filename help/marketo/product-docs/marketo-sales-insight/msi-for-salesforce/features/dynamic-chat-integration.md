---
description: 動的チャットの統合 - Marketo ドキュメント - 製品ドキュメント
title: 動的チャットの統合
exl-id: b2e3b4da-9ca7-4299-9c50-f52e0de91e36
feature: Marketo Sales Insights
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 43%

---

# 動的チャットの統合 {#dynamic-chat-integration}

Sales Insight と動的チャットの統合について詳しく説明します。

>[!PREREQUISITES]
>
>* 営業Insight SFDC パッケージは、バージョン [2.4.0 以降である必要があります ](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target="_blank"}
>
>* [動的チャットの統合](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md){target="_blank"}セットアップを持っている必要があります。
>
>* Sales Insight[Operational Settings](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.md#operational-settings){target="_blank"} で、「API Secret Key」フィールドに値が入力されていることを確認します。 含まれていない場合は、その取得方法を参照してください [ こちら ](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md#configure-sales-insight-in-marketo){target="_blank"}。

## 「[!DNL Marketo Sales Insight] 設定」タブ {#marketo-sales-insight-configuration-tab}

[!DNL Dynamic Chat] 統合を有効にするには、次の手順に従います。

1. [!DNL Salesforce] アカウントにログインし、タブバーの最後にある「+」をクリックして、「**[!DNL Marketo Sales Insight Config]**」をクリックします。

1. クリックして「[!UICONTROL Visualforce パネル &#x200B;]」を展開します。

   ![](assets/dynamic-chat-integration-1.png)

1. 「**[!UICONTROL 動的チャットデータを有効にする]**」チェックボックスを選択します。

   ![](assets/dynamic-chat-integration-2.png)

## 機能の概要 {#feature-overview}

次の [!DNL Dynamic Chat] アクティビティは、[!DNL Sales Insight] のユーザーが利用できます。

関与したダイアログ：Marketoにログインし、訪問者がチャットボットをクリックしてダイアログに関与すると [!DNL Sales Insight] に入力されます。

* ダイアログ名
* ページ URL
* ステータス（開始済み／離脱済み／完了済み）

スケジュールされた予定：Marketoにログインし、訪問者がチャットボットを使用して予定を正常にスケジュールすると [!DNL Sales Insight] に入力されます。

* ダイアログ名
* エージェント
* ページ URL
* スケジュール日（日付とタイムスタンプを挿入）
* ステータス（スケジュール済み、再スケジュール済み、キャンセル済み）

目標を達成：Marketoにログインし、訪問者がダイアログフローで目標に到達した [!DNL Sales Insight] に入力します。

* ダイアログ名
* 目標名
* ページ URL

ドキュメントとのインタラクション：Marketoにログインし、訪問者がチャットボットを介して共有されたドキュメントとやり取りすると [!DNL Sales Insight] に入力されます。

* ダイアログ名
* ドキュメント
* ステータス

チャットアクティビティは Insights ダッシュボードで利用できます。

![](assets/dynamic-chat-integration-3.png)

「チャット」タブは、リードパネルと取引先責任者パネルで使用できます。[!UICONTROL &#x200B; アクティビティタイプ &#x200B;]、[!UICONTROL &#x200B; ダイアログ名 &#x200B;] および [!UICONTROL &#x200B; 日付 &#x200B;] 列が含まれます。

![](assets/dynamic-chat-integration-4.png)

アクティビティタイプをクリックすると、そのタイプに関する詳細を確認できます。

![](assets/dynamic-chat-integration-5.png)

同様に、アカウントパネルと商談パネルには、[!UICONTROL &#x200B; 名前 &#x200B;]、[!UICONTROL &#x200B; アクティビティタイプ &#x200B;]、[!UICONTROL &#x200B; ダイアログ名 &#x200B;]、[!UICONTROL &#x200B; 日付 &#x200B;] 列が含まれています。

![](assets/dynamic-chat-integration-6.png)

「チャット」タブは、「グローバル Marketo」タブにも表示されます。次の列と共に、3 つのアクティビティタイプ（[!UICONTROL &#x200B; エンゲージメントダイアログ &#x200B;]、[!UICONTROL &#x200B; 予定予定 &#x200B;]、[!UICONTROL &#x200B; 達成目標 &#x200B;]）が含まれます。

* [!UICONTROL &#x200B; 人物 &#x200B;]
* [!UICONTROL アカウント]
* [!UICONTROL &#x200B; アクティビティタイプ &#x200B;] （[!UICONTROL &#x200B; エンゲージメント済みダイアログ &#x200B;]、[!UICONTROL &#x200B; スケジュール済み予定 &#x200B;]、[!UICONTROL &#x200B; 目標達成 &#x200B;]）
* [!UICONTROL &#x200B; ダイアログ名 &#x200B;]
* [!UICONTROL 日付]

ここでも、アクティビティタイプをクリックすると、そのアクティビティの詳細を確認できます。

![](assets/dynamic-chat-integration-7.png)

>[!NOTE]
>
>「[!UICONTROL Dynamic Chat データを有効にする &#x200B;]」チェックボックスが無効になっている場合、次の機能は無効になります。
>
>* Insights ダッシュボードのチャットアクティビティの行（スマートグリッドと週別リスト表示）
>* リード、取引先責任者、アカウント、商談の各パネルの「チャット」タブ
>* 「グローバル Marketo」タブの「チャット」タブ
>
>これらの機能の 1 つのみを無効にすることはできません。
