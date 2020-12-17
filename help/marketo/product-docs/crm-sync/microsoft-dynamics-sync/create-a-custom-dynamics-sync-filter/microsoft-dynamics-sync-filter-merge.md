---
unique-page-id: 10092969
description: Microsoft Dynamics Sync Filter -Merge - Marketto Docs — 製品ドキュメント
title: Microsoft Dynamics同期フィルタ — 結合
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 0%

---


# Microsoft Dynamics同期フィルタ：{#microsoft-dynamics-sync-filter-merge}を結合

Microsoft Dynamicsでリードをマージする際に、同期フィルター=はい(TRUE)と同期フィルター=いいえ(FALSE)の2つのオプションタイプが使用されます。 2つのレコードを結合する場合、結果は、TrueとFalseのレコードによって異なります。

リードレコードは、勝者を決定するために管理者が定義したワークフロールールに基づいて、真か偽になります。 勝者レコードの同期フィルターは、最終的にMS DynamicsレコードがMarketoと同期するかどうかを決定します。

一つのレコードが真で、一つは偽の場合、それが難しくなります。

| 失われるレコードの同期フィルタが次の場合： | 勝者レコードの同期フィルターは次のとおりです。 | これは、Marketo |
|---|---|---|
| True | True | 勝者レコードは引き続きマーケティング担当者と同期されます |
| False | False | 勝者レコードは引き続き&#x200B;**Marketoと**&#x200B;同期&lt;a1/>されません |
| False | True | 勝者レコードは、マーケティング担当者と同期されます |
| True | False | 勝者レコードはマーケティング担当者と同期されません |

