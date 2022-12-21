---
unique-page-id: 2949891
description: 静的リストについて - Marketo ドキュメント - 製品ドキュメント
title: 静的リストについて
exl-id: c37c1496-cf19-4e44-aaec-77b10669b9bf
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 100%

---

# 静的リストについて {#understanding-static-lists}

静的リストは、Marketo の最もシンプルで便利な機能の 1 つです。これらは、データベースから取得した名前のリストにすぎません。使う理由はたくさんあります。

>[!NOTE]
>
>データベース内の 1 人のユーザーが様々な静的リストに存在する場合があります。

静的リストとスマートリストの違いを理解することは非常に重要です。

| タイプ | ロジック |
|---|---|
| スマートリスト | **定義済みルール**&#x200B;に基づく |
| 静的リスト | **各ユーザーの追加と削除**&#x200B;に基づく |

>[!CAUTION]
>
>最も一般的な間違いの 1 つは、単に「ユーザーを削除する」ことで、リストからユーザーを削除できると考えることです。**これは間違っています**。削除したユーザーは、リストだけではなく、**データベース全体**&#x200B;から削除されます。

## リストにユーザーを追加／削除する方法 {#ways-to-add-remove-people-from-a-list}

1. スマートキャンペーンフローステップ（[リストに追加](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-to-list.md)、[リストから削除](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/remove-from-list.md)）

1. [単一アクションフローステップ](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/run-a-single-flow-step-from-a-smart-list.md)
1. ツリー内のリストにユーザーをドラッグする
1. [リストのインポート](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md)

## 静的リストの使用例 {#some-uses-of-a-static-list}

* マーケティングメッセージの受信のために事前に選択されたリスト
* 有害なカウンターインテリジェンスメッセージを送信するために使用する「競合他社」リスト
* 特定の状態にあるユーザーの一時的なリスト（ユーザーはその状態が終了したときにスマートキャンペーンによって削除される）

リストの機能をお楽しみください。

>[!MORELIKETHIS]
>
>[静的リストの作成](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/create-a-static-list.md)
