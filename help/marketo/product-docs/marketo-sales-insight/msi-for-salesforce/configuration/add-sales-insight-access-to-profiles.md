---
description: Sales Insight へのアクセスをプロファイルに追加 - Marketo ドキュメント - 製品ドキュメント
title: Sales Insight へのアクセスをプロファイルに追加
exl-id: 269f9093-f530-4e3b-aac7-e317976cf0f0
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 44%

---

# プロファイルへの [!DNL Sales Insight] アクセスの追加 {#add-sales-insight-access-to-profiles}

次に、他のプロファイルへのアクセス権を削除しながら、[!DNL Sales Insight] へのアクセス権を持つプロファイルを作成する方法を示します。 [[!DNL Sales Insight] AppExchange パッケージ ](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"} を既にインストールしているユーザー用です。

>[!IMPORTANT]
>
>以前にすべてのプロファイルに [!DNL Sales Insight] アクセス権を付与した場合、この権限セットを使用するには [ プロファイルレベルのアクセス権を削除 ](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/remove-sales-insight-access.md){target="_blank"} する必要があります。

## [!DNL Sales Insight] の新規プロファイルを作成 {#create-a-new-profile-for-sales-insight}

[!DNL Sales Insight] ユーザー専用のプロファイルがある場合は、この手順をスキップできます。

1. [!DNL Salesforce] で、設定ページに移動します。

1. クイック検索でプロファイルを検索し、「**[!UICONTROL プロファイル]**」オプションを選択します。

1. ページの上部にある「**[!UICONTROL 新規プロファイル]**」ボタンをクリックします。

1. 複製するプロファイルを選択して、名前を付けます（例：Sales Insight ユーザ）。

1. 終了したら「**[!UICONTROL 保存]**」をクリックします。

## [!DNL Sales Insight] 権限の追加 {#add-sales-insight-permissions}

1. プロファイルリストに戻ります。

1. 作成したばかりの新しいプロファイル（またはアクセス権を付与したい他の既存プロファイル）の **[!UICONTROL 編集]** リンクをク [!DNL Sales Insight] ックします。

1. 編集ページでは、いくつかの設定を変更する必要があります。

   **アクセスが許可されているプロファイルの場合：[!DNL Sales Insight]**

   * 「タブ設定」で、Marketo タブを「デフォルトでオン」に変更します
   * カスタムオブジェクト権限で、[!DNL Marketo Sales Insight] 設定に対する読み取り、作成、編集、削除を確認します（ユーザーが設定へのアクセス権を持っている必要がある場合で、通常、管理者が使用します）

   **[!DNL Sales Insight]** へのアクセスが許可されていないプロファイルの場合：

   * 「タブ設定」で、Marketo タブを「タブ非表示」に変更します
   * 「カスタム・オブジェクト」権限で、[!DNL Marketo Sales Insight] 設定の「読取り」、「作成」、「編集」、「削除」のチェックを外します

1. 終了したら「**[!UICONTROL 保存]**」をクリックします。

## [!DNL Sales Insight] のレイアウトを作成 {#create-layout-for-sales-insight}

1. セットアップページに移動して、**[!UICONTROL アプリセットアップ]**／**[!UICONTROL カスタマイズ]**／**[!UICONTROL リード]**／**[!UICONTROL ページレイアウト]**&#x200B;をクリックします。次に、「**[!UICONTROL 新規]**」ボタンをクリックします。

1. お好みのレイアウトを複製し、レイアウトに適切な名前を付けます（例：Sales Insight レイアウト）。

1. 終了したら「**[!UICONTROL 保存]**」をクリックします。

1. [!UICONTROL  連絡先 ]、[!UICONTROL  商談 ]、[!UICONTROL  アカウント ]」ページレイアウトに対して、これらの手順を繰り返します。

## プロファイルのレイアウトへの割り当て {#assign-profile-to-layout}

1. 「ページレイアウト」セクションに戻り、「**[!UICONTROL ページレイアウト割り当て]**」ボタンをクリックします。

1. 「**[!UICONTROL 割り当てを編集]**」を選択します。

1. リストから [!DNL Sales Insight] プロファイルを選択し、「[!DNL Sales insight] ページレイアウトを選択 [!UICONTROL 」ドロップダウンから ] レイアウトを選択します。

1. 終了したら「**[!UICONTROL 保存]**」をクリックします。

1. [!UICONTROL  連絡先 ]、[!UICONTROL  商談 ]、[!UICONTROL  アカウント ]」ページレイアウトに対して、これらの手順を繰り返します。

## その他の変更点 {#other-changes}

[!DNL Sales Insight] の項目が表示される他の場所を次に示します。 プロファイルを使用してアクセスを制限することはできないので、これらの項目を完全に削除する必要があります。

* [!DNL Sales Insight] 連絡先 [!UICONTROL 、] リード [!UICONTROL 、] アカウント [!UICONTROL  の検索レイアウトから ] のボタンを削除
* 連絡先リストとリードリストから [!DNL Sales Insight] 列を削除
