---
unique-page-id: 10092977
description: Microsoft Dynamics Sync フィルター - 認定 - Marketo ドキュメント - 製品ドキュメント
title: Microsoft Dynamics Sync フィルター - 認定
exl-id: 9b26795c-fc94-478e-a7f0-ac8e602792b1
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '116'
ht-degree: 100%

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
