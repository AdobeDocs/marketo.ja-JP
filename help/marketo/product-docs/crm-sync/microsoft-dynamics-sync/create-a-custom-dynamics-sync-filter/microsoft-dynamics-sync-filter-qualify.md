---
unique-page-id: 10092977
description: Microsoft Dynamics Sync Filter — 資格 —Marketoドキュメント — 製品ドキュメント
title: Microsoft Dynamics Sync Filter — 条件付き
exl-id: 9b26795c-fc94-478e-a7f0-ac8e602792b1
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 6%

---

# Microsoft Dynamics同期フィルタ：{#microsoft-dynamics-sync-filter-qualify}に適合

Microsoft Dynamicsでリードを連絡先に変換する場合は、この既定の「限定処理」を必ず使用してください。 それから、Marketoと同期して。

## 変換プロセス{#the-conversion-process}

変換プロセス中のフィルターの動作は次のとおりです。

| リード同期フィルタが次の場合： | 連絡先の同期フィルタは次のとおりです。 | これがMarketoの結果だ |
|---|---|---|
| False | False | Marketoでは何も同期されません |
| True | True | 連絡先はMarketoで同期されています |
| False | True | 新しい連絡先レコードがMarketoに作成されました |
| True | False | MS Dynamicsは、Marketoのリード情報を更新しましたが、連絡先レコードは同期されません |

>[!CAUTION]
>
>デルは、すぐに使用できる「コンバージョンの認定」プロセスのみをサポートします。
