---
description: メール、ランディングページ、キャンペーンなど、あらゆるコンポーネントをまたいでベストプラクティスに関するプログラムを監査する方法について説明します。
title: プログラム QA
badge: ベータ版
exl-id: 51d4b2d8-44b0-4b51-851f-7cb233baf2d6
source-git-commit: ff71b9e2a743056f8efd64d3debdf498ee3e43df
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 2%

---

# プログラム QA {#program-qa}

メール、ランディングページ、キャンペーンなど、あらゆるコンポーネントをまたいでベストプラクティスのプログラムを監査します。

>[!AVAILABILITY]
>
>この機能は限定的に利用できます。 サブスクリプションへのアクセスをリクエストするには、Adobe アカウントチーム（アカウントマネージャー）にお問い合わせください。

>[!PREREQUISITES]
>
>この機能を使用するには、まず[Core Gen-AI条件と補足条件](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"}に同意する必要があります。 詳しくは、アカウントマネージャーにお問い合わせください。

## 使用方法 {#how-to-use}

1. マイMarketoで、**AIでビルド** タイルをクリックします。

   ![](assets/program-qa-1.png)

1. **プログラム QA** エージェントを選択します。

   ![](assets/program-qa-2.png)

   会話型AI画面が表示されます。

1. 右側のパネルで、QAを行うプログラムを選択します。

   ![](assets/program-qa-3.png){width="800" zoomable="yes"}

   選択したプログラムの概要が中央のペインに表示されます。

   ![](assets/program-qa-4.png){width="450" zoomable="yes"}

1. プロンプトウィンドウで、「QA プログラム」と入力し、**送信**&#x200B;をクリックします。

   ![](assets/program-qa-5.png)

   AI アシスタントが選択したプログラムのQAを表示し、何が合格し、何が失敗したかを示します。

   ![](assets/program-qa-6.png)

<!--
   You have three validation paths to choose from:

   | Path | What You Provide | Verification Type | Best For |
   | --- | --- | --- | --- |
   | Rules Only | Nothing | Compliance checks | Org compliance & audits |
   | + Test Plan | Your team's test document | Rules + Custom checks | Team or channel-specific checks |
   | + Campaign Brief | Campaign brief document | Exact field matching | Pre-launch readiness |

1. To Upload a Test Plan, a Campaign Brief, or both, click the upload icon, add your files and click **Send**. To proceed with rules only, enter "Proceed with Rules Only" in the prompt window and click **Send**. In this example, we are proceeding with rules only.

PICC

1. To start validation, click **Run QA Validation**.

PICC

1. The report generates. To see the full report, click View Full Report.

PICC

1. The report appears in the center console. Scroll down to view. You can also download the report via .docx file.

PICC
-->
