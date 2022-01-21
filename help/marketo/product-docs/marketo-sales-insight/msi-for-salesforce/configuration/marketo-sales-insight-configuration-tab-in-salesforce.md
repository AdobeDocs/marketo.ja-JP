---
unique-page-id: 42762322
description: Salesforce の「Marketo Sales Insight 設定」タブ — Marketoドキュメント — 製品ドキュメント
title: Salesforce の Marketo Sales Insight 設定タブ
exl-id: 4e2abd48-b0a5-4b71-939b-e66c7e39bb6c
source-git-commit: 15263f9c23c958499aaa2e4e6491b4962c617358
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 4%

---

# Salesforce の Marketo Sales Insight 設定タブ {#marketo-sales-insight-configuration-tab-in-salesforce}

## 操作設定 {#operational-settings}

SFDC で Sales Insight を使用するには、この設定が必要です。

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-1.png)

* MSI は Soap と Rest API の両方を使用します
* Marketoアカウントの Sales Insight ページには、Soap および Rest API 資格情報を持つ 2 つの対応するパネルが表示され、ここにコピーして貼り付けることができます
* Soap API と Rest API には、組織のニーズに基づいて個別にタイムアウトを設定できます。 最大時間は 120 秒です
* インサイトダッシュボードを無効にする：Rest API 資格情報を削除し、Soap API のみを使用できます。 これにより、すべての MSI Visualforce パネルの「インサイトダッシュボード」タブが無効になります

## MSI 設定 {#msi-configuration}

設定は、すべての MSI ユーザに適用でき、プロファイルに固有の設定ではありません。

**Visualforce ページ設定**

* アクションを有効にするドロップダウン：
   * リードと連絡先 MSI レイアウトのドロップダウンから「Marketoメールを送信」を非表示にする機能
   * リードと連絡先 MSI レイアウトのドロップダウンから「 Marketo Campaign に追加」オプションを非表示にする機能
* 今後のイベント：招待イベント、ユーザーに対するすべてのイベント、またはこのタブを完全に非表示にする機能
* 今後のキャンペーン：すべての電子メールキャンペーンを表示する機能、またはこのタブを完全に非表示にする機能
* 今後のキャンペーンおよびイベントの読み込み：イベントとキャンペーンタブをオンデマンドの「次の項目を読み込み」ボタンの後に配置することで、ユーザーがおこなう Rest API 呼び出しの数を減らす機能
* タブ設定：デフォルトでは、5 つのタブすべてが使用可能になります。 Sales Insight パネルでタブの順序を選択できます。 すべてのレイアウト（リード、連絡先、アカウント、商談）に同じ順序が適用されます

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-2.png)

**Marketo Global Tab**

* RSS フィードが有効：有効にすると、MSI ユーザは（Salesforce のリードフィードに加えて）RSS フィードでリードフィードを表示できます。 RSS フィードは、「トークンの有効期限」機能が無効な場合にのみ機能します。 この設定は、Marketo Sales Insight 管理ページで制御します。
* 最優先 (デバッグモード)
* デフォルトの非表示：ここで選択するオプションは、「非表示」アイコンをクリックしたときに、Marketoの「最優先」タブに最適なコンテンツが表示されなくなる日数です
* 連絡先ステータスフィールド：ここで選択するオプションは、Marketoの「最優先」タブの「ステータスヘッダー」列に入力される値です
* ライブフィード設定：ライブフィードのみを表示するオプション ( リード、連絡先、アカウント、商談パネル、およびグローバルMarketoページ )、リードフィードのみを表示するオプション (Marketoグローバルページ内 )、またはライブとリードフィードの両方を表示するオプション
* タブ設定：デフォルトでは、5 つのタブすべてが使用可能になります。 Marketoグローバルページでタブの順序を選択できます

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-3.png)

**制限**

* アクティビティ（注目のアクティビティ、Web アクティビティ、電子メール）は、デフォルトで 1000 に設定されています。 電子メールキャンペーンとイベントは、デフォルトで 200 に設定されています
* 組織でタイムアウトの問題が発生した場合は、制限を減らすことができます

**アクション設定**

* Marketoメールの送信：これを有効にすると、すべての Sales Insight ユーザーがリード、連絡先、アカウント、商談のパネル、および「最優先」タブ（一括アクションとインラインエンゲージメント）からメールを送信するためのアクセス権を付与されます
* Marketo Campaign に追加：これを有効にすると、すべての Sales Insight ユーザーがリード、連絡先、アカウント、商談パネル、「Best Bets」タブ（一括アクションとインラインエンゲージメント）からキャンペーンに追加できるようになります

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-4.png)

## Marketo Sales Insight をリセット {#reset-marketo-sales-insight}

これを選択すると、SFDC 内のすべての設定が消去され、復元できなくなります。 すべてを再度設定する必要があります。

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-5.png)

>[!MORELIKETHIS]
>
>[チーム向けの Sales Insight の設定](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/setting-up-sales-insight-for-your-team.md)
