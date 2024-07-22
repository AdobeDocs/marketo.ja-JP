---
unique-page-id: 2953132
description: バッチおよびトリガースマートキャンペーンについて - Marketo ドキュメント - 製品ドキュメント
title: バッチおよびトリガースマートキャンペーンについて
exl-id: 84a7b38c-b79c-4360-bd0b-3beb8ca35ac7
feature: Smart Campaigns
source-git-commit: 9e51ece12742152040dbbcb6a1584fba28e863ff
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 52%

---

# バッチおよびトリガースマートキャンペーンについて {#understanding-batch-and-trigger-smart-campaigns}

スマートキャンペーンには、バッチおよびトリガーの 2 種類があります。

## バッチキャンペーン {#batch-campaign}

>[!NOTE]
>
>**定義**
>
>バッチキャンペーンは特定の時間に開始され、特定のユーザーセットに一度に影響します。 例えば、「東京都」にいるすべてのリードにメールを送信する場合に使用します。

バッチキャンペーンには、スマートリストセクション内にフィルターのみが含まれます（トリガーなし）。

![](assets/understanding-batch-and-trigger-smart-campaigns-1.png)

**[!UICONTROL スケジュール]** タブをクリックすると、スマートキャンペーンが「バッチ」に設定されていることを確認できます。

![](assets/understanding-batch-and-trigger-smart-campaigns-2.png)

**バッチスマートキャンペーン**

* 毎日、毎週、毎月のように、反復するスケジュール設定が可能です。あるいは、単発で 1 回のみ実行するよう設定することも可能です。
* [プログラムスケジュール表示](/help/marketo/product-docs/core-marketo-concepts/programs/program-schedule-view/navigating-the-program-schedule-view.md){target="_blank"}に表示されます。Smart Campaign 内の「待機」ステップの後はビューに含まれません。

<br> 

## トリガーキャンペーン {#trigger-campaign}

>[!NOTE]
>
>**定義**
>
>トリガーキャンペーンは、トリガーイベントに基づいて、一度に 1 人のユーザーに影響を与えます。 例えば、メール内のリンクがクリックされた場合です。

スマートキャンペーンで「スマートリスト」セクション内の 1 つ以上のトリガーを使用すると、モードが自動的に「トリガー」に設定されます。

![](assets/understanding-batch-and-trigger-smart-campaigns-3.png)

**[!UICONTROL スケジュール]** タブをクリックすると、スマートキャンペーンが「トリガー済み」に設定されていることを確認できます。

![](assets/understanding-batch-and-trigger-smart-campaigns-4.png)

**トリガーキャンペーン**

* 反復するスケジュール設定はできません。アクティブまたは非アクティブの設定のみです。
* トリガーは複数設定できます。ただし、いずれかのトリガーが起動した場合に、当該キャンペーンが実行されます。

>[!TIP]
>
>[ アクティビティログ ](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.md){target="_blank"} を使用して、スマートキャンペーン内で何が発生したかを段階的に確認できます。 アクティビティログは、各リードの詳細ページにある一番右側のタブから確認できます。
