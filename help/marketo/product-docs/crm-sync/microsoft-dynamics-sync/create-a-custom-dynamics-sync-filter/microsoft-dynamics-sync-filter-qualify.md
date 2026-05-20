---
unique-page-id: 10092977
description: リードを連絡先に変換する際のDynamics同期フィルターの選定プロセスについて説明します。 リードと取引先責任者の同期フィルター値がMarketoの同期にどのような影響を与えるかを理解します。
title: Microsoft Dynamics Sync フィルター - 認定
exl-id: 9b26795c-fc94-478e-a7f0-ac8e602792b1
feature: Microsoft Dynamics
TQID: https://experienceleague.adobe.com/3jC9Y9fpBNjUzjE1Dy7JBuhNlYQpnc7kjF2LxV-hrp4
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 124
ht-degree: 66%

---

# [!DNL Microsoft Dynamics] 同期フィルター：認定 {#microsoft-dynamics-sync-filter-qualify}

リードを[!DNL Microsoft Dynamics]の連絡先に変換する場合は、このデフォルトの選定プロセスを使用します。 次に、Marketo と同期します。

## 変換プロセス {#the-conversion-process}

| リード同期フィルター： | 取引担当者同期フィルター： | Marketo での結果 |
|---|---|---|
| [!UICONTROL False] | [!UICONTROL False] | Marketo では何も同期されない |
| [!UICONTROL True] | [!UICONTROL True] | 取引先責任者が Marketo で同期される |
| [!UICONTROL False] | [!UICONTROL True] | Marketo で新しい取引先責任者レコードが作成される |
| [!UICONTROL True] | [!UICONTROL False] | [!DNL MS Dynamics] によって Marketo のリード情報が更新されるが、取引先責任者レコードは同期されない |

>[!CAUTION]
>
>アドビでは、標準の認定コンバージョンプロセスのみをサポートしています。
