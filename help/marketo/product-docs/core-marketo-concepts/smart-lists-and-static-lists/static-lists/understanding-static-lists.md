---
unique-page-id: 2949891
description: Marketoの固定リストについて説明します。 メンバーシップを手動で管理する場合は、静的リストを使用します。
title: 静的リストについて
exl-id: c37c1496-cf19-4e44-aaec-77b10669b9bf
feature: Static Lists
TQID: https://experienceleague.adobe.com/rRi3-6ZggKswYYLTZjUr5EBDNoMRirDc1KJgHbbDqP4
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483id: c5f60233-d5ea-4453-a799-0ad258b4d399id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
subfeature_v2: id: ad89fb33-8541-4339-afe7-bb13d1633714
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 222
ht-degree: 57%

---

# 静的リストについて {#understanding-static-lists}

静的リストは、Marketo の最もシンプルで便利な機能の 1 つです。 データベースの名前のリストです。 使う理由はたくさんあります。

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
>最も一般的な間違いの1つは、「人物を削除」することでリストから人物を削除できると考えることです。 **これは間違っています**。 削除したユーザーは、リストだけではなく、**データベース全体**&#x200B;から削除されます。

## リストにユーザーを追加または削除する方法 {#ways-to-add-remove-people-from-a-list}

1. スマートキャンペーンのフローステップ （[ リストに追加](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-to-list.md){target="_blank"}、[ リストから削除](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/remove-from-list.md){target="_blank"}）

1. [単一のアクションフローステップ](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/run-a-single-flow-step-from-a-smart-list.md){target="_blank"}
1. ツリー内のリストにユーザーをドラッグする
1. [リストの読み込み](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md){target="_blank"}

## 静的リストの使用例 {#some-uses-of-a-static-list}

* マーケティングメッセージの受信のために事前に選択されたリスト
* 有害なカウンターインテリジェンスメッセージを送信するために使用する「競合他社」リスト
* 特定の状態にある人物の一時的なリスト。その状態を終了すると、スマートキャンペーンによって削除されます。

>[!MORELIKETHIS]
>
>[静的リストの作成](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/create-a-static-list.md){target="_blank"}
