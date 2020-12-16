---
unique-page-id: 2953132
description: バッチとトリガースマートキャンペーンについて — Marketto Docs — 製品ドキュメント
title: バッチとトリガースマート・キャンペーンの理解
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---


# バッチとトリガースマート・キャンペーンの理解 {#understanding-batch-and-trigger-smart-campaigns}

スマートキャンペーンには2種類あります。バッチとトリガーを参照してください。

## バッチスマートキャンペーン {#batch-smart-campaign}

>[!NOTE]
>
>**定義**
>
>バッチキャンペーンは、特定の時刻に起動し、特定の一連のユーザーにすべて同時に影響します。 例えば、カリフォルニアの全人に電子メールを送信する場合です。

バッチスマートキャンペーンは、スマートリストセクション内のフィルターのみを持ちます（つまり、トリガーは持ちません）。

![](assets/batch-filter.png)

「 **スケジュール** 」タブをクリックすると、スマートキャンペーンが「バッチ」に設定されていることが確認されます。

![](assets/batch-c4.png)

**バッチスマートキャンペーン**

* 毎日、毎週、毎月など、繰り返しのスケジュールを設定できます。 1回だけ実行させることもできます。
* は、 [プログラムスケジュール表示に表示されます](../../../../product-docs/core-marketo-concepts/programs/program-schedule-view/navigating-the-program-schedule-view.md)。\
   *スマートキャンペーン内の「待機」ステップの後は、表示に含まれないことに注意してください。

<br> 

## スマートキャンペーンのトリガー {#trigger-smart-campaign}

>[!NOTE]
>
>**定義**
>
>トリガースマートキャンペーンは、トリガーされたイベントに基づいて、一度に1人の人に影響を与える。 トリガーの例としては、電子メール内のリンクをクリックします。

スマート・キャンペーンがスマート・リスト・セクション内で少なくとも1つのトリガを使用する場合、モードは自動的にトリガに設定されます。

![](assets/trigger.png)

「 **スケジュール** 」タブをクリックすると、スマートキャンペーンが「トリガー済み」に設定されていることが確認されます。

![](assets/trigger2.png)

**スマートキャンペーンのトリガー**

* 繰り返しのスケジュールは設定できません。 アクティブまたは非アクティブに設定することのみ可能です。
* 複数のトリガーを設定できます。 ただし、トリガーが発生した場合は、キャンペーンのアクションが実行されます。

## トリガーされる電子メールキャンペーンの作成に関するビデオを視聴する {#watch-a-video-on-creating-triggered-email-campaigns}

`<iframe width="630" height="470" src="//play.vidyard.com/6zNazwTgt2LNeCjPAt3W9K.html?v=3.1.1" frameborder="0" allowfullscreen></iframe>`

>[!TIP]
>
>[アクティビティログを使用して](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.md) 、スマートキャンペーン内で何が順を追って発生したかを確認します。 アクティビティログは、ユーザーの詳細ページの最後のタブに表示されます。

