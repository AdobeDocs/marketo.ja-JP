---
unique-page-id: 10092977
description: リードを連絡先に変換する際の Dynamics 同期フィルターの選定プロセスについて説明します。 リードおよび取引先責任者同期フィルターの値がMarketo同期に与える影響を理解します。
title: Microsoft Dynamics Sync フィルター - 認定
exl-id: 9b26795c-fc94-478e-a7f0-ac8e602792b1
feature: Microsoft Dynamics
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '133'
ht-degree: 80%

---

# [!DNL Microsoft Dynamics] 同期フィルター：認定 {#microsoft-dynamics-sync-filter-qualify}

リードを [!DNL Microsoft Dynamics] の取引先責任者に変換する場合は、このデフォルトの認定プロセスを使用するようにしてください。次に、Marketo と同期します。

## 変換プロセス {#the-conversion-process}

変換プロセス中のフィルターの仕組みを次に示します。

| リード同期フィルター： | 取引担当者同期フィルター： | Marketo での結果 |
|---|---|---|
| [!UICONTROL False] | [!UICONTROL False] | Marketo では何も同期されない |
| [!UICONTROL True] | [!UICONTROL True] | 取引先責任者が Marketo で同期される |
| [!UICONTROL False] | [!UICONTROL True] | Marketo で新しい取引先責任者レコードが作成される |
| [!UICONTROL True] | [!UICONTROL False] | [!DNL MS Dynamics] によって Marketo のリード情報が更新されるが、取引先責任者レコードは同期されない |

>[!CAUTION]
>
>アドビでは、標準の認定コンバージョンプロセスのみをサポートしています。
