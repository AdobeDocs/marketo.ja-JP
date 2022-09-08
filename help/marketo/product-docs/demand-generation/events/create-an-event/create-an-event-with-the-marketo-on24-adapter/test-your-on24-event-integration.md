---
unique-page-id: 10096677
description: ON24 イベント統合のテスト — Marketo ドキュメント — 製品ドキュメント
title: ON24 イベント統合のテスト
exl-id: 8326b81e-abf7-4615-9a0b-b0a579be8bb8
source-git-commit: 40cfdddac66b7cd90e33bedf11888a7c5e3b38c9
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 90%

---

# ON24 イベント統合のテスト {#test-your-on-event-integration}

>[!IMPORTANT]
>
>2022 年 8 月以降、ON24 は新しいMarketo統合をサポートしません。 この記事の情報は、既存のユーザーにのみ適用されます。

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
>* [ON24 イベント統合の例](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md)
>* [Marketo ON24 アダプターイベントについて](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md)

