---
unique-page-id: 3571743
description: Salesforce Professional Edition でMarketo Sales Insight を設定する方法を説明します。
title: Salesforce Professional Edition での Marketo Sales Insight の設定
exl-id: fae63560-0bb3-46a9-94a3-cc27c1aa363e
feature: Marketo Sales Insights
source-git-commit: 68abebb5e1f9dc0780aedcff51d46ed12d5b4d0a
workflow-type: tm+mt
source-wordcount: '773'
ht-degree: 39%

---

# Salesforce Professional Edition での Marketo Sales Insight の設定 {#configure-marketo-sales-insight-in-salesforce-professional-edition}

次の手順を実行して、Salesforce Professional Edition でMarketo Sales Insight を設定します。

>[!PREREQUISITES]
>
>* Salesforce Professional Edition に Marketo をインストールします。
>
>* [Salesforce AppExchange での Marketo Sales Insight パッケージのインストール](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}

>[!NOTE]
>
>**管理者権限が必要です。**

## Sales Insight のMarketo Engage {#configure-sales-insight-in-marketo}

1. MarketoアカウントからMarketo Sales Insight の資格情報を取得するには、新しいブラウザーウィンドウを開きます。

1. 次に移動： **[!UICONTROL 管理者]** 領域と選択 **[!UICONTROL Sales Insight]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1-1.png)

1. 「**[!UICONTROL API 設定を編集]**」をクリックします。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2-1.png)

1. 任意の API 秘密鍵を入力し、「**[!UICONTROL 保存]**」をクリックします。アンパサンド (`&`) を API 秘密鍵に置き換えます。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3-1.png)

   >[!NOTE]
   >
   >API 秘密鍵は組織のパスワードのようなもので、セキュリティで保護されている必要があります。

1. 資格情報を入力するには、 **[!UICONTROL 表示]** （内） _[!UICONTROL Rest API 設定]_ パネル。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4-1.png)

1. 確認ダイアログが表示されたら、「 **[!UICONTROL OK]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5-1.png)

## Salesforce での Sales Insight の設定 {#configure-sales-insight-in-salesforce}

1. Salesforce から、 **[!UICONTROL 設定]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6-1.png)

1. 「リモートサイト」を検索し、「**[!UICONTROL リモートサイトの設定]**」を選択します。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7-1.png)

1. 「**[!UICONTROL 新規リモートサイト]**」をクリックします。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8-1.png)

1. リモートサイト名を入力します（次のように指定できます）。 `MarketoSoapAPI`) をクリックします。 Remote Site URL と入力します。これは、Marketo Engageの Soap API 設定パネルのMarketoホスト URL です。 「**[!UICONTROL 保存]**」をクリックします。これで、Soap API 用のリモートサイト設定が作成されました。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9-1.png)

1. もう一度「**[!UICONTROL 新規リモートサイト]**」をクリックします。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10-1.png)

1. リモートサイト名を入力します（「MarketoRestAPI」など）。「リモートサイト URL」に、Marketo の Rest API 設定パネルの API URL を入力します。「**[!UICONTROL 保存]**」をクリックします。Rest API 用のリモートサイト設定が作成されました。

## Sales Insight ユーザーに標準の Salesforce オブジェクトへのプロファイルアクセスを許可する {#grant-sales-insight-users-profile-access}

Salesforce のセキュリティ強化により、AppExchangeパッケージは標準オブジェクトに権限を付与できなくなり、Salesforce ユーザーのプロファイルから関連する Salesforce オブジェクトにアクセス権を付与する必要があります。 次の手順に従って、必要な権限を付与します。

1. 「**[!UICONTROL 設定]**」をクリックします。

1. クイック検索で「プロファイル」を検索します。

1. クリック **[!UICONTROL 編集]** をクリックします。

1. [ 標準オブジェクト権限 ] セクションで、リード、連絡先、アカウント、商談の各オブジェクトに対して読み取りアクセスを有効にします。

1. 「**[!UICONTROL 保存]**」をクリックします。

## ページレイアウトのカスタマイズ {#customize-page-layouts}

1. 「**[!UICONTROL 設定]**」をクリックします。

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. 「ページレイアウト」を検索し、「**[!UICONTROL リード]**」の下の「**[!UICONTROL ページレイアウト]**」を選択します。

   ![](assets/image2015-5-28-14-3a58-3a39-1.png)

1. 左側の「**[!UICONTROL Visualforce Pages]**」をクリックします。「**[!UICONTROL セクション]**」をカスタムリンクセクションの下のレイアウトにドラッグします。

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. 「**[!UICONTROL セクション名]**」に「Marketo Sales Insight」と入力します。「**[!UICONTROL 1 列]**」を選択し、「**[!UICONTROL OK]**」をクリックします。

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. 「**リード**」を新しいセクションにドラッグ＆ドロップします。

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   >
   >このボックスの名前は、オブジェクトの種類に応じて変わります。 例えば、連絡先のページレイアウトを変更する場合、連絡先と表示されます。

