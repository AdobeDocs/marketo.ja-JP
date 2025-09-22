---
unique-page-id: 1146997
description: 待機フローステップで日付トークンを使用 - Marketo ドキュメント - 製品ドキュメント
title: 待機フローステップで日付トークンを使用
exl-id: d161922b-ce90-4e65-9282-d3bb866c1d94
feature: Smart Campaigns
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 100%

---

# 待機フローステップで日付トークンを使用 {#use-a-date-token-in-a-wait-flow-step}

待機フローステップを使用すると、スマートキャンペーンを通じて、日付トークンを使用する特定の日付まで個人のジャーニーを一時停止できます。また、終了日を日数で変更することもできます。

>[!NOTE]
>
>これは、トリガーキャンペーンにのみ当てはまります。この機能はバッチキャンペーンでは使用できません。

1. スマートキャンペーンの「**[!UICONTROL フロー]**」タブで、**[!UICONTROL 待機]**&#x200B;フローステップをドラッグします。

   ![](assets/use-a-date-token-in-a-wait-flow-step-1.png)

1. 歯車アイコンをクリックします。

   ![](assets/use-a-date-token-in-a-wait-flow-step-2.png)

1. **[!UICONTROL タイプ]**&#x200B;ドロップダウンで、「**[!UICONTROL 日付トークン]**」を選択します。

   ![](assets/use-a-date-token-in-a-wait-flow-step-3.png)

1. 「[!UICONTROL 日付トークン]」を選択して、待機ステップを終了するタイミングを指定します。

   * `{{my._____}}`
   * `{{lead.______}}`
   * `{{company.______}}`
   * `{{system._______}}`

   ![](assets/use-a-date-token-in-a-wait-flow-step-4.png)

1. 今年または翌年に発生する次のイベント日まで待つには、チェックボックスをオンにします。

   ![](assets/use-a-date-token-in-a-wait-flow-step-5.png)

   >[!TIP]
   >
   >このオプションは、誕生日や契約の開始日など、過去の日付を参照する日付トークンに対して使用します。

1. 必要に応じて、終了日を指定した日数で変更できます。

   ![](assets/use-a-date-token-in-a-wait-flow-step-6.png)

   >[!NOTE]
   >
   >また、整数フィールドを表す `{{lead.` または `{{company.` トークンを使用するか、`{{my.` 番号タイプのトークンを使用して、日数を指定することもできます。

1. 「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/use-a-date-token-in-a-wait-flow-step-7.png)

   >[!MORELIKETHIS]
   >
   >* [待機フローステップで停止期間を使用](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md){target="_blank"}
   >* [待機フローステップで特定の日付を使用](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md){target="_blank"}
