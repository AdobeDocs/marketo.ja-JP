---
unique-page-id: 10092977
description: リードを連絡先に変換する際のDynamics同期フィルターの選定プロセスについて説明します。 リードと取引先責任者の同期フィルター値がMarketoの同期にどのような影響を与えるかを理解します。
title: Microsoft Dynamics Sync フィルター - 認定
exl-id: 9b26795c-fc94-478e-a7f0-ac8e602792b1
feature: Microsoft Dynamics
TQID: 'https://experienceleague.adobe.com/3jC9Y9fpBNjUzjE1Dy7JBuhNlYQpnc7kjF2LxV-hrp4'
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
source-wordcount: '124'
ht-degree: 66%
---
# [!DNL Microsoft Dynamics] 同期フィルター：認定 {#microsoft-dynamics-sync-filter-qualify}

リードを[!DNL Microsoft Dynamics]の連絡先に変換する場合は、このデフォルトの選定プロセスを使用します。 次に、Marketo と同期します。

## 変換プロセス {#the-conversion-process}

| リード同期フィルター： | 取引先担当者同期フィルターが次の値の場合： | Marketo での結果 |
|---|---|---|
| [!UICONTROL False] | [!UICONTROL False] | Marketo では何も同期されない |
| [!UICONTROL True] | [!UICONTROL True] | 取引先責任者が Marketo で同期される |
| [!UICONTROL False] | [!UICONTROL True] | Marketo で新しい取引先責任者レコードが作成される |
| [!UICONTROL True] | [!UICONTROL False] | [!DNL MS Dynamics] によって Marketo のリード情報が更新されるが、取引先責任者レコードは同期されない |

>[!CAUTION]
>
>アドビでは、標準の選定コンバージョンプロセスのみをサポートしています。
