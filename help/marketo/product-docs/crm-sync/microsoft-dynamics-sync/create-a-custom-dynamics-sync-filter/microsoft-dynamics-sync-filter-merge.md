---
unique-page-id: 10092969
description: リードを結合する際のDynamics同期フィルターの仕組みを説明します。 勝者レコードの同期フィルター値が、レコードがMarketoに同期されるかどうかを決定する方法を説明します。
title: Microsoft Dynamics 同期フィルター - 結合
exl-id: f8da9c3c-0f04-4f61-be03-7e7953d25afe
feature: Microsoft Dynamics
TQID: 'https://experienceleague.adobe.com/wxPBvOQk4SW8gocZOGfagAMAG4OH9ghTqhh0lVRGI-U'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
subfeature_v2:
  - id: d5c7388a-594e-4d15-9b39-98d6ce479e8b
    internal-label: Microsoft Dynamics
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 78%
---
# [!DNL Microsoft] Dynamics 同期フィルター：結合 {#microsoft-dynamics-sync-filter-merge}

[!DNL Microsoft Dynamics] でリードを結合するときには、同期フィルターが「はい」（TRUE）、同期フィルターが「いいえ」（FALSE）の 2 つのオプションタイプが使用できます。 2 つのレコードを結合すると、True のレコードと False のレコードによって結果が異なります。

勝者を決定するために管理者が定義したワークフロールールに基づいて、リードレコードは true または false になります。 勝者レコードの同期フィルターは、[!DNL MS Dynamics] レコードが Marketo と同期するかどうかを最終的に決定するものです。

ある記録が真実で、ある記録が真実で、ある記録が真実でない場合、それは難しくなる。

| 失われるレコードの同期フィルターが次の場合 | かつ、勝者レコードの同期フィルターが次の場合、 | Marketo での結果 |
|---|---|---|
| [!UICONTROL True] | [!UICONTROL True] | 勝ちレコードは引き続き Marketo と同期します |
| [!UICONTROL False] | [!UICONTROL False] | 勝者レコードは引き続き Marketo と&#x200B;**同期しない** |
| [!UICONTROL False] | [!UICONTROL True] | 勝ちレコードは Marketo と同期します |
| [!UICONTROL True] | [!UICONTROL False] | 勝者レコードは Marketo と同期しない |
