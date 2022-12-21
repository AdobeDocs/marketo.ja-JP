---
unique-page-id: 42762322
description: Salesforce の Marketo Sales Insight 設定タブ - Marketo ドキュメント - 製品ドキュメント
title: Salesforce の Marketo Sales Insight 設定タブ
exl-id: 4e2abd48-b0a5-4b71-939b-e66c7e39bb6c
source-git-commit: 5c4bce6ab6801b861f70722b6782df34f96fed10
workflow-type: tm+mt
source-wordcount: '601'
ht-degree: 100%

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
* 今後のキャンペーンおよびイベントの読み込み：「イベントとキャンペーン」タブをオンデマンドの「次の項目を読み込み」ボタンの後に配置することで、ユーザが行う Rest API 呼び出しの数を減らすことができます
* タブ設定：デフォルトでは、5 つのタブすべてが使用可能になります。Sales Insight パネルでタブの順序を選択できます。すべてのレイアウト（リード、取引先責任者、アカウント、商談）に同じ順序が適用されます。

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-2.png)

**「Marketo グローバル」タブ**

* RSS フィードが有効：有効にすると、MSI ユーザは（Salesforce のリードフィードに加えて）RSS フィードでリードフィードを表示できます。RSS フィードは、「トークンの有効期限」機能が無効な場合にのみ機能します。この設定は、Marketo Sales Insight 管理ページで制御します。
* 最有望見込客（デバッグモード）
* デフォルトの非表示：ここで選択するオプションは、「非表示」アイコンをクリックしたときに、Marketo の「最有望見込客」タブに最有望見込客が非表示になる日数です
* 取引先責任者ステータスフィールド：ここで選択するオプションは、Marketo の「最有望見込客」タブの「ステータスヘッダー」列に入力される値です
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

## Marketo Sales Insight のリセット {#reset-marketo-sales-insight}

これを選択すると、SFDC 内のすべての設定が消去され、復元できなくなります。すべてを再度設定する必要があります。

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-5.png)

>[!IMPORTANT]
>
>Sales Insights Actions 機能を使用していない場合は、「MSI Actions を有効にする」チェックボックスをオンにしないでください。

>[!MORELIKETHIS]
>
>[Sales Insight へのアクセスをプロファイルに追加](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target=&quot;_blank&quot;}
