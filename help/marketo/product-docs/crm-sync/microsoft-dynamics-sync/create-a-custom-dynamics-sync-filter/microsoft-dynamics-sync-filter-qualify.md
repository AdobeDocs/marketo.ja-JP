---
unique-page-id: 10092977
description: Microsoft Dynamics Sync Filter — 資格 — Marketto Docs — 製品ドキュメント
title: Microsoft Dynamics Sync Filter — 条件付き
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 0%

---


# Microsoft Dynamics同期フィルタ：{#microsoft-dynamics-sync-filter-qualify}に適合

Microsoft Dynamicsでリードを連絡先に変換する場合は、この既定の「限定処理」を必ず使用してください。 その後、Marketoと同期します。

## 変換プロセス{#the-conversion-process}

変換プロセス中のフィルターの動作は次のとおりです。

| リード同期フィルタが次の場合： | 連絡先の同期フィルタは次のとおりです。 | これは、Marketo |
|---|---|---|
| False | False | Marketoでは何も同期されません |
| True | True | 連絡先はMarketoで同期されます |
| False | True | 新しい連絡先レコードがMarketoに作成されます |
| True | False | MS DynamicsはMarketorのリード情報を更新しますが、連絡先レコードは同期されません |

>[!CAUTION]
>
>デルは、すぐに使用できる「コンバージョンの認定」プロセスのみをサポートします。
