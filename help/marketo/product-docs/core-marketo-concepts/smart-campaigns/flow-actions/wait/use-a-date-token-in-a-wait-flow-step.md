---
unique-page-id: 1146997
description: 待機フロー手順 — Marketto Docs — 製品ドキュメントでの日付トークンの使用
title: 待機フロー手順での日付トークンの使用
translation-type: tm+mt
source-git-commit: 5b9f48c98464c79bcdca2e335f6a4a2edce98ce4
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---


# 待機フロー手順での日付トークンの使用{#use-a-date-token-in-a-wait-flow-step}

待機フローステップを使用すると、スマートキャンペーンを介して、日付トークンを使用する特定の日付まで人のジャーニーを一時停止できます。 終了日は、日数によって変更することもできます。

>[!NOTE]
>
>これは、トリガーキャンペーンにのみ適用されます。 この機能はバッチキャンペーンでは使用できません。

1. スマートキャンペーン&#x200B;**「フロー**」タブで、**待機**&#x200B;フローステップの上にドラッグします。

   ![](assets/image2014-9-22-14-3a8-3a22.png)

1. 右側の歯車アイコンをクリックします。

   ![](assets/image2014-9-22-14-3a8-3a37.png)

1. 「**タイプ**」ドロップダウンから、「**日付トークン**」を選択します。

   ![](assets/image2014-9-22-14-3a8-3a41.png)

1. 日付トークンを選択して、待機ステップを終了するタイミングを指定します。

   * `{{my._____}}`
   * `{{lead.______}}`
   * `{{company.______}}`
   * `{{system._______}}`

   ![](assets/image2014-9-22-14-3a9-3a33.png)

1. 現在または次の年に発生する日付の次の記念日まで待つには、チェックボックスをオンにします。

   ![](assets/image2014-9-22-14-3a9-3a37.png)

   >[!TIP]
   >
   >このオプションは、誕生日や契約開始日など、過去の日付を参照する日付トークンに対して使用します。

1. オプションで、終了日を指定した日数だけ変更できます。

   ![](assets/image2014-9-22-14-3a9-3a57.png)

   >[!NOTE]
   >
   >整数フィールドを表す`{{lead.`または`{{company.`トークン、または数値型の`{{my.`トークンを使用して、日数を指定することもできます。

1. 「**保存**」をクリックします。

   ![](assets/image2014-9-22-14-3a11-3a3.png)

   >[!MORELIKETHIS]
   >
   >* [待機フローステップでの期間の使用](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md)
   >* [特定の日付を待機フロー・ステップで使用](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)

