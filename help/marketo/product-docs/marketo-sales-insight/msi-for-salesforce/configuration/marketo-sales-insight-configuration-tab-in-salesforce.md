---
unique-page-id: 42762322
description: Salesforce - Marketto Docs — 製品ドキュメントの「Marketto Sales Insight Configuration」タブ
title: SalesforceのMarketo Sales Insightの「Configuration」タブ
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '398'
ht-degree: 0%

---


# SalesforceのMarketo Sales Insightの「Configuration」タブ {#marketo-sales-insight-configuration-tab-in-salesforce}

## 操作設定 {#operational-settings}

SFDCでSales Insightを使用して開始を行うには、この設定を行う必要があります。

![](assets/one.png)

* MSIはSoap APIとRest APIの両方を使用
* MarketoアカウントのSales Insightページには、SoapおよびRest API資格情報を含む2つのパネルが表示され、ここにコピーして貼り付けることができます
* Soap APIとRest APIには、組織のニーズに基づいて設定できる個別のタイムアウトがあります。 最大時間は120秒です
* インサイトダッシュボードを無効にする：Rest API証明書は削除でき、Soap APIのみを使用できます。 これを行うと、すべてのMSI visualforceパネルの「インサイトのダッシュボード」タブが無効になります

## MSI設定 {#msi-configuration}

設定は、すべてのMSIユーザーに適用され、プロファイルに固有のものではありません。

**マーケティングタブの設定**

* 最適なデバッグモード
* デフォルトの非表示 — ここで選択するオプションは、「非表示」アイコンをクリックしたときに、マーケティングの「おすすめコンテンツ」タブにおすすめコンテンツが表示されなくなる日数です
* 連絡先ステータスフィールド — ここで選択するオプションは、マーケティング担当者の「おすすめコンテンツ」タブにある「ステータスヘッダー」列に入力される値です
* タブの設定 — デフォルトでは、5つのタブすべてが使用可能になります。 Marketogetグローバルページでタブの順序を選択できます

**Visualforceページ設定**

* 「アクションを有効にする」ドロップダウンリスト：

   * 「Lead &amp; Contact MSI Layout」のドロップダウンからマーケティング担当者の電子メールを非表示にする機能
   * 「Lead &amp; Contact MSI Layout」のドロップダウン追加から、Marketorキャンペーンオプションを非表示にする機能

* 今後のイベント:招待イベント、ユーザーに対するすべてのイベントを表示したり、このタブを完全に非表示にしたりする機能
* 今後のキャンペーン:すべての電子メールキャンペーンを表示するか、このタブを完全に非表示にするかを指定できます
* タブの設定 — デフォルトでは、5つのタブすべてが使用可能になります。 デフォルトでは、5つのタブすべてが使用可能になります。 Sales Insightパネルでタブの順序を選択できます。 同じ注文がすべてのレイアウト（リード、連絡先、アカウント、オポチュニティ）に適用されます。

![](assets/two.png)

**制限**

* アクティビティ(注目の瞬間、ウェブアクティビティ、電子メール)は、デフォルトで1000に設定されています。 電子メールのキャンペーンとイベントは、デフォルトで200に設定されています
* 組織でタイムアウトに関する問題が発生した場合に備えて、制限を減らすことができます

## Markettor Sales Insightのリセット {#reset-marketo-sales-insight}

これを選択すると、SFDC内のすべての設定が消去され、復元できなくなります。 すべての設定を再度行う必要があります。

![](assets/three.png)

