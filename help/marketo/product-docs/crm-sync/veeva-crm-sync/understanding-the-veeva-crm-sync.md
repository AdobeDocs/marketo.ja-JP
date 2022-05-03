---
description: Veeva CRM 同期について — Marketoドキュメント — 製品ドキュメント
title: Veeva CRM 同期について
hide: true
hidefromtoc: true
source-git-commit: 93e6bb881e10cda26b3a33569dc67627d628a178
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 10%

---

# Veeva CRM 同期について {#understanding-the-veeva-crm-sync}

いくつかの簡単な手順で、Adobe Marketo Engageと Veeva CRM 間の同期を簡単に実行できます。

## 同期の仕組み {#how-the-sync-works}

Marketo Engageは毎日 Veeva CRM と同期します。 各同期には時間がかかり、5 分間一時停止した後、再び開始します。

>[!NOTE]
>
>最初の同期には、Marketo Engageが Veeva からデータベース全体をコピーするので、数時間から数日かかる場合があります。 その後、各同期には通常数分（秒）かかり、変更されたデータのみが同期されます。

![](assets/understanding-the-veeva-sync-1.png)

Veeva とMarketo Engageの同期は、担当者アカウントオブジェクトの連絡先フィールドに対してのみ双方向です。 この場合、Veeva またはMarketo Engageで変更を加えると、常に両方のシステムで更新が反映されます。 その他の同期はすべて Veeva からMarketo Engageのみです。 詳しくは、次のリンクをクリックしてください。

## Marketo Engageと Veeva 間の同期内容 {#what-is-synced-between-marketo-engage-and-veeva}

* 担当者アカウント
* ユーザー
* 呼び出しおよび呼び出しキーオブジェクト
* カスタムオブジェクト

## 留意事項 {#things-to-know}

* Veeva のMarketo Engageに入力した資格情報は、データの同期に使用されます。 その認証情報でアクセスできるデータのみが含まれます。

* Veeva CRM は force.com に基づいており、プラットフォームとのリッチエクスペリエンスMarketo Engageがこの同期に継承されます。

* Veeva CRM には次の内容が表示されます。リード、連絡先、アカウント（ビジネスアカウント、商談、キャンペーン、アクティビティ） ただし、Marketo Engageとの同期ではサポートされていません。
