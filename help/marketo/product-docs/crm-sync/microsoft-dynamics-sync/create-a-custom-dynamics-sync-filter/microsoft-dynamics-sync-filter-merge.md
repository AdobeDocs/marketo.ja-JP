---
unique-page-id: 10092969
description: Microsoft Dynamics 同期フィルター - 結合 - Marketo ドキュメント - 製品ドキュメント
title: Microsoft Dynamics 同期フィルター - 結合
exl-id: f8da9c3c-0f04-4f61-be03-7e7953d25afe
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '172'
ht-degree: 100%

---

# Microsoft Dynamics 同期フィルター：結合 {#microsoft-dynamics-sync-filter-merge}

Microsoft Dynamics でリードを結合するときには、同期フィルターが「はい」（TRUE）、同期フィルターが「いいえ」（FALSE）の 2 つのオプションタイプが使用できます。2 つのレコードを結合すると、True のレコードと False のレコードによって結果が異なります。

勝者を決定するために管理者が定義したワークフロールールに基づいて、リードレコードは true または false になります。勝者レコードの同期フィルターは、MS Dynamics レコードが Marketo と同期するかどうかを最終的に決定するものです。

1 つのレコードが true で、1 つが false の場合、決定が難しくなります。

| 失われるレコードの同期フィルターが次の場合 | 勝者レコードの同期フィルターが次の場合 | Marketo での結果 |
|---|---|---|
| True | True | 勝者レコードは引き続き Marketo と同期 |
| False | False | 勝者レコードは引き続き Marketo と&#x200B;**同期しない** |
| False | True | 勝者レコードは Marketo と同期 |
| True | False | 勝者レコードは Marketo と同期しない |
