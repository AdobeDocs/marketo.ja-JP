---
unique-page-id: 10096677
description: ON24イベント統合のテスト — Marketto Docs — 製品ドキュメント
title: ON24イベント統合のテスト
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---


# ON24イベント統合のテスト {#test-your-on-event-integration}

必ず、イベント統合を十分にテストしてください。

## 最初のキャンペーンを実行する前に推奨されるテストシーケンス {#recommended-test-sequence-before-running-your-first-campaign}

1. イベントの登録フォームに入力し、有効な電子メールアドレスを使用してテストします。
1. MarketorイベントのMembershipグリッドに、 **登録済み** ステータスのテスト名が表示されることを確認します。
1. テスト名がON24に **登録済みと表示されることを確認します** 。
1. テスト名の登録に使用した有効な電子メールアドレスに確認の電子メールがイベントに届いていること、および一意のURLが電子メール内で解決されていることを確認します。

   >[!NOTE]
   >
   >一意のURLを各登録者の電子メールに表示するには、確認用の電子メールで `{{member.webinar url}}` トークンを使用する必要があります。

## イベント後 {#after-the-event}

イベントの発生後にデータを更新する方法は次のとおりです。

* 毎夜、ON24から出席者データを取得します。
* 参加者のデータがMarketoとON24の間で同期されると、Marketorはメンバーシップのステータスを「出席済み」、「出席済みオンデマンド」または「ショーなし」に更新します。 イベントの「 **概要** 」タブで、イベントのステータスが「 **イベント完了**」に更新されます。

>[!NOTE]
>
>**関連記事**
>
>* [ON24イベント統合の例](example-on24-event-integration.md)
>* [ON24アダプタイベントについて](understanding-marketo-on24-adapter-events.md)

>



