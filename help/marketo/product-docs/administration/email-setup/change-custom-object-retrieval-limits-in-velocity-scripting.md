---
description: メールの[!DNL Velocity] スクリプトの親カスタムオブジェクト取得制限を増減します（10から100）。
title: '[!DNL Velocity Scripting] でのカスタムオブジェクト取得制限の変更'
exl-id: ef45205e-421d-4d1d-8c9d-7d627326a90c
feature: Email Setup
TQID: 'https://experienceleague.adobe.com/8zdwliEWuUxePbN3RyElJZydMfPHO8sQbgZbaTda6iY'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
    internal-label: Configuration
subfeature_v2:
  - id: a03c57fb-0705-4a0d-b463-bbc931d4cefa
    internal-label: Email setup
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 53%
---
# [!DNL Velocity Scripting] でのカスタムオブジェクト取得制限の変更 {#change-custom-object-retrieval-limits-in-velocity-scripting}

[!DNL Velocity Script]を使用してメールでカスタムオブジェクトデータを表示する場合、この機能はユースケースに適用される場合があります。 デフォルトでは、Velocity Scriptから10個の親カスタムオブジェクトにアクセスできます。 さらにアクセスする必要がある場合は、以下の手順を参照してください。

## [!DNL Velocity] とは {#what-is-velocity}

[[!DNL Apache Velocity]](https://velocity.apache.org/) は、HTML コンテンツのテンプレート化とスクリプティングのために設計された [!DNL Java] で構築された言語です。 Marketoでは、[ スクリプトトークン ](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md)を使用して、メールのコンテキストで使用できます。 これにより、カスタムオブジェクトに保存されたデータにアクセスできます。

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
