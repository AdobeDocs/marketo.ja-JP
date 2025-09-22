---
description: Sales Insight へのアクセスをプロファイルに追加 - Marketo ドキュメント - 製品ドキュメント
title: Sales Insight へのアクセスをプロファイルに追加
exl-id: 269f9093-f530-4e3b-aac7-e317976cf0f0
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 100%

---

# [!DNL Sales Insight] へのアクセスをプロファイルに追加 {#add-sales-insight-access-to-profiles}

ここでは、[!DNL Sales Insight] へのアクセス権を持つプロファイルを作成し、他のプロファイルのアクセス権を削除する方法について説明します。これは、[[!DNL Sales Insight]  AppExchange パッケージ](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}を既にインストール済みのユーザ向けです。

>[!IMPORTANT]
>
>以前にすべてのプロファイルに [!DNL Sales Insight] へのアクセス権を付与している場合は、[プロファイルレベルのアクセス権を削除](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/remove-sales-insight-access.md){target="_blank"}して、この権限セットを使用する必要があります。

## [!DNL Sales Insight] の新しいプロファイルの作成 {#create-a-new-profile-for-sales-insight}

[!DNL Sales Insight] ユーザの専用プロファイルがある場合は、この手順をスキップできます。

1. [!DNL Salesforce] で、セットアップページに移動します。

1. クイック検索でプロファイルを検索し、「**[!UICONTROL プロファイル]**」オプションを選択します。

1. ページの上部にある「**[!UICONTROL 新規プロファイル]**」ボタンをクリックします。

1. 複製するプロファイルを選択して、名前を付けます（例：Sales Insight ユーザ）。

1. 終了したら「**[!UICONTROL 保存]**」をクリックします。

## [!DNL Sales Insight] 権限の追加 {#add-sales-insight-permissions}

1. プロファイルリストに戻ります。

1. 作成した新規プロファイル（または [!DNL Sales Insight] のアクセス権を付与する既存のプロファイル）の「**[!UICONTROL 編集]**」リンクをクリックします。

1. 編集ページでは、いくつかの設定を変更する必要があります。

   **[!DNL Sales Insight]** へのアクセスが許可されているプロファイルの場合：

   * 「タブ設定」で、Marketo タブを「デフォルトでオン」に変更します
   * 「カスタムオブジェクト権限」で、「[!DNL Marketo Sales Insight] 設定」の「読み取り」、「作成」、「編集」、「削除」チェックボックスをオンにします（ユーザが設定にアクセスする必要がある場合。通常は管理者に使用されます）。

   **[!DNL Sales Insight]** へのアクセスが許可されていないプロファイルの場合：

   * 「タブ設定」で、Marketo タブを「タブを非表示」に変更します
   * 「カスタムオブジェクト権限」で、「[!DNL Marketo Sales Insight] 設定」の「読み取り」、「作成」、「編集」、「削除」チェックボックスをオフにします。

1. 終了したら「**[!UICONTROL 保存]**」をクリックします。

## [!DNL Sales Insight] のレイアウトの作成 {#create-layout-for-sales-insight}

1. セットアップページに移動して、**[!UICONTROL アプリセットアップ]**／**[!UICONTROL カスタマイズ]**／**[!UICONTROL リード]**／**[!UICONTROL ページレイアウト]**&#x200B;をクリックします。次に、「**[!UICONTROL 新規]**」ボタンをクリックします。

1. お好みのレイアウトを複製し、レイアウトに適切な名前を付けます（例：Sales Insight レイアウト）。

1. 終了したら「**[!UICONTROL 保存]**」をクリックします。

1. 「[!UICONTROL 取引先責任者]」、「[!UICONTROL 商談]」、「[!UICONTROL アカウント]」のページレイアウトについても、この手順を繰り返します。

## プロファイルのレイアウトへの割り当て {#assign-profile-to-layout}

1. 「ページレイアウト」セクションに戻り、「**[!UICONTROL ページレイアウト割り当て]**」ボタンをクリックします。

1. 「**[!UICONTROL 割り当てを編集]**」を選択します。

1. リストから [!DNL Sales Insight] プロファイルを選択して、[!UICONTROL ページレイアウトを選択]ドロップダウンから [!DNL Sales insight] レイアウトを選択します。

1. 終了したら「**[!UICONTROL 保存]**」をクリックします。

1. 「[!UICONTROL 取引先責任者]」、「[!UICONTROL 商談]」、「[!UICONTROL アカウント]」のページレイアウトについても、この手順を繰り返します。

## その他の変更点 {#other-changes}

以下に、[!DNL Sales Insight] 項目が表示される可能性のあるその他の場所を示します。プロファイルを使用してアクセスを制限することはできないので、これらの項目を完全に削除する必要があります。

* 「[!UICONTROL 取引先責任者]」、「[!UICONTROL リード]」、「[!UICONTROL アカウント]」の「検索レイアウト」から「[!DNL Sales Insight]」ボタンを削除
* 取引先責任者リストおよびリードリストから [!DNL Sales Insight] 列を削除
