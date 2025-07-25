---
unique-page-id: 2360368
description: Salesforce Enterprise／Unlimited エディションでの Marketo Sales Insight の設定方法について説明します。
title: Salesforce Enterprise／Unlimited での Marketo Sales Insight の設定
exl-id: a33ed396-8d26-403f-b6d8-fe7c55ce76ba
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '867'
ht-degree: 90%

---

# [!DNL Marketo Sales Insight] Enterprise/Unlimited での [!DNL Salesforce] の設定 {#configure-marketo-sales-insight-in-salesforce-enterprise-unlimited}

次の手順を実行して、Salesforce Enterprise／Unlimited エディションで Marketo Sales Insight を設定します。

>[!PREREQUISITES]
>
>[Install [!DNL Marketo Sales Insight] Package in [!DNL Salesforce] AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)

>[!NOTE]
>
>**管理者権限が必要です。**

## Marketo Engage での Sales Insight の設定 {#configure-sales-insight-in-marketo}

1. Marketo Engage で Marketo Sales Insight 資格情報を取得するには、**[!UICONTROL 管理者]**&#x200B;領域に移動し、「**[!UICONTROL Sales Insight]**」を選択します。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1.png)

1. 「**[!UICONTROL API 設定を編集]**」をクリックします。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2.png)

1. 任意の API 秘密鍵を入力し、「**[!UICONTROL 保存]**」をクリックします。API 秘密鍵にアンパサンド（`&`）を使用しないでください。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3.png)

   >[!NOTE]
   >
   >API 秘密鍵は組織のパスワードと同じです。安全に保管してください。

1. 資格情報を入力するには、_[!UICONTROL Rest API 設定]_&#x200B;パネルで「**[!UICONTROL 表示]**」をクリックします。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4.png)

1. 確認ダイアログが表示されたら、「**[!UICONTROL OK]**」をクリックします。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5.png)

   >[!TIP]
   >
   >このウィンドウは開いたままにしておきます。この情報は、後で Salesforce の設定で必要になります。

## [!DNL Sales Insight] での [!DNL Salesforce] の設定 {#configure-sales-insight-in-salesforce}

1. Salesforce で、「**[!UICONTROL 設定]**」をクリックします。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6.png)

1. 「リモートサイト」を検索し、「**[!UICONTROL リモートサイトの設定]**」を選択します。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7.png)

1. 「**[!UICONTROL 新規リモートサイト]**」をクリックします。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8.png)

1. リモートサイト名を入力します（`MarketoSoapAPI` など）。Marketo Engage の _[!UICONTROL Soap API 設定]_&#x200B;パネルの Marketo ホスト URL であるリモートサイト URL を入力します。「**[!UICONTROL 保存]**」をクリックします。これで、Soap API 用のリモートサイト設定が作成されました。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9.png)

1. もう一度「**[!UICONTROL 新規リモートサイト]**」をクリックします。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10.png)

1. リモートサイト名を入力します（`MarketoAPI` など）。Marketo Engage の _[!UICONTROL Rest API 設定]_&#x200B;パネルの API URL であるリモートサイト URL を入力します。「**[!UICONTROL 保存]**」をクリックします。Rest API 用のリモートサイト設定が作成されました。

   >[!NOTE]
   >
   >__「**[!UICONTROL リモートサイト名]**」を選択します（`MarketoAPI` はここで使用されます）。**[!UICONTROL リモートサイト URL]** は、「Marketo での Sales Insight の設定」節の手順 3、API 設定を編集ダイアログの「Marketo ホスト」フィールドにあります。

## Sales Insight ユーザのプロファイルに標準の Salesforce オブジェクトへのアクセス権を付与 {#grant-sales-insight-users-profile-access}

Salesforce のセキュリティ強化により、AppExchange パッケージは標準オブジェクトに権限を付与できなくなり、Salesforce ユーザのプロファイルから関連する Salesforce オブジェクトにアクセス権を付与する必要があります。必要な権限を付与するには、次の手順に従います。

1. 「**[!UICONTROL 設定]**」をクリックします。

1. クイック検索で「プロファイル」を検索します。

1. Salesforce ユーザが使用しているプロファイルの横にある「**[!UICONTROL 編集]**」をクリックします。

1. 「_[!UICONTROL 標準オブジェクト権限]_」セクションで、[!UICONTROL リード]、[!UICONTROL 取引先責任者]、[!UICONTROL アカウント]、[!UICONTROL 商談]の各オブジェクトに対して&#x200B;**[!UICONTROL 読み取り]**&#x200B;アクセス権を有効にします。

1. 「**[!UICONTROL 保存]**」をクリックします。

## ページレイアウトのカスタマイズ {#customize-page-layouts}

1. 「**[!UICONTROL 設定]**」をクリックします。

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. 「ページレイアウト」を検索し、「**[!UICONTROL リード]**」の下の「**[!UICONTROL ページレイアウト]**」を選択します。

   ![](assets/image2015-5-28-14-3a58-3a39.png)

