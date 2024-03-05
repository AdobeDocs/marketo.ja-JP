---
unique-page-id: 2360368
description: Salesforce Enterprise/Unlimited エディションでMarketo Sales Insight を設定する方法を説明します。
title: Salesforce Enterprise／Unlimited での Marketo Sales Insight の設定
exl-id: a33ed396-8d26-403f-b6d8-fe7c55ce76ba
feature: Marketo Sales Insights
source-git-commit: 3cbefabe80778b0502eaecd733b5732fd9003316
workflow-type: tm+mt
source-wordcount: '885'
ht-degree: 39%

---

# Salesforce Enterprise／Unlimited での Marketo Sales Insight の設定 {#configure-marketo-sales-insight-in-salesforce-enterprise-unlimited}

以下の手順を実行して、Salesforce Enterprise/Unlimited エディションでMarketo Sales Insight を設定します。

>[!PREREQUISITES]
>
>[Salesforce AppExchange での Marketo Sales Insight パッケージのインストール](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)

>[!NOTE]
>
>**管理者権限が必要です。**

## Sales Insight のMarketo Engage {#configure-sales-insight-in-marketo}

1. Marketo Sales Insight の資格情報をMarketo Engageで取得するには、 **[!UICONTROL 管理者]** 領域と選択 **[!UICONTROL Sales Insight]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1.png)

1. 「**[!UICONTROL API 設定を編集]**」をクリックします。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2.png)

1. 任意の API 秘密鍵を入力し、「**[!UICONTROL 保存]**」をクリックします。アンパサンド (`&`) を API 秘密鍵に置き換えます。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3.png)

   >[!NOTE]
   >
   >API 秘密鍵は組織のパスワードのようなもので、セキュリティで保護されている必要があります。

1. 資格情報を入力するには、 **[!UICONTROL 表示]** （内） _[!UICONTROL Rest API 設定]_ パネル。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4.png)

1. 確認ダイアログが表示されたら、「 **[!UICONTROL OK]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5.png)

   >[!TIP]
   >
   >このウィンドウは開いたままにしておきます。この情報は後で Salesforce 設定に必要になります。

## Salesforce での Sales Insight の設定 {#configure-sales-insight-in-salesforce}

1. Salesforce で、「**[!UICONTROL 設定]**」をクリックします。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6.png)

1. 「リモートサイト」を検索し、「**[!UICONTROL リモートサイトの設定]**」を選択します。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7.png)

1. 「**[!UICONTROL 新規リモートサイト]**」をクリックします。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8.png)

1. リモートサイト名を入力します（次のように指定できます）。 `MarketoSoapAPI`) をクリックします。 リモートサイトの URL を入力します。これは、 _[!UICONTROL SOAP API 設定]_ パネルをMarketo Engage。 「**[!UICONTROL 保存]**」をクリックします。これで、Soap API 用のリモートサイト設定が作成されました。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9.png)

1. もう一度「**[!UICONTROL 新規リモートサイト]**」をクリックします。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10.png)

1. リモートサイト名を入力します（次のように指定できます）。 `MarketoAPI`) をクリックします。 リモートサイト URL(API URL: ) を入力します。 _[!UICONTROL Rest API 設定]_ パネルをMarketo Engage。 「**[!UICONTROL 保存]**」をクリックします。Rest API 用のリモートサイト設定が作成されました。

   >[!NOTE]
   >
   >_あなた_ を選択します。 **[!UICONTROL リモートサイト名]** (`MarketoAPI` はここで使用されます )。 The **[!UICONTROL リモートサイトの URL]** は、「Marketoでの Sales Insight の設定」セクションの手順 3 の「API 設定を編集」ダイアログの「Marketoホスト」フィールドにあります。

## Sales Insight ユーザーに標準の Salesforce オブジェクトへのプロファイルアクセスを許可する {#grant-sales-insight-users-profile-access}

