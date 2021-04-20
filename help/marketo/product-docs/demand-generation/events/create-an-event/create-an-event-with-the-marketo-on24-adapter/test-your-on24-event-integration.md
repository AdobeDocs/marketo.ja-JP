---
unique-page-id: 10096677
description: ON24イベント統合のテスト —Marketoドキュメント — 製品ドキュメント
title: ON24イベント統合のテスト
exl-id: 8326b81e-abf7-4615-9a0b-b0a579be8bb8
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 0%

---

# ON24イベント統合のテスト{#test-your-on-event-integration}

必ず、イベント統合を十分にテストしてください。

## 最初のキャンペーン{#recommended-test-sequence-before-running-your-first-campaign}を実行する前に推奨されるテストシーケンス

1. イベントの登録フォームに入力し、有効な電子メールアドレスを使用してテストします。
1. Marketoイベントのメンバーシップグリッドに、テスト名が&#x200B;**登録済み**&#x200B;ステータスで表示されていることを確認します。
1. テスト名がON24に「**登録済み**」と表示されていることを確認します。
1. テスト名の登録に使用した有効な電子メールアドレスに確認の電子メールがイベントに届いていること、および一意のURLが電子メール内で解決されていることを確認します。

   >[!NOTE]
   >
   >一意のURLを各登録者の電子メールに表示するには、確認用の電子メールに`{{member.webinar url}}`トークンを使用する必要があります。

## イベント{#after-the-event}の後

イベントの発生後にデータを更新する方法は次のとおりです。

* Marketoは毎夜ON24から出席者のデータを取得します。
* 出席者のデータがMarketoとON24の間で同期されると、Marketoはメンバーシップのステータスを「出席済み」、「出席済み」、「出席済み」、「非表示」に更新します。 イベントの「**概要**」タブで、イベントの状態が「**イベント完了**」に更新されます。

>[!MORELIKETHIS]
>
>* [ON24イベント統合の例](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md)
>* [MarketoON24アダプタイベントについて](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md)

