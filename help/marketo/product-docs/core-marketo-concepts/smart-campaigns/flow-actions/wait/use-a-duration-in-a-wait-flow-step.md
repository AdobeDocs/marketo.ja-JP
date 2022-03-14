---
unique-page-id: 1146978
description: 待機フローステップで停止期間を使用 - Marketo ドキュメント - 製品ドキュメント
title: 待機フローステップで停止期間を使用
exl-id: 7b13d225-78ba-4ef1-9ff5-0f6acde6e5ff
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '203'
ht-degree: 100%

---

# 待機フローステップで停止期間を使用 {#use-a-duration-in-a-wait-flow-step}

待機フローステップを使用すると、スマートキャンペーンを通じて一定期間、個人のジャーニーを一時停止できます。また、曜日と終了時刻の条件も指定できます。

1. スマートキャンペーン「**フロー**」タブに、「**待機**」フローステップをドラッグします。

   ![](assets/image2014-9-22-11-3a53-3a57.png)

1. 一時停止する期間を入力します。

   ![](assets/image2014-9-22-11-3a54-3a0.png)

1. これで完了です。フローは、指定された期間一時停止します。詳細設定オプションについては、右側の歯車アイコンをクリックします。

   ![](assets/image2014-9-22-11-3a54-3a7.png)

1. 待機ステップを終了する曜日を指定します。

   ![](assets/image2014-9-22-11-3a54-3a10.png)

1. 必要に応じて、時刻を指定します。「**保存**」をクリックします。

   ![](assets/image2014-9-22-11-3a54-3a35.png)

   >[!NOTE]
   >
   >**例**
   >
   >ある人が金曜日の午後 5 時にスマートキャンペーンをトリガーします。待機ステップは、48 時間、月～金曜日の午前 9 時に終了、といったように詳細に設定します。
   >
   >その結果、その人は&#x200B;**月曜日午前 9 時**&#x200B;にフローを続行することになります。これは、48 時間後、月～金曜日の中で最初に該当するものです。

   >[!NOTE]
   >
   >期間、日付、時間、使用日数はすべて、ご利用のサブスクリプションのタイムゾーンに基づきます。

   >[!MORELIKETHIS]
   >
   >* [待機フローステップで特定の日付を使用](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)
   >* [待機フローステップで日付トークンを使用](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-date-token-in-a-wait-flow-step.md)