Salesforce のセキュリティ強化により、AppExchangeパッケージは標準オブジェクトに権限を付与できなくなり、Salesforce ユーザーのプロファイルから関連する Salesforce オブジェクトにアクセス権を付与する必要があります。 必要な権限を付与するには、次の手順に従います。

1. 「**[!UICONTROL 設定]**」をクリックします。

1. クイック検索で「プロファイル」を検索します。

1. クリック **[!UICONTROL 編集]** をクリックします。

1. の下 _[!UICONTROL 標準オブジェクト権限]_ セクション、有効 **[!UICONTROL 読み取り]** 次のオブジェクトへのアクセス： [!UICONTROL リード], [!UICONTROL 連絡先], [!UICONTROL アカウント]、および [!UICONTROL 商談].

1. 「**[!UICONTROL 保存]**」をクリックします。

## ページレイアウトのカスタマイズ {#customize-page-layouts}

1. 「**[!UICONTROL 設定]**」をクリックします。

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. 「ページレイアウト」を検索し、「**[!UICONTROL リード]**」の下の「**[!UICONTROL ページレイアウト]**」を選択します。

   ![](assets/image2015-5-28-14-3a58-3a39.png)

1. 左側の「**[!UICONTROL Visualforce Pages]**」をクリックします。ドラッグ **[!UICONTROL セクション]** を _[!UICONTROL カスタムリンク]_ 」セクションに入力します。

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. として「Marketo Sales Insight」と入力します。 **[!UICONTROL セクション名]**&#x200B;を選択します。 **[!UICONTROL 1 列]**&#x200B;をクリックし、 **[!UICONTROL OK]**.

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. 「**[!UICONTROL リード]**」を新しいセクションにドラッグ＆ドロップします。

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   >
   >このボックスの名前は、オブジェクトの種類に応じて変わります。 例えば、連絡先のページレイアウトを変更する場合、連絡先と表示されます。

1. 次をダブルクリックします。 **[!UICONTROL リード]** ブロックを追加しました。

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. 高さを **450** ピクセルに編集し、「**[!UICONTROL OK]**」をクリックします。

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!NOTE]
   >
   >スクロールを使用してアクティビティにアクセスする必要がある場合は、「**[!UICONTROL スクロールバーを表示]**」をチェックします。

   >[!TIP]
   >
   >Accounts オブジェクトと Opportunity オブジェクトの推奨高さは 410 ピクセルです。

1. クリック **[!UICONTROL フィールド]** 左側に 次に、「**[!UICONTROL 緊急度]**」ラベルを検索して、**[!UICONTROL Marketo Sales Insight]** レイアウトにドラッグします。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-18.png)

1. これらのフィールドに対しても、上記の手順を繰り返します。

   * 最新の注目のアクション
   * 最新の注目のアクション発生日
   * 最新の注目のアクションの詳細
   * 最新の注目のアクションのソース
   * 最新の注目のアクションのタイプ
   * セールス別の最後のアクティビティ
   * セールス別の最後のエンゲージメント
   * MSI 取引先責任者 ID
   * 相対スコア
   * 相対スコア値
   * 緊急度
   * 緊急度の値
   * Marketo 内に表示

1. 終了したら「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. 手順 5～7 を繰り返して、次の用の Visualforce ページセクションと Sales Insight フィールドを追加します。 **[!UICONTROL 連絡先]**, **[!UICONTROL アカウント]**、および **[!UICONTROL 商談]**.

1. 手順 8 ～ 10 を繰り返して、次の Sales Insight フィールドを **[!UICONTROL 連絡先]**. 変更したら必ず保存します。

   * 最新の注目のアクション
   * 最新の注目のアクション発生日
   * [!UICONTROL 最新の注目のアクションの詳細]
   * [!UICONTROL 最新の注目のアクションのソース]
   * [!UICONTROL 最新の注目のアクションのタイプ]
   * [!UICONTROL セールス別の最後のMarketoアクティビティ]
   * [!UICONTROL セールス別の最後のMarketoエンゲージメント]
   * [!UICONTROL MKTO リードスコア]
   * [!UICONTROL 相対スコア]
   * [!UICONTROL 相対スコア値]
   * [!UICONTROL Sales Insight]  — 連絡先の完全なリストページを開きます
   * [!UICONTROL 緊急度]
   * [!UICONTROL 緊急度の値]

