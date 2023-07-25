---
unique-page-id: 10092977
description: Microsoft Dynamics Sync フィルター - 認定 - Marketo ドキュメント - 製品ドキュメント
title: Microsoft Dynamics Sync フィルター - 認定
exl-id: 9b26795c-fc94-478e-a7f0-ac8e602792b1
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 100%

---

# Microsoft Dynamics Sync フィルター：認定 {#microsoft-dynamics-sync-filter-qualify}

リードを Microsoft Dynamics の取引担当者に変換する場合は、このデフォルトの適合プロセスを使用するようにしてください。次に、Marketo と同期します。

## 変換プロセス {#the-conversion-process}

変換プロセス中のフィルターの仕組みを次に示します。

| リード同期フィルター： | 取引担当者同期フィルター： | Marketo での結果 |
|---|---|---|
| False | False | Marketo では何も同期されない |
| True | True | 取引担当者が Marketo で同期される |
| False | True | Marketo で新しい取引担当者レコードが作成される |
| True | False | MS Dynamics によって Marketo のリード情報が更新されるが、取引担当者レコードは同期されない |

>[!CAUTION]
>
>アドビでは、標準の認定コンバージョンプロセスのみをサポートしています。
