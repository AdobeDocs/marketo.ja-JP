---
unique-page-id: 37355758
description: イベントプログラムへのメンバーの追加 — Marketto Docs — 製品ドキュメント
title: イベントプログラムへのメンバーの追加
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 0%

---


# イベントプログラムへのメンバの追加{#adding-members-to-an-event-program}

この記事は、イベントの上限またはイベントの目標を利用しているユーザーにのみ適用されます。

>[!CAUTION]
>
>人のリストをイベントプログラムに直接インポートすると、目標追跡レポートおよびイベント上限の進行状況レポートで、これらのレコードが実際の登録数にカウントされなくなります。 次の手順に従って、レコードが確実にカウントされるようにします。

1. ユーザーを作成して[静的なリスト](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/create-a-static-list.md)に追加します。

1. [スマートキャンペーンの作成](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md)。

1. 手順2で作成したスマートキャンペーンのスマートリストで、**リストのメンバー**&#x200B;フィルターを探して追加します。

   ![](assets/three.png)

1. 手順1で作成したリストを探して選択します。

   ![](assets/four.png)

1. フローで、**プログラムステータスの変更**&#x200B;フローステップを探して追加します。

   ![](assets/five.png)

1. イベントプログラムを探して選択します。

   ![](assets/six.png)

1. ステータスを選択します。

   ![](assets/seven.png)

1. 「スケジュール」タブで、「**1回実行**」をクリックします。

   ![](assets/eight.png)

1. 「**今すぐ実行**」を選択し、「**実行**」をクリックします。

   ![](assets/nine.png)

1. スマート・キャンペーンの実行後、メンバーはプログラムに追加され、目標追跡とイベント上限の進行状況の計算でカウントされます。