1. 左側の「**[!UICONTROL Visualforce Pages]**」をクリックします。「**[!UICONTROL セクション]**」を「_[!UICONTROL カスタムリンク]_」セクションの下のレイアウトにドラッグします。

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. **[!UICONTROL セクション名]**&#x200B;として「Marketo Sales Insight」と入力し、「**[!UICONTROL 1 列]**」を選択して、「**[!UICONTROL OK]**」をクリックします。

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. 「**[!UICONTROL リード]**」を新しいセクションにドラッグ＆ドロップします。

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   >
   >このボックスの名前は、オブジェクトタイプに基づいて変更されます。例えば、取引先責任者のページレイアウトを変更する場合、「取引先責任者」と表示されます。

1. 先ほど追加した「**[!UICONTROL リード]**」ブロックをダブルクリックします。

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. 高さを **450** ピクセルに編集し、「**[!UICONTROL OK]**」をクリックします。

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!NOTE]
   >
   >スクロールを使用してアクティビティにアクセスする必要がある場合は、「**[!UICONTROL スクロールバーを表示]**」をチェックします。

   >[!TIP]
   >
   >アカウントオブジェクトおよび商談オブジェクトの推奨される高さは 410 ピクセルです。

1. 左側の「**[!UICONTROL フィールド]**」をクリックします。次に、「**[!UICONTROL 緊急度]**」ラベルを検索して、**[!UICONTROL Marketo Sales Insight]** レイアウトにドラッグします。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-18.png)

1. 以下のフィールドについても、上記の手順を繰り返します。

   * 最新の注目のアクション
   * 最新の注目のアクション発生日
   * 最新の注目のアクションの詳細
   * 最新の注目のアクションのソース
   * 最新の注目のアクションのタイプ
   * セールスによる最後のアクティビティ
   * セールスによる最後のエンゲージメント
   * MSI 取引先責任者 ID
   * 相対スコア
   * 相対スコア値
   * 緊急度
   * 緊急度の値
   * Marketo 内に表示

1. 終了したら「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. 手順 5〜7 を繰り返して、**[!UICONTROL 取引先責任者]**、**[!UICONTROL アカウント]**、**[!UICONTROL 商談]**&#x200B;のそれぞれについて Visualforce ページセクションと Sales Insight フィールドを追加します。

1. 手順 8〜10 を繰り返して、**[!UICONTROL 取引先責任者]**&#x200B;にこれらの Sales Insight のフィールドを追加します。変更したら必ず保存します。

   * 最新の注目のアクション
   * 最新の注目のアクション発生日
   * [!UICONTROL 最新の注目のアクションの詳細]
   * [!UICONTROL 最新の注目のアクションのソース]
   * [!UICONTROL 最新の注目のアクションのタイプ]
   * [!UICONTROL セールスによる最後の Marketo アクティビティ]
   * [!UICONTROL セールスによる最後の Marketo エンゲージメント]
   * [!UICONTROL MKTO リードスコア]
   * [!UICONTROL 相対スコア]
   * [!UICONTROL 相対スコア値]
   * [!UICONTROL Sales Insight] - 取引先責任者の完全なリストページを開きます。
   * [!UICONTROL 緊急度]
   * [!UICONTROL 緊急度の値]

## カスタムユーザフィールドのマッピング {#map-custom-person-fields}

コンバージョンの際にデータが失われないように、Marketo のユーザフィールドを Salesforce の取引先責任者フィールドにマッピングする必要があります。次の手順に従って、マッピングします。

1. 「**[!UICONTROL 設定]**」をクリックします。

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. 検索バーで「フィールド」を検索し、「**[!UICONTROL リード]**」の下の「**[!UICONTROL フィールド]**」をクリックします。

   ![](assets/image2015-6-1-9-3a54-3a50.png)

1. 「**[!UICONTROL リードフィールドをマッピング]**」をクリックします。

   ![](assets/image2015-6-1-9-3a58-3a48.png)

1. **[!UICONTROL エンゲージメント]**&#x200B;の右側にあるドロップダウンをクリックします。

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

1. [Marketoの Sales Insight管理ページの Soap API パネルから資格情報をコピーして ](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"}[!DNL Salesforce] [!DNL Sales Insight] Configuration ページの Soap API セクションに貼り付けます。

1. [Marketoの Sales Insight管理ページの Rest API パネルから資格情報をコピーして ](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"}[!DNL Salesforce] [!DNL Sales Insight] Configuration ページの Rest API セクションに貼り付けます。

   ![](assets/configure-marketo-sales-insight-in-salesforce-enterprise-edition-25.png)

Marketo Sales Insight フィールドで、リード、取引先責任者、アカウント、商談の詳細を確認できます。

>[!NOTE]
>
>診断テストが失敗した場合は、[ ページレイアウトにさらにフィールドを追加する ](https://nation.marketo.com:443/t5/knowledgebase/how-to-repair-marketo-sales-insight-setup-configuration-problems/ta-p/248218){target="_blank"} ことで問題が解決する可能性があります。

>[!NOTE]
>
>アカウントの場合、Sales Insight にはすべてのメールが含まれますが、最新の注目のアクション、web アクティビティ、スコアの変更のみが含まれます。

>[!MORELIKETHIS]
>
>* [優先度、緊急度、相対スコア、最有望見込客](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md)
>* [ 「Marketo」タブを追加  [!DNL Salesforce]](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-marketo-tab-to-salesforce.md)
>* [Sales Insight へのアクセスをプロファイルに追加](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"}
