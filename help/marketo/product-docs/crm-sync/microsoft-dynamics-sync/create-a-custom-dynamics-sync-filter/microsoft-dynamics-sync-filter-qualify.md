---
unique-page-id: 10092977
description: Microsoft Dynamics Sync フィルター - 認定 - Marketo ドキュメント - 製品ドキュメント
title: Microsoft Dynamics Sync フィルター - 認定
exl-id: 9b26795c-fc94-478e-a7f0-ac8e602792b1
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '116'
ht-degree: 64%

---

# [!DNL Microsoft Dynamics] 同期フィルター：適合 {#microsoft-dynamics-sync-filter-qualify}

[!DNL Microsoft Dynamics] でリードを連絡先に変換する場合は、このデフォルトの選定プロセスを必ず使用してください。 次に、Marketo と同期します。

## 変換プロセス {#the-conversion-process}

変換プロセス中のフィルターの仕組みを次に示します。

| リード同期フィルター： | 取引担当者同期フィルター： | Marketo での結果 |
|---|---|---|
| [!UICONTROL False] | [!UICONTROL False] | Marketo では何も同期されない |
| [!UICONTROL True] | [!UICONTROL True] | 取引担当者が Marketo で同期される |
| [!UICONTROL False] | [!UICONTROL True] | Marketo で新しい取引担当者レコードが作成される |
| [!UICONTROL True] | [!UICONTROL False] | [!DNL MS Dynamics] はMarketoでリード情報を更新しますが、連絡先レコードは同期されません |

>[!CAUTION]
>
>アドビでは、標準の認定コンバージョンプロセスのみをサポートしています。
