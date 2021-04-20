---
unique-page-id: 42762322
description: Salesforceの「MarketoSales Insight設定」タブ —Marketoドキュメント — 製品ドキュメント
title: Salesforceの「MarketoSales Insight設定」タブ
exl-id: 4e2abd48-b0a5-4b71-939b-e66c7e39bb6c
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---

# SalesforceのMarketoSales Insight設定タブ{#marketo-sales-insight-configuration-tab-in-salesforce}

## 操作設定{#operational-settings}

SFDCでSales Insightを使用して開始を行うには、この設定を行う必要があります。

![](assets/one.png)

* MSIはSoap APIとRest APIの両方を使用
* MarketoアカウントのSales Insightページには、SoapおよびRest APIの秘密鍵証明書を含む2つのパネルが表示され、ここにコピーして貼り付けることができます
* Soap APIとRest APIには、組織のニーズに基づいて設定できる個別のタイムアウトがあります。 最大時間は120秒です
* インサイトダッシュボードを無効にする：Rest API証明書は削除でき、Soap APIのみを使用できます。 これを行うと、すべてのMSI visualforceパネルの「インサイトのダッシュボード」タブが無効になります

## MSI設定{#msi-configuration}

設定は、すべてのMSIユーザーに適用され、プロファイルに固有のものではありません。

**Marketoタブ設定**

* 最優先 (デバッグモード)
* デフォルトの非表示 — ここで選択するオプションは、「非表示」アイコンをクリックしたときに、Marketoの「おすすめコンテンツ」タブにおすすめコンテンツが表示されなくなる日数です
* 連絡先ステータスフィールド — ここで選択するオプションは、Marketoの「おすすめコンテンツ」タブにある「ステータスヘッダー」列に入力される値です
* タブの設定 — デフォルトでは、5つのタブすべてが使用可能になります。 Marketoのグローバルページでは、タブの順序を選択できます

**Visualforceページ設定**

* 「アクションを有効にする」ドロップダウンリスト：

   * 「Lead &amp; Contact MSI Layout」のドロップダウンから「SendMarketo」電子メールを隠す機能
   * 「Lead &amp; Contact MSI Layout」のドロップダウンから追加Marketoキャンペーンに対して非表示にする機能

* 今後のイベント:招待イベント、ユーザーに対するすべてのイベントを表示したり、このタブを完全に非表示にしたりする機能
* 今後のキャンペーン:すべての電子メールキャンペーンを表示するか、このタブを完全に非表示にするかを指定できます
* 今後のキャンペーンおよびイベントの読み込み：ユーザーが実行するREST API呼び出しの数を減らす機能。イベントとキャンペーンのタブをオンデマンドの「今後の項目を読み込む」ボタンの後ろに配置します。
* タブの設定 — デフォルトでは、5つのタブすべてが使用可能になります。 デフォルトでは、5つのタブすべてが使用可能になります。 Sales Insightパネルでタブの順序を選択できます。 同じ注文がすべてのレイアウト（リード、連絡先、アカウント、オポチュニティ）に適用されます。

![](assets/two.png)

**制限**

* アクティビティ(注目の瞬間、ウェブアクティビティ、電子メール)は、デフォルトで1000に設定されています。 電子メールのキャンペーンとイベントは、デフォルトで200に設定されています
* 組織でタイムアウトに関する問題が発生した場合に備えて、制限を減らすことができます

## Marketo販売インサイトのリセット{#reset-marketo-sales-insight}

これを選択すると、SFDC内のすべての設定が消去され、復元できなくなります。 すべての設定を再度行う必要があります。

![](assets/three.png)

>[!MORELIKETHIS]
>
>[チーム向けのSales Insightの設定](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/setting-up-sales-insight-for-your-team.md)
