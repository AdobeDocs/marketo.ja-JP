---
description: チーム向けのSales Insightの設定 — Marketto Docs — 製品ドキュメント
title: チーム向けのSales Insightの設定
translation-type: tm+mt
source-git-commit: ed9399396c82a3b2fb93c83ffdaa1dc7b0827306
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 0%

---


# チームのSales Insightの設定{#setting-up-sales-insight-for-your-team}

他のプロファイルのアクセスを削除しながら、Sales Insightへのアクセスを持つプロファイルを作成する方法を次に示します。 これは、[Sales InsightAppExchangeパッケージ](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)を既にインストール済みのユーザー用です。

## Sales Insight用の新しいプロファイルの作成{#create-a-new-profile-for-sales-insight}

Sales Insightユーザー専用のプロファイルがある場合は、この手順をスキップできます。

1. Salesforceで、設定ページに移動します。

1. クイック検索でプロファイルを検索し、**プロファイル**&#x200B;オプションを選択します。

1. ページ上部の「**新規プロファイル**」ボタンをクリックします。

1. コピーするプロファイルを選択し、名前を付けます(例：Sales Insightユーザーを参照)。

1. 終了したら「**保存**」をクリックします。

## 追加Sales Insightの権限{#add-sales-insight-permissions}

1. プロファイルリストに戻ります。

1. 先ほど作成した新しいプロファイル(またはSales Insightにアクセス権を与えたい他の既存のプロファイル)の&#x200B;**編集**&#x200B;リンクをクリックします。

1. 編集ページで、いくつかの設定を変更する必要があります。

   **Sales Insight**:

   * 「アプリのカスタム設定」で、「マーケティング」にチェックを付けて、Marketoアプリを表示します。
   * 「タブの設定」で、「マーケティング」タブを「デフォルトオン」に変更します
   * 「カスタムオブジェクト権限」で、Marketor Sales InsightのConfigの読み取り、作成、編集および削除(ユーザーが、設定設定に対するアクセス権を持っている必要がある場合（通常は管理者に使用）)をオンにします

   **Sales Insightへのアクセスを許可されないプロファイルの場合**:

   * 「アプリのカスタム設定」で、「マーケティング」のチェックを外して、Marketorアプリを非表示にします
   * 「タブの設定」で、「マーケティング」タブを「タブを非表示」に変更します
   * 「カスタムオブジェクト権限」で、Marketor Sales Insight設定の「読み取り」、「作成」、「編集」、「削除」のチェックを外します。


1. 終了したら「**保存**」をクリックします。

## 販売インサイトのレイアウトを作成{#create-layout-for-sales-insight}

1. 設定ページに移動し、**アプリ設定**/**カスタマイズ**/**リード**/**ページレイアウト**&#x200B;をクリックします。 次に、「**新規**」ボタンをクリックします。

1. 選択したレイアウトをコピーし、適切な名前を付けます(例：Sales Insightのレイアウトを参照)。

1. 終了したら「**保存**」をクリックします。

1. 連絡先、オポチュニティ、アカウントのページレイアウトに対して、この手順を繰り返します。

## プロファイルをレイアウトに割り当て{#assign-profile-to-layout}

1. 「ページレイアウト」セクションに戻り、「**ページレイアウトの割り当て**」ボタンをクリックします。

1. 「**割り当てを編集**」を選択します。

1. リストからSales Insightプロファイルを選択し、「ページレイアウトを選択」ドロップダウンからSales Insightレイアウトを選択します。

1. 終了したら「**保存**」をクリックします。

1. 連絡先、オポチュニティ、アカウントのページレイアウトに対して、この手順を繰り返します。

## その他の変更{#other-changes}

Sales Insightの項目が表示される他の場所は、次のとおりです。 プロファイルを使用してアクセスを制限できないので、すぐに削除する必要があります。

* 連絡先、リード、アカウントの検索レイアウトから「Sales Insight」ボタンを削除します。
* 「連絡先」および「リードリスト」から「Sales Insight」列を削除します。
