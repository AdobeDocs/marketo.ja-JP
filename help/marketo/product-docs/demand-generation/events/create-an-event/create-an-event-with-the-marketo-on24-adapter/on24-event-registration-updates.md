---
unique-page-id: 10096683
description: ON24 イベント登録のアップデート -  Marketo ドキュメント - 製品ドキュメント
title: ON24 イベント登録のアップデート
exl-id: 1d194ef2-b6ca-4e2d-b476-beb5bccd3c5f
feature: Events
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 72%

---

# ON24 イベント登録のアップデート {#on-event-registration-updates}

## 登録者の手動承認 {#manually-approving-registrants}

確認メールを送信する前に、手動で登録者を承認できます。そのためには、この追加手順を処理するようにキャンペーンを設定する必要があります。

1. 登録トリガーキャンペーン：

   * [!UICONTROL &#x200B; スマートリスト &#x200B;] で、「トリガー」を **[!UICONTROL フォームに入力]** に設定します。
   * フローで、[!UICONTROL &#x200B; ステータスが進行 &#x200B;] を **[!UICONTROL 承認保留中]** に設定します。

1. 「イベント」に移動し、「**[!UICONTROL メンバー]**」タブをクリックします。このタブには、フォームに入力したすべての個人が表示されます。ステータスは「**[!UICONTROL 承認待ち]**」に設定されています。
1. グリッドの上部にあるフィルターを使用して、ステータスが「**[!UICONTROL 承認待ち]**」の個人のみを表示します。
1. 登録する個人を選択します（Shift キーを押しながらクリック、Ctrl キーを押しながらクリック、または「すべてを選択」）。
1. メニューから、「**[!UICONTROL ステータスを変更]**」をクリックします。「**[!UICONTROL 登録済み]**」、「**[!UICONTROL 却下]**」、またはその他の該当するステータスを選択します。

## 登録エラーのある個人の処理 {#handling-people-with-a-registration-error}

ある人物が登録されずに、ステータス [!UICONTROL &#x200B; 登録エラー &#x200B;] に設定された場合は、回復するのに遅すぎるわけではありません。

1. 「[!UICONTROL &#x200B; メンバー &#x200B;]」タブで、ステータスが **[!UICONTROL 登録エラー]** のユーザーのリストをフィルタリングします。
1. 続行する前に、統合に関する問題を特定し、修正したことを確認します（管理の「**[!UICONTROL イベントパートナー]**」でエラーがないことを確認してください）。
1. イシューが解決したら、[!UICONTROL &#x200B; 登録エラー &#x200B;] ステータスのすべての人物を選択し、ステータスを **[!UICONTROL 登録済み]** に変更します。 ON24 への登録が再試行されます。

## ON24 からのメンバーステータスのアップデート {#updating-member-status-from-on}

Marketo は、毎晩午後 11 時頃（米国太平洋時間）に、稼動情報を自動的に取り込みます。稼動情報を手動でアップデートするには、「**[!UICONTROL イベントアクション]**」の下にある「**[!UICONTROL ウェビナープロバイダーから更新]**」をクリックします。

>[!MORELIKETHIS]
>
>[Marketo ON24 アダプターイベントについて](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
