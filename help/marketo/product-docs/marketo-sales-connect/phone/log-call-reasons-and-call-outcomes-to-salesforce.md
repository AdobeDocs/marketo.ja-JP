---
description: Salesforce に対するログ呼び出し理由と呼び出し結果 — Marketoドキュメント — 製品ドキュメント
title: Salesforce に通話理由と通話結果を記録
hide: true
hidefromtoc: true
source-git-commit: 1dd4a4f6bfac0b101f85f3776396aeef1a1f7182
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 5%

---

# Salesforce に通話理由と通話結果を記録 {#log-call-reasons-and-call-outcomes-to-salesforce}

レポートや表示の目的で、通話の結果や通話理由を Salesforce に記録したい場合は、それぞれにカスタムアクティビティフィールドを作成できます。 各フィールドは、特定の API 名を使用する必要があります。

* コールアウトカム API 名：mktosales_call_outcome
* 呼び出し理由 API 名：mktosales_call_reason

これらのフィールドを利用するには、まず、カスタムアクティビティフィールドとしてフィールドを作成する必要があります。 ユーザーに表示するには、タスクオブジェクトのページレイアウトに追加する必要があります。

## Salesforce Classic でカスタムアクティビティフィールドを作成  {#create-custom-activity-field-in-salesforce-classic}

1. Salesforce で、「セットアップ」に移動します。

PICC

1. [ クイック検索 ] ボックスに&quot;アクティビティ&quot;と入力します。

PICC

1. クリック **アクティビティカスタムフィールド**.

PICC

1. 「**新規**」をクリックします。

PICC

## Salesforce Lightning でカスタムアクティビティフィールドを作成 {#create-custom-activity-field-in-salesforce-lightning}

1. Salesforce で、右上の歯車アイコンをクリックします。

PICC

1. クリック **設定**.

PICC

1. クリック **オブジェクトマネージャ**.

PICC

1. 「クイック検索」ボックスに「アクティビティ」と入力し、アクティビティラベルをクリックして、オブジェクトの設定を開きます。

PICC

1. 左側で、 **フィールドと関係**.

PICC

1. 「**新規**」をクリックします。

PICC

## Salesforce Classic のタスクページレイアウトにカスタムアクティビティフィールドを追加 {#add-custom-activity-field-to-task-page-layout-in-salesforce-classic}

手順

## Salesforce Lightning のタスクページレイアウトにカスタムアクティビティフィールドを追加 {#add-custom-activity-field-to-task-page-layout-in-salesforce-lightning}

手順

>[!MORELIKETHIS]
>
>[アクティビティ履歴への Sales Connect イベントフィールドのインストール](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/install-sales-connect-event-fields-on-activity-history.md)
