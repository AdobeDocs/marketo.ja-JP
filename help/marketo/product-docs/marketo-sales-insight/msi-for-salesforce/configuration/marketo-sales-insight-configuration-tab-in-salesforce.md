---
unique-page-id: 42762322
description: Salesforce の Marketo Sales Insight 設定タブ - Marketo ドキュメント - 製品ドキュメント
title: Salesforce の Marketo Sales Insight 設定タブ
exl-id: 4e2abd48-b0a5-4b71-939b-e66c7e39bb6c
feature: Marketo Sales Insights
source-git-commit: 4848676d423ff96c2e880819bc760b2f8dbbd094
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 78%

---

# Salesforce の Marketo Sales Insight 設定タブ {#marketo-sales-insight-configuration-tab-in-salesforce}

## 操作上の設定 {#operational-settings}

SFDC で Sales Insight を使用するには、この設定が必要です。

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-1.png)

* MSI は Soap と Rest API の両方を使用します
* Marketo アカウントの Sales Insight ページには、Soap および Rest API 資格情報を持つ 2 つの対応するパネルが表示され、ここにコピーして貼り付けることができます
* Soap API と Rest API には、組織のニーズに基づいて個別にタイムアウトを設定できます。最大時間は 120 秒です
* インサイトダッシュボードを無効にする：Rest API 資格情報を削除し、Soap API のみを使用できます。これにより、すべての MSI Visualforce パネルの「Insights ダッシュボード」タブが無効になります

## MSI の設定 {#msi-configuration}

設定は、すべての MSI ユーザに適用でき、プロファイルに固有の設定ではありません。

**Visualforce ページの設定**

* アクションを有効にするドロップダウン：
   * リードと取引先責任者 MSI レイアウトのドロップダウンから「Marketo メールを送信」を非表示にできます
   * リードと取引先責任者 MSI レイアウトのドロップダウンから「Marketo キャンペーンに追加」オプションを非表示にできます
* 今後のイベント：招待イベント、ユーザに対するすべてのイベント、またはこのタブを完全に非表示にできます
* 今後のキャンペーン：すべてのメールキャンペーンを表示、またはこのタブを完全に非表示にできます
* 今後のキャンペーンとイベントの読み込み：オンデマンドの「今後の項目を読み込み」ボタンの背後にイベントおよび「キャンペーン」タブを配置することで、ユーザーが実行する Rest API 呼び出しの数を減らす機能
* タブ設定：デフォルトでは、5 つのタブすべてが使用可能になります。Sales Insight パネルでタブの順序を選択できます。すべてのレイアウト（リード、取引先責任者、アカウント、商談）に同じ順序が適用されます。

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-2.png)

**「Marketo グローバル」タブ**

* RSS フィードが有効：有効にすると、MSI ユーザは（Salesforce のリードフィードに加えて）RSS フィードでリードフィードを表示できます。RSS フィードは、「トークンの有効期限」機能が無効になっている場合にのみ機能します。 この設定は、Marketo Sales Insight 管理ページで制御します。
* 最有望見込客（デバッグモード）
* デフォルトの非表示：ここで選択するオプションは、「非表示」アイコンをクリックすると、Marketoのおすすめコンテンツのタブにベストベットが表示されない日数です
* 連絡先ステータスフィールド：ここで選択するオプションは、Marketoの「おすすめコンテンツ」タブのステータスヘッダー列に入力される値です
* ライブフィード設定：ライブフィードのみを表示するオプション（リードパネル、取引先責任者パネル、アカウントパネル、商談パネル、グローバル Marketo ページ）、リードフィードのみを表示するオプション（Marketo グローバルページ内）、またはライブとリードフィードの両方を表示するオプション
* タブ設定：デフォルトでは、5 つのタブすべてが使用可能になります。Marketo グローバルページでタブの順序を選択できます

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-3.png)

**制限**

* アクティビティ（注目のアクティビティ、web アクティビティ、メール）は、デフォルトで 1000 に設定されています。メールキャンペーンとイベントは、デフォルトで 200 に設定されています
* 組織でタイムアウトの問題が発生した場合は、制限を減らすことができます

**アクションの設定**

* Marketo メールの送信：これを有効にすると、すべての Sales Insight ユーザが、リードパネル、取引先責任者パネル、アカウントパネル、商談パネルおよび「最有望見込客」タブ（一括アクションとインラインエンゲージメント）からメールを送信するアクセス権を付与されます
* Marketo Campaign に追加：これを有効にすると、すべての Sales Insight ユーザが、リードパネル、取引先責任者パネル、アカウントパネル、商談パネルおよび「最有望見込客」タブ（一括アクションとインラインエンゲージメント）からキャンペーンに追加できるようになります

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-4.png)

## サポート設定 {#support-settings}

このチェックボックスを選択すると、Salesforce インスタンスでデバッグログが有効になります。 問題のトラブルシューティングに役立ちます。

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-5.png)

## Marketo Sales Insight のリセット {#reset-marketo-sales-insight}

これを選択すると、SFDC 内のすべての設定が消去され、復元できなくなります。すべてを再度設定する必要があります。

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-6.png)

>[!IMPORTANT]
>
>Sales Insights のアクション機能を使用している場合を除き、「MSI アクションを有効にする」チェックボックスを選択しないでください。

>[!MORELIKETHIS]
>
>[Sales Insight へのアクセスをプロファイルに追加](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"}
