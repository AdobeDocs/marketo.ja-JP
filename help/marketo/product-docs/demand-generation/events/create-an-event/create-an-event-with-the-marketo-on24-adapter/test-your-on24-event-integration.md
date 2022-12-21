---
unique-page-id: 10096677
description: ON24 イベント統合のテスト - Marketo ドキュメント - 製品ドキュメント
title: ON24 イベント統合のテスト
exl-id: 8326b81e-abf7-4615-9a0b-b0a579be8bb8
source-git-commit: 0c6c119f5be6e2ac3db7d99f7e8623d8aaa3555c
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 100%

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
* Marketo と ON24 の間で出席者のデータ同期が完了すると、Marketo はメンバーシップのステータスを「出席」、「オンデマンドで出席」、「欠席」に更新します。イベントの「**概要**」タブで、イベントのステータスが「**イベント完了**」に更新されます。

>[!MORELIKETHIS]
>
>* [ON24 イベント統合の例](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target=&quot;_blank&quot;}
>* [Marketo ON24 アダプターイベントについて](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target=&quot;_blank&quot;}

