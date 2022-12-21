---
unique-page-id: 1146997
description: 待機フローステップで日付トークンを使用 - Marketo ドキュメント - 製品ドキュメント
title: 待機フローステップで日付トークンを使用
exl-id: d161922b-ce90-4e65-9282-d3bb866c1d94
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 100%

---

# 待機フローステップで日付トークンを使用 {#use-a-date-token-in-a-wait-flow-step}

待機フローステップを使用すると、スマートキャンペーンを通じて、日付トークンを使用する特定の日付まで、人のジャーニーを一時停止できます。また、終了日を日数で変更することもできます。

>[!NOTE]
>
>これは、トリガーキャンペーンにのみ適用されます。この機能はバッチキャンペーンでは使用できません。

1. スマートキャンペーン「**フロー**」タブに、「**待機**」フローステップをドラッグします。

   ![](assets/image2014-9-22-14-3a8-3a22.png)

1. 右側の歯車アイコンをクリックします。

   ![](assets/image2014-9-22-14-3a8-3a37.png)

1. 「**タイプ**」ドロップダウンで、「**日付トークン**」を選択します。

   ![](assets/image2014-9-22-14-3a8-3a41.png)

1. 日付トークンを選択して、待機ステップを終了するタイミングを指定します。

   * `{{my._____}}`
   * `{{lead.______}}`
   * `{{company.______}}`
   * `{{system._______}}`

   ![](assets/image2014-9-22-14-3a9-3a33.png)

1. 今年または翌年に発生する次のイベント日まで待つには、チェックボックスをオンにします。

   ![](assets/image2014-9-22-14-3a9-3a37.png)

   >[!TIP]
   >
   >このオプションは、誕生日や契約の開始日など、過去の日付を参照する日付トークンに対して使用します。

1. 必要に応じて、終了日を指定した日数で変更できます。

   ![](assets/image2014-9-22-14-3a9-3a57.png)

   >[!NOTE]
   >
   >また、整数フィールドを表す `{{lead.` または `{{company.` トークンを使用するか、`{{my.` 番号タイプのトークンを使用して、日数を指定することもできます。

1. 「**保存**」をクリックします。

   ![](assets/image2014-9-22-14-3a11-3a3.png)

   >[!MORELIKETHIS]
   >
   >* [待機フローステップで停止期間を使用](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md)
   >* [待機フローステップで特定の日付を使用](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)

