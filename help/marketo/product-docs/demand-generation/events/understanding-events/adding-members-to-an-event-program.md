---
unique-page-id: 37355758
description: Marketoでイベントプログラムにメンバーを追加する方法を説明します。 登録または出席の追跡のために、プログラムにユーザーを追加します。
title: イベントプログラムへのメンバーの追加
exl-id: 05bd4807-3ab8-452d-a389-b22477cf7445
feature: Events
source-git-commit: 031eb5f3ff8aac185ce496664f984a4c745c6e44
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 88%

---

# イベントプログラムへのメンバーの追加 {#adding-members-to-an-event-program}

この記事は、イベントキャップまたはイベントゴールを利用するユーザーにのみ適用されます。

>[!CAUTION]
>
>イベントプログラムにユーザーのリストを直接インポートすると、これらのレコードがゴールトラッキングレポートおよびイベントキャップ進行状況レポートの実際の登録でカウントされなくなります。以下の手順に従って、レコードが確実にカウントされるようにします。

1. リードを作成し、[静的リストに追加](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/create-a-static-list.md)します。

1. [スマートキャンペーンの作成](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md)。

1. 手順 2 で作成したスマートキャンペーンのスマートリストで、**[!UICONTROL リストのメンバー]**&#x200B;フィルターを探して追加します。

   ![](assets/three.png)

1. 手順 1 で作成したリストを見つけて選択します。

   ![](assets/four.png)

1. フローで、**[!UICONTROL プログラムステータスの変更]**&#x200B;フローステップを探して追加します。

   ![](assets/five.png)

1. イベントプログラムを見つけて選択します。

   ![](assets/six.png)

1. 目的のステータスを選択します。

   ![](assets/seven.png)

1. 「[!UICONTROL スケジュール]」タブで、「**[!UICONTROL 1 回実行]**」をクリックします。

   ![](assets/eight.png)

1. 「**[!UICONTROL 今すぐ実行]**」を選択し、「**[!UICONTROL 実行]**」をクリックします。

   ![](assets/nine.png)

1. スマートキャンペーンの実行後に、メンバーがプログラムに追加されます。ゴールトラッキングやイベントキャップ進行状況が正しく計測されるようになります。
