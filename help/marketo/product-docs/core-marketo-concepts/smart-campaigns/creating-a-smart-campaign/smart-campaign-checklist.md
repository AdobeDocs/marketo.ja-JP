---
unique-page-id: 1147051
description: スマートキャンペーンのチェックリスト - Marketo ドキュメント - 製品ドキュメント
title: スマートキャンペーンのチェックリスト
exl-id: 3c0d08c9-66ae-4083-ab0a-fa5a95149aba
source-git-commit: 56d3d05d5462c79f32f507655266e3bfa0cc6846
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# スマートキャンペーンのチェックリスト {#smart-campaign-checklist}

スマートキャンペーンを円滑に実行し、エラーをできるだけ防ぐには、次の手順に従います。

## スマートリストのエラーの除去 {#get-rid-of-smart-list-errors}

スマートキャンペーンで、 **スマートリスト**. 赤い波線が下に表示されている部分はエラー箇所なので、すべて修正します。

![](assets/smart-campaign-checklist-1.png)

>[!TIP]
>
>赤い波線は、エラーまたは情報が見つからないことを示します。修正されない場合、キャンペーンは無効になり、実行されません。
>
>また、**シンプルな構成**&#x200B;のスマートリストを心がけるようにします。何十、あるいは何百ものフィルターが含まれる場合、維持とトラックが困難になります。フィルターが少ないほどロード時間も速まります。

>[!NOTE]
>
>**スマートリストのメンバー**&#x200B;を使用した場合、他のリストにエラーが発生することがあるので、この点も問題がないか確認します。

## フローのエラーの除去 {#get-rid-of-flow-errors}

スマートキャンペーンで、 **フロー**. 赤い波線が表示されている部分はエラー箇所なので、すべて修正します。

![](assets/smart-campaign-checklist-2.png)

>[!TIP]
>
>赤い波線の箇所にマウスオーバーすると、エラーの詳細が表示されます。

## 「スケジュール」タブのレビュー {#review-the-schedule-tab}

内 **スケジュール** タブ、チェック **スマート** **リスト** **ステータス** 修正が必要なスマートキャンペーンのエラー。

![](assets/smart-campaign-checklist-3.png)

## リード制限数の確認 {#check-person-restrictions-limit}

「**スケジュール**」タブ内で、条件を満たすリード数がリード制限数を越えていないかを確認します。

![](assets/smart-campaign-checklist-4.png)

>[!TIP]
>
>必要に応じて、 [スマートキャンペーンでの担当者制限の上書き](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/override-person-restrictions-in-a-smart-campaign.md).

>[!NOTE]
>
>**リマインダー**
>
>それでもスマートキャンペーンが失敗する場合は、 [通知について](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications.md) 何が起こったのか、どのように修正すればよいのかを調べるために

完成です。スマートキャンペーンを実行する前に、このチェックリストを手元に用意してください。
