---
unique-page-id: 10092969
description: Microsoft Dynamics 同期フィルター - 結合 - Marketo ドキュメント - 製品ドキュメント
title: Microsoft Dynamics 同期フィルター - 結合
exl-id: f8da9c3c-0f04-4f61-be03-7e7953d25afe
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 72%

---

# [!DNL Microsoft] Dynamics 同期フィルター：結合 {#microsoft-dynamics-sync-filter-merge}

[!DNL Microsoft Dynamics] でのリードの結合では、同期フィルター= Yes （TRUE）と同期フィルター= No （FALSE）の 2 つのオプションタイプを使用します。 2 つのレコードを結合すると、True のレコードと False のレコードによって結果が異なります。

勝者を決定するために管理者が定義したワークフロールールに基づいて、リードレコードは true または false になります。勝者レコードの同期フィルターは、実 [!DNL MS Dynamics] 者レコードがMarketoと同期されるかどうかを最終的に決定するものです。

1 つのレコードが true で、1 つが false の場合、決定が難しくなります。

| 失われるレコードの同期フィルターが次の場合 | 勝者レコードの同期フィルターが次の場合 | Marketo での結果 |
|---|---|---|
| [!UICONTROL True] | [!UICONTROL True] | 勝者レコードは引き続き Marketo と同期 |
| [!UICONTROL False] | [!UICONTROL False] | 勝者レコードは引き続き Marketo と&#x200B;**同期しない** |
| [!UICONTROL False] | [!UICONTROL True] | 勝者レコードは Marketo と同期 |
| [!UICONTROL True] | [!UICONTROL False] | 勝者レコードは Marketo と同期しない |
