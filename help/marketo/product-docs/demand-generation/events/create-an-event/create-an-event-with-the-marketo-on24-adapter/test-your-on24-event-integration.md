---
unique-page-id: 10096677
description: ON24 イベント統合のテスト - Marketo ドキュメント - 製品ドキュメント
title: ON24 イベント統合のテスト
exl-id: 8326b81e-abf7-4615-9a0b-b0a579be8bb8
feature: Events
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 89%

---

# ON24 イベント統合のテスト {#test-your-on-event-integration}

イベント統合は必ず十分にテストしてください。

## 最初のキャンペーンを実行する前に推奨されるテストシーケンス {#recommended-test-sequence-before-running-your-first-campaign}

1. イベントの登録フォームに入力し、有効なメールアドレスを使用してテストします。
1. Marketo イベントのメンバーシップグリッドに、テスト名が「**登録済み**」ステータスで表示されることを確認します。
1. また、ON24 でテスト名が「**登録済み**」と表示されることを確認します。
1. テスト名の登録に使用した有効なメールアドレスで、イベント確認メールが受信されており、メールで一意の URL が解決されたことを確認します。

   >[!NOTE]
   >
   >各登録者のメールに一意の URL を表示するには、確認メールで `{{member.webinar url}}` トークンを使用する必要があります。

## イベント後 {#after-the-event}

イベント発生後にデータが更新される方法を次に示します。

* Marketo では、毎晩 ON24 から出席者データを取得します。
* Marketoと ON24 の間で出席者データが同期されると、Marketoはメンバーシップステータスを [!UICONTROL &#x200B; 出席済み &#x200B;]、[!UICONTROL &#x200B; 出席済みオンデマンド &#x200B;]、または [!UICONTROL &#x200B; 表示なし &#x200B;] に更新します。 イベントの「**[!UICONTROL 概要]**」タブで、イベントのステータスが「**[!UICONTROL イベント完了]**」に更新されます。

>[!MORELIKETHIS]
>
>* [ON24 イベント統合の例](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target="_blank"}
>* [Marketo ON24 アダプターイベントについて](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
