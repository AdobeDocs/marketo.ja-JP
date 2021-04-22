---
unique-page-id: 10092969
description: Microsoft Dynamics Sync Filter -Merge -Marketoドキュメント — 製品ドキュメント
title: Microsoft Dynamics同期フィルタ — 結合
exl-id: f8da9c3c-0f04-4f61-be03-7e7953d25afe
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 4%

---

# Microsoft Dynamics同期フィルタ：{#microsoft-dynamics-sync-filter-merge}を結合

Microsoft Dynamicsでリードをマージする際に、同期フィルター=はい(TRUE)と同期フィルター=いいえ(FALSE)の2つのオプションタイプが使用されます。 2つのレコードを結合する場合、結果は、TrueとFalseのレコードによって異なります。

リードレコードは、勝者を決定するために管理者が定義したワークフロールールに基づいて、真か偽になります。 勝者レコードの同期フィルターは、最終的にMS DynamicsレコードがMarketoと同期するかどうかを決定します。

一つのレコードが真で、一つは偽の場合、それが難しくなります。

| 失われるレコードの同期フィルタが次の場合： | 勝者レコードの同期フィルターは次のとおりです。 | これがMarketoの結果だ |
|---|---|---|
| True | True | 勝者レコードはMarketoと同期し続ける |
| False | False | 勝者レコードは&#x200B;**** Marketoと同期しません |
| False | True | 勝者レコードはMarketoと同期します |
| True | False | 勝者レコードはMarketoと同期しません |
