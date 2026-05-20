---
unique-page-id: 2953132
description: バッチおよびトリガースマートキャンペーンについて詳しく見る。 各タイプの用途と運用方法を把握できます。
title: バッチおよびトリガースマートキャンペーンについて
exl-id: 84a7b38c-b79c-4360-bd0b-3beb8ca35ac7
feature: Smart Campaigns
TQID: https://experienceleague.adobe.com/48wdmRPcrjaIavo4EQG3nkQNcUMH33tuISSqU2VouTM
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 275
ht-degree: 46%

---

# バッチおよびトリガースマートキャンペーンについて {#understanding-batch-and-trigger-smart-campaigns}

スマートキャンペーンには、バッチおよびトリガーの 2 種類があります。

## バッチキャンペーン {#batch-campaign}

>[!NOTE]
>
>**定義**
>
>バッチキャンペーンは、特定の時間に開始され、特定の一連のユーザーに一括で影響を与えます。 例えば、「東京都」にいるすべてのリードにメールを送信する場合に使用します。

バッチキャンペーンには、スマートリストセクション内のフィルターのみが含まれます（トリガーはありません）。

![](assets/understanding-batch-and-trigger-smart-campaigns-1.png)

「**[!UICONTROL スケジュール]**」タブをクリックすると、スマートキャンペーンが「バッチ」に設定されていることを確認できます。

![](assets/understanding-batch-and-trigger-smart-campaigns-2.png)

**バッチスマートキャンペーン**

* 毎日、毎週、毎月のように、繰り返しのスケジュール設定が可能です。 あるいは、単発で 1 回のみ実行するよう設定することも可能です。
* [プログラムスケジュール表示](/help/marketo/product-docs/core-marketo-concepts/programs/program-schedule-view/navigating-the-program-schedule-view.md){target="_blank"}に表示されます。 スマートキャンペーン内の「待機」ステップの後のものは、ビューに含まれません。

<br> 

## トリガーキャンペーン {#trigger-campaign}

>[!NOTE]
>
>**定義**
>
>トリガー施策は、トリガーされたイベントにもとづいて、一人ひとりに影響を与えます。 例えば、メール内のリンクがクリックされた場合です。

スマートキャンペーンで「スマートリスト」セクション内の少なくとも1つのトリガーを使用すると、自動的にトリガーされます。

![](assets/understanding-batch-and-trigger-smart-campaigns-3.png)

「**[!UICONTROL スケジュール]**」タブをクリックすると、スマートキャンペーンが「トリガー」に設定されていることを確認できます。

![](assets/understanding-batch-and-trigger-smart-campaigns-4.png)

**トリガーキャンペーン**

* 繰り返しのスケジュール設定はできません。 アクティブまたは非アクティブの設定のみです。
* トリガーは複数設定できます。 ただし、いずれかのトリガーが起動した場合に、当該キャンペーンが実行されます。

>[!TIP]
>
>[ アクティビティログ ](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.md){target="_blank"}を使用して、スマートキャンペーン内で発生したステップバイステップを確認します。 アクティビティログは、各リードの詳細ページにある一番右側のタブから確認できます。
