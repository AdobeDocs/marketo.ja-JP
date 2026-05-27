---
unique-page-id: 10096683
description: ON24 イベント登録の更新と、Marketoとの同期方法について説明します。 登録の変更時に、個人とプログラムのステータスを同期します。
title: ON24 イベント登録のアップデート
exl-id: 1d194ef2-b6ca-4e2d-b476-beb5bccd3c5f
feature: Events
TQID: https://experienceleague.adobe.com/2G9BHBIeyQS6ID6nT8rjDbRfx1re3z4tUslY4QEki7Y
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 299
ht-degree: 84%

---

# ON24 イベント登録のアップデート {#on-event-registration-updates}

## 登録者の手動承認 {#manually-approving-registrants}

確認メールを送信する前に、手動で登録者を承認できます。 そのためには、この追加手順を処理するようにキャンペーンを設定する必要があります。

1. 登録トリガーキャンペーン：

   * 「[!UICONTROL スマートリスト]」で、トリガーを「**[!UICONTROL フォームを記入]**」に設定します。
   * 「フロー」で、「[!UICONTROL 進行中のステータス]」を「**[!UICONTROL 承認待ち]**」に設定します。

1. 「イベント」に移動し、「**[!UICONTROL メンバー]**」タブをクリックします。 このタブには、フォームに入力したすべての個人が表示されます。 ステータスは「**[!UICONTROL 承認待ち]**」に設定されています。
1. グリッドの上部にあるフィルターを使用して、ステータスが「**[!UICONTROL 承認待ち]**」の個人のみを表示します。
1. 登録する個人を選択します（Shift キーを押しながらクリック、Ctrl キーを押しながらクリック、または「すべてを選択」）。
1. メニューから、「**[!UICONTROL ステータスを変更]**」をクリックします。 「**[!UICONTROL 登録済み]**」、「**[!UICONTROL 却下]**」、またはその他の該当するステータスを選択します。

## 登録エラーのある個人の処理 {#handling-people-with-a-registration-error}

ユーザーが登録されておらず、ステータス [!UICONTROL 登録エラー]に設定された場合、回復するのは遅くはありません。

1. 「[!UICONTROL メンバー]」タブで、ステータスが「**[!UICONTROL 登録エラー]**」の個人のリストをフィルターします。
1. 続行する前に、統合に関する問題を特定し、修正したことを確認します（管理の「**[!UICONTROL イベントパートナー]**」でエラーがないことを確認してください）。
1. 問題が解決したら、「[!UICONTROL 登録エラー]」ステータスのすべての個人を選択し、ステータスを「**[!UICONTROL 登録済み]**」に変更します。 ON24 への登録が再試行されます。

## ON24 からのメンバーステータスのアップデート {#updating-member-status-from-on}

Marketo は、毎晩午後 11 時頃（米国太平洋時間）に、稼動情報を自動的に取り込みます。 稼動情報を手動でアップデートするには、「**[!UICONTROL イベントアクション]**」の下にある「**[!UICONTROL ウェビナープロバイダーから更新]**」をクリックします。

>[!MORELIKETHIS]
>
>[Marketo ON24 アダプターイベントについて](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
