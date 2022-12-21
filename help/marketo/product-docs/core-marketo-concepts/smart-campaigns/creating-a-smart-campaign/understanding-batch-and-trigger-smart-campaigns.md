---
unique-page-id: 2953132
description: バッチおよびトリガースマートキャンペーンについて - Marketo ドキュメント - 製品ドキュメント
title: バッチおよびトリガースマートキャンペーンについて
exl-id: 84a7b38c-b79c-4360-bd0b-3beb8ca35ac7
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 100%

---

# バッチおよびトリガースマートキャンペーンについて {#understanding-batch-and-trigger-smart-campaigns}

スマートキャンペーンには、バッチおよびトリガーの 2 種類があります。

## バッチスマートキャンペーン {#batch-smart-campaign}

>[!NOTE]
>
>**定義**
>
>バッチスマートキャンペーンは、特定の時刻に起動し、特定のリードのセットに対して一度に処理を行います。例えば、「東京都」にいるすべてのリードにメールを送信する場合に使用します。

バッチスマートキャンペーンでは、スマートリストのセクションで設定するのはフィルターのみです（つまり、トリガーはありません）。

![](assets/batch-filter.png)

「**スケジュール**」タブをクリックすると、当該のスマートキャンペーンが実際に「バッチ」と設定されていることがわかります。

![](assets/batch-c4.png)

**バッチスマートキャンペーン**

* 毎日、毎週、毎月のように、反復するスケジュール設定が可能です。あるいは、単発で 1 回のみ実行するよう設定することも可能です。
* [プログラムスケジュール表示](/help/marketo/product-docs/core-marketo-concepts/programs/program-schedule-view/navigating-the-program-schedule-view.md)に表示されます。スマートキャンペーン内の「待機」ステップ以降の処理は、この表示に表示されません。

<br> 

## トリガースマートキャンペーン {#trigger-smart-campaign}

>[!NOTE]
>
>**定義**
>
>トリガースマートキャンペーンは、トリガー起動イベントに基づいて、一度に 1 つのリードに対して処理を行います。例えば、メール内のリンクがクリックされた場合です。

スマートキャンペーンのスマートリストのセクション内で、少なくとも 1 つのトリガーが使用されている場合、自動的にトリガーモードに設定されます。

![](assets/trigger.png)

「**スケジュール**」タブをクリックすると、当該のスマートキャンペーンが実際に「トリガー起動」と設定されていることがわかります。

![](assets/trigger2.png)

**トリガースマートキャンペーン**

* 反復するスケジュール設定はできません。アクティブまたは非アクティブの設定のみです。
* トリガーは複数設定できます。ただし、いずれかのトリガーが起動した場合に、当該キャンペーンが実行されます。

>[!TIP]
>
>[アクティビティログ](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.md)を使用して、スマートキャンペーン内で発生したことをステップごとに確認します。アクティビティログは、各リードの詳細ページにある一番右側のタブから確認できます。
