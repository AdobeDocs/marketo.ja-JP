---
unique-page-id: 10096683
description: ON24イベント登録の更新 — Marketto Docs — 製品ドキュメント
title: ON24イベント登録の更新
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 0%

---


# ON24イベント登録の更新{#on-event-registration-updates}

## 手動による登録者の承認{#manually-approving-registrants}

登録者に確認の電子メールを送信する前に、手動で登録者を承認できます。 これを行うには、次の追加手順に従ってキャンペーンを設定する必要があります。

1. 登録トリガーキャンペーンの場合：

   * スマートリストで、トリガーを&#x200B;**Fills Out Form**&#x200B;に設定します。
   * フローで、「進行状況」を「**承認待ち**」に設定します。

1. イベントーに移動し、「**メンバー**」タブをクリックします。 このタブには、フォームに入力したすべての人が表示されます。 これらのステータスは、**承認待ち**&#x200B;に設定する必要があります。
1. グリッドの上部にあるフィルターを使用して、ステータスが&#x200B;**承認待ち**&#x200B;の人のみを表示します。
1. 登録するユーザーを選択します（Shiftキーを押しながらクリック、Ctrlキーを押しながらクリック、または「すべて選択」をクリック）。
1. メニューで[**ステータスの変更**]をクリックします。 「**登録済み**」、「**却下**」、またはその他の該当するステータスを選択します。

## 登録エラーのある人の処理{#handling-people-with-a-registration-error}

登録されずに、「登録エラー」のステータスに設定された場合は、回復に遅すぎません。

1. 「Members」タブで、ステータス&#x200B;**Registration Error**&#x200B;のユーザーのリストをフィルターします。
1. 先に進む前に、統合に関する問題を決定し、修正したことを確認します(管理の&#x200B;**イベントパートナー**&#x200B;にエラーがないことを確認してください)。
1. 問題が解決したら、登録エラーのステータスを持つすべてのユーザーを選択し、ステータスを&#x200B;**登録済み**&#x200B;に変更します。 これにより、ON24に再度登録が試行されます。

## ON24 {#updating-member-status-from-on}からメンバーの状態を更新中

Marketoは、太平洋標準時の約11時に、毎夜自動的に出席情報を取り込みます。 出席情報を手動で更新するには、**イベントアクション**&#x200B;の下の「ウェビナープロバイダーから更新&#x200B;**」をクリックします。**

>[!MORELIKETHIS]
>
>[ON24アダプタイベントについて](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md)
