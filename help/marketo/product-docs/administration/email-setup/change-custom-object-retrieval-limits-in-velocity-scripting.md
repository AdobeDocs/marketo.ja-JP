---
description: " [!DNL Velocity Scripting]  でのカスタムオブジェクト取得制限の変更 - Marketo ドキュメント - 製品ドキュメント"
title: " [!DNL Velocity Scripting] でのカスタムオブジェクト取得制限の変更"
exl-id: ef45205e-421d-4d1d-8c9d-7d627326a90c
feature: Email Setup
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 100%

---

# [!DNL Velocity Scripting] でのカスタムオブジェクト取得制限の変更 {#change-custom-object-retrieval-limits-in-velocity-scripting}

[!DNL Velocity Script] を使用してメールにカスタムオブジェクトデータを表示する場合、この機能が役に立つでしょう。デフォルトでは、Velocity スクリプトから 10 個の親カスタムオブジェクトにアクセスできます。詳しくは、以下を参照してください。

## [!DNL Velocity] とは {#what-is-velocity}

[[!DNL Apache Velocity]](https://velocity.apache.org/) は、HTML コンテンツのテンプレート化とスクリプティングのために設計された [!DNL Java] で構築された言語です。Marketo では、[スクリプトトークン](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md)の使用を通じて、メールのコンテキストで使用できます。これにより、カスタムオブジェクトに保存されたデータにアクセスできます。

リードや取引先責任者に直接接続されているが、第 3 レベルのカスタムオブジェクトには接続していない、親および子のカスタムオブジェクトを参照できます。各カスタムオブジェクトに対して、人物／取引先責任者ごとの最近更新された 10 個のレコードが実行時に使用可能で、最新の更新（0 番目）から最も古い更新（9 番目）まで順番に並べられます。

## 制限の変更方法 {#how-to-change-the-limit}

1. 「**[!UICONTROL 管理者]**」セクションに移動します。

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-1.png)

1. 「**[!UICONTROL メール]**」をクリックします。

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-2.png)

1. [!UICONTROL カスタムオブジェクト取得制限]テーブルで、新しい[!UICONTROL 親の取得制限]を入力し、「**[!UICONTROL 変更を保存]**」をクリックします。

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-3.png)

>[!NOTE]
>
>[!UICONTROL 親の取得制限]値は 10 ～ 100 の範囲にする必要があります。[!UICONTROL 子の取得制限]が自動的に設定されます。これは、1000 を[!UICONTROL 親の取得制限]で割ることで得られます。例えば、親の制限を 50 に設定した場合、子の制限は 20 になります（1000 ÷ 50 = 20）。

作業は以上です。これで、[!DNL Velocity script] からより多くのカスタムオブジェクトにアクセスできるようになりました。
