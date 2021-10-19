---
description: チーム向けの Sales Insight の設定 - Marketo ドキュメント - 製品ドキュメント
title: チーム向けの Sales Insight の設定
exl-id: 269f9093-f530-4e3b-aac7-e317976cf0f0
source-git-commit: ecceb1a3aff3a2088379f8f4f2ac33e566f90e21
workflow-type: ht
source-wordcount: '416'
ht-degree: 100%

---

# チーム向けの Sales Insight の設定 {#setting-up-sales-insight-for-your-team}

ここでは、Sales Insight へのアクセス権を持つプロファイルを作成し、他のプロファイルのアクセス権を削除する方法を説明します。これは、[Sales Insight AppExchange パッケージ](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)を既にインストール済みのユーザー向けです。

## Sales Insight 用の新しいプロファイルの作成 {#create-a-new-profile-for-sales-insight}

Sales Insight ユーザー専用のプロファイルがある場合は、この手順をスキップできます。

1. Salesforce で、Setup ページに移動します。

1. クイック検索でプロファイルを検索し、「**Profile**」オプションを選択します。

1. ページの上部にある「**New Profile**」ボタンをクリックします。

1. 複製するプロファイルを選択して、名前を付けます（例：Sales Insight User）。

1. 終了したら「**保存**」をクリックします。

## Sales Insight 権限の追加 {#add-sales-insight-permissions}

1. プロファイルリストに戻ります。

1. 作成した新規プロファイル（または Sales Insight のアクセス権を付与したい既存のプロファイル）の「**編集**」リンクをクリックします。

1. 編集ページでは、いくつかの設定を変更する必要があります。

   **Sales Insight へのアクセスが許可されているプロファイルの場合**：

   * 「Tab Settings」で、Marketo タブを「Default On」に変更します
   * 「Custom Object Permissions」で、「Marketo Sales Insight Config」の「Read」、「Create」、「Edit」、「Delete」チェックボックスをオンにします（ユーザーが構成設定にアクセスする必要がある場合。通常は管理者に使用されます）

   **Sales Insight へのアクセスが許可されていないプロファイルの場合**：

   * 「Tab Settings」で、Marketo タブを「Tab Hidden」に変更します
   * 「Custom Object Permissions」で、「Marketo Sales Insight Config」の「Read」、「Create」、「Edit」、「Delete」チェックボックスをオフにします


1. 終了したら「**保存**」をクリックします。

## Sales Insight のレイアウトの作成 {#create-layout-for-sales-insight}

1. Setup ページに移動して、**App Setup**／**Customize**／**Leads**／**Page Layouts** をクリックします。次に、「**New**」ボタンをクリックします。

1. お好みのレイアウトを複製し、レイアウトに適切な名前を付けます（例：Sales Insight Layout）。

1. 終了したら「**保存**」をクリックします。

1. 「Contacts」、「Opportunities」、「Accounts」のページレイアウトについても、この手順を繰り返します。

## プロファイルのレイアウトへの割り当て {#assign-profile-to-layout}

1. 「Page Layouts」セクションに戻り、「**Page Layout Assignment**」ボタンをクリックします。

1. 「**Edit Assignment**」を選択します。

1. リストから Sales Insight プロファイルを選択して、「Select Page Layout」ドロップダウンから Sales Insight レイアウトを選択します。

1. 終了したら「**保存**」をクリックします。

1. 「Contacts」、「Opportunities」、「Accounts」のページレイアウトについても、この手順を繰り返します。

## その他の変更点 {#other-changes}

以下に、Sales Insight 項目が表示される可能性のあるその他の場所を示します。プロファイルを使用してアクセスを制限することはできないので、これらの項目を完全に削除する必要があります。

* 「Contacts」、「Leads」、「Accounts」の「Search Layouts」から「Sales Insight」ボタンを削除
* Contact および Lead リストから Sales Insight 列を削除