1. 次をダブルクリックします。 **[!UICONTROL リード]** ブロックを追加しました。

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. 高さを 450 ピクセルに編集し、 **[!UICONTROL OK]**.

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!NOTE]
   >
   >スクロールを使用してアクティビティにアクセスする必要がある場合は、「**[!UICONTROL スクロールバーを表示]**」をチェックします。

   >[!TIP]
   >
   >Accounts オブジェクトと Opportunity オブジェクトの推奨高さは 410 ピクセルです。

1. クリック **[!UICONTROL フィールド]** 左側に 次に、「**[!UICONTROL エンゲージメント]**」ラベルを検索して、**[!UICONTROL Marketo Sales Insight]** レイアウトにドラッグします。

   ![](assets/image2015-5-22-16-3a32-3a46-1.png)

1. 次のフィールドについて、前述の手順を繰り返します。

   * [!UICONTROL エンゲージメント]
   * [!UICONTROL 相対スコア値]
   * [!UICONTROL 緊急度の値]
   * [!UICONTROL 最新の注目のアクションの日付]
   * [!UICONTROL 最新の注目のアクションの詳細]
   * [!UICONTROL 最新の注目のアクションのソース]
   * [!UICONTROL 最新の注目のアクションのタイプ]

1. 終了したら「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. Visualforce のページセクションを追加するには **[!UICONTROL 連絡先]**, **[!UICONTROL アカウント]**、および **[!UICONTROL 商談]**、手順 5～7 を繰り返します。

1. 手順 8 ～ 10 を繰り返して、次の項目に Sales Insight フィールドを追加します。 **[!UICONTROL 連絡先]**. 変更したら必ず保存します。

## カスタム担当者フィールドのマッピング {#map-custom-person-fields}

変換が正しく機能するように、Marketoの担当者フィールドを Salesforce の連絡先フィールドにマッピングする必要があります。 次の手順に従って、マップします。

1. 「**[!UICONTROL 設定]**」をクリックします。

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. 検索バーで「フィールド」を検索し、「**[!UICONTROL リード]**」の下の「**[!UICONTROL フィールド]**」をクリックします。

   ![](assets/image2015-6-1-9-3a54-3a50-1.png)

1. 「**[!UICONTROL リードフィールドをマッピング]**」をクリックします。

   ![](assets/image2015-6-1-9-3a58-3a48-1.png)

1. 右側のドロップダウンをクリックし、 **[!UICONTROL エンゲージメント]**.

   ![](assets/image2015-6-1-10-3a9-3a53-1.png)

1. リストから「**[!UICONTROL 取引先責任者、エンゲージメント]**」を選択します。

   ![](assets/image2015-6-1-10-3a12-3a11-1.png)

1. これらのフィールドも繰り返し、マッピングします。

   | Marketo の人物のカスタムフィールド | Salesforce の取引先責任者のカスタムフィールド |
   |--- |--- |
   | `Engagement` | `Contact.Engagement` |
   | `Relative Score Value` | `Contact.Relative Score Value` |
   | `Urgency Value` | `Contact.Urgency Value` |
   | `Last Interesting Moment Date` | `Contact.Last Interesting Moment Date` |
   | `Last Interesting Moment Desc` | `Contact.Last Interesting Moment Desc` |
   | `Last Interesting Moment Source` | `Contact.Last Interesting Moment Source` |
   | `Last Interesting Moment Type` | `Contact.Last Interesting Moment Type` |

   {style="table-layout:auto"}

1. 完了したら、「 **[!UICONTROL 保存]**.

   ![](assets/image2014-9-24-17-3a37-3a17.png)

## Marketo Sales Insight の「設定」タブ {#marketo-sales-insight-configuration-tab}

1. Salesforce から、 **+** をクリックし、 **[!UICONTROL Marketo Sales Insight 設定]**.

1. の Soap API パネルから資格情報をコピーします。[Marketo Sales Insight 管理ページ](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"}をクリックし、Salesforce Sales Insight 設定ページの「SOAP API」セクションに貼り付けます。

1. から資格情報をコピーします。 **[!UICONTROL Rest API]** パネル内 [Marketo Sales Insight 管理ページ](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} をクリックし、Salesforce Sales Insight 設定ページの Rest API セクションに貼り付けます。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-27.png)

リード、連絡先、アカウント、商談のMarketo Sales Insight フィールドが表示されます。

>[!NOTE]
>
>診断テストに失敗した場合は、 [ページレイアウトへのフィールドの追加](https://nation.marketo.com/t5/knowledgebase/how-to-repair-marketo-sales-insight-setup-configuration-problems/ta-p/248218){target="_blank"} 問題が修正される可能性があります。

>[!NOTE]
>
>アカウントの場合、Sales Insight にはすべてのメールが含まれますが、最新の注目のアクション、Web アクティビティ、スコアの変更のみが含まれます。

>[!MORELIKETHIS]
>
>* [優先度、緊急度、相対スコア、最有望見込客](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md){target="_blank"}
>* [Salesforce への「Marketo」タブの追加](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-marketo-tab-to-salesforce.md){target="_blank"}
>* [Sales Insight へのアクセスをプロファイルに追加](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"}
