---
description: メールの [!DNL Velocity]  スクリプトの親カスタムオブジェクト取得制限を増減します（10 ～ 100）。
title: ' [!DNL Velocity Scripting]でのカスタムオブジェクト取得制限の変更'
exl-id: ef45205e-421d-4d1d-8c9d-7d627326a90c
feature: Email Setup
TQID: https://experienceleague.adobe.com/8zdwliEWuUxePbN3RyElJZydMfPHO8sQbgZbaTda6iY
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 256
ht-degree: 51%

---

# [!DNL Velocity Scripting] でのカスタムオブジェクト取得制限の変更 {#change-custom-object-retrieval-limits-in-velocity-scripting}

[!DNL Velocity Script]を使用してメールでカスタムオブジェクトデータを表示する場合、この機能はユースケースに適用される場合があります。 デフォルトでは、Velocity Scriptから10個の親カスタムオブジェクトにアクセスできます。 さらにアクセスする必要がある場合は、以下の手順を参照してください。

## [!DNL Velocity] とは {#what-is-velocity}

[[!DNL Apache Velocity]](https://velocity.apache.org/) は、HTML コンテンツのテンプレート化とスクリプティングのために設計された [!DNL Java] で構築された言語です。 Marketoでは、[&#x200B; スクリプトトークン &#x200B;](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md)を使用して、メールのコンテキストで使用できます。 これにより、カスタムオブジェクトに保存されたデータにアクセスできます。

リードまたは取引先責任者に直接接続されている親と子のカスタムオブジェクトを参照できますが、サードレベルのカスタムオブジェクトは参照できません。 各カスタムオブジェクトに対して、人物／取引先責任者ごとの最近更新された 10 個のレコードが実行時に使用可能で、最新の更新（0 番目）から最も古い更新（9 番目）まで順番に並べられます。

## 制限の変更方法 {#how-to-change-the-limit}

1. 「**[!UICONTROL 管理者]**」セクションに移動します。

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-1.png)

1. 「**[!UICONTROL メール]**」をクリックします。

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-2.png)

1. [!UICONTROL カスタムオブジェクト取得制限]テーブルで、新しい[!UICONTROL 親の取得制限]を入力し、「**[!UICONTROL 変更を保存]**」をクリックします。

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-3.png)

>[!NOTE]
>
>[!UICONTROL 親検索制限]の値は10 ～ 100の範囲である必要があります。 [!UICONTROL 子の取得制限]が自動的に設定されます。 これは、1000 を[!UICONTROL 親の取得制限]で割ることで得られます。 例えば、親の制限を 50 に設定した場合、子の制限は 20 になります（1000 ÷ 50 = 20）。

[!DNL Velocity script]からさらにカスタムオブジェクトにアクセスできるようになりました。
