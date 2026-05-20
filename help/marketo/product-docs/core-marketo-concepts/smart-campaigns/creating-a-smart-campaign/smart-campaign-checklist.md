---
unique-page-id: 1147051
description: スマートキャンペーンに関するヘルプを参照してください。 このリストを使用して、アクティブ化する前にキャンペーンが正しく設定されていることを確認します。
title: スマートキャンペーンのチェックリスト
exl-id: 3c0d08c9-66ae-4083-ab0a-fa5a95149aba
feature: Smart Campaigns
TQID: https://experienceleague.adobe.com/R94BEUOHsfCoIwAvl7QKDRvBw5mU3szqH6n27qd3yk0
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 257
ht-degree: 70%

---

# スマートキャンペーンのチェックリスト {#smart-campaign-checklist}

スマートキャンペーンをスムーズに実行し、可能な限りエラーを防ぐには、以下の手順に従います。

## スマートリストのエラーの除去 {#get-rid-of-smart-list-errors}

スマートキャンペーンで、「**[!UICONTROL スマートリスト]**」をクリックします。 赤い波線が下に表示されている部分はエラー箇所なので、すべて修正します。

![](assets/smart-campaign-checklist-1.png)

>[!TIP]
>
>赤い波線は、エラーまたは情報が見つからないことを示します。 修正されない場合、キャンペーンは無効になり、実行されません。
>
>シンプルなユースケースを。 何十個または何百個ものフィルターがある場合、それを維持して追跡するのは困難です。 フィルターが少ないほどロード時間も速まります。

>[!NOTE]
>
>**[!UICONTROL スマートリストのメンバー]**&#x200B;を使用した場合、他のリストにエラーが発生することがあるので、 この点も問題がないか確認します。

## フローのエラーの除去 {#get-rid-of-flow-errors}

スマートキャンペーンで、「**[!UICONTROL 結果]**」をクリックします。 赤い波線が表示されている部分はエラー箇所なので、すべて修正します。

![](assets/smart-campaign-checklist-2.png)

>[!TIP]
>
>赤い波線の箇所にマウスオーバーすると、エラーの詳細が表示されます。

## 「スケジュール」タブのレビュー {#review-the-schedule-tab}

「**[!UICONTROL スケジュール]**」タブで、**[!UICONTROL スマートリストステータス]**&#x200B;で、修正が必要なスマートキャンペーンのエラーを確認します。

![](assets/smart-campaign-checklist-3.png)

## リード制限数の確認 {#check-person-restrictions-limit}

「**[!UICONTROL スケジュール]**」タブで、適格なユーザーの数がユーザー制限の制限を超えていないことを確認します。

![](assets/smart-campaign-checklist-4.png)

>[!TIP]
>
>必要に応じて、[スマートキャンペーンでリード制限数を上書き](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/override-person-restrictions-in-a-smart-campaign.md)できます。

>[!NOTE]
>
>**リマインダー**
>
>以上を行ってもスマートキャンペーンがうまく機能しない場合、何が原因でどこを修正すればいいのか、[通知の内容によく目を通して詳細を確認](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications.md)してください。

スマートキャンペーンを実行するときは、常にこのチェックリストで内容を点検してください。