## カスタムユーザフィールドのマッピング {#map-custom-person-fields}

変換が正しく機能するように、Marketoの担当者フィールドを Salesforce の連絡先フィールドにマッピングする必要があります。 次の手順に従って、マップします。

1. 「**[!UICONTROL 設定]**」をクリックします。

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. 検索バーで「フィールド」を検索し、「**[!UICONTROL リード]**」の下の「**[!UICONTROL フィールド]**」をクリックします。

   ![](assets/image2015-6-1-9-3a54-3a50.png)

1. 「**[!UICONTROL リードフィールドをマッピング]**」をクリックします。

   ![](assets/image2015-6-1-9-3a58-3a48.png)

1. 右側のドロップダウンをクリックし、 **[!UICONTROL エンゲージメント]**.

   ![](assets/image2015-6-1-10-3a9-3a53.png)

1. リストから「**[!UICONTROL 取引先責任者、エンゲージメント]**」を選択します。

   ![](assets/image2015-6-1-10-3a12-3a11.png)

1. 上の手順を繰り返して、以下のフィールドもマッピングします。

   | Marketo の人物のカスタムフィールド | Salesforce の取引先責任者のカスタムフィールド |
   |--- |--- |
   | `Engagement` | `Contact.Engagement` |
   | `Relative Score Value` | `Contact.Relative Score Value` |
   | `Urgency Value` | `Contact.Urgency Value` |
   | `Last Interesting Moment Date` | `Contact.Last Interesting Moment Date` |
   | `Last Interesting Moment Desc` | `Contact.Last Interesting Moment Desc` |
   | `Last Interesting Moment Source` | `Contact.Last Interesting Moment Source` |
   | `Last Interesting Moment Type` | `Contact.Last Interesting Moment Type` |

1. 完了したら、「**[!UICONTROL 保存]**」をクリックします。

## Marketo Sales Insight の「設定」タブ {#marketo-sales-insight-configuration-tab}

1. Salesforce で、タブバーの最後にある「**+**」をクリックし、「**[!UICONTROL Marketo Sales Insight の設定]**」をクリックします。

1. の Soap API パネルから資格情報をコピーします。[Marketo Sales Insight 管理ページ](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"}をクリックし、Salesforce Sales Insight 設定ページの「SOAP API」セクションに貼り付けます。

1. の Rest API パネルから資格情報をコピーします。[Marketo Sales Insight 管理ページ](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"}をクリックし、Salesforce Sales Insight 設定ページの Rest API セクションに貼り付けます。

   ![](assets/configure-marketo-sales-insight-in-salesforce-enterprise-edition-25.png)

リード、連絡先、アカウント、商談のMarketo Sales Insight フィールドが表示されます。

>[!NOTE]
>
>診断テストに失敗した場合は、 [ページレイアウトへのフィールドの追加](https://nation.marketo.com:443/t5/knowledgebase/how-to-repair-marketo-sales-insight-setup-configuration-problems/ta-p/248218){target="_blank"} 問題が修正される可能性があります。

>[!NOTE]
>
>アカウントの場合、Sales Insight にはすべてのメールが含まれますが、最新の注目のアクション、Web アクティビティ、スコアの変更のみが含まれます。

>[!MORELIKETHIS]
>
>* [優先度、緊急度、相対スコア、最有望見込客](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md)
>* [Salesforce への「Marketo」タブの追加](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-marketo-tab-to-salesforce.md)
>* [Sales Insight へのアクセスをプロファイルに追加](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"}
