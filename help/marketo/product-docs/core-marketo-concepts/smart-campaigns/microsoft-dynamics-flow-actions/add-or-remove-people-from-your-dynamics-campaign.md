---
description: Dynamics Campaign での人物の追加または削除 — Marketo ドキュメント — 製品ドキュメント
title: Dynamics Campaign での人物の追加または削除
exl-id: 4fea2f7c-0655-4816-8640-76878f760b6e
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '320'
ht-degree: 100%

---

# Dynamics Campaign での人物の追加または削除 {#add-or-remove-people-from-your-dynamics-campaign}

## Dynamics キャンペーンへの追加 {#add-to-dynamics-campaign}

このフローステップは、Marketo スマートキャンペーンで人物を Microsoft キャンペーンのリードまたは連絡先として追加するために使用できます。Dynamics にまだ存在しない場合、リードは自動的に同期され、キャンペーンに追加されます。

>[!NOTE]
>
>このフローアクションは、トリガーキャンペーンでのみ使用できます。

スマートキャンペーンで、ユーザーを追加する Dynamics キャンペーンを見つけて選択します。

![](assets/add-or-remove-people-from-your-dynamics-campaign-1.png)

>[!NOTE]
>
>キャンペーンリストに Dynamics キャンペーンが表示されない場合：
>
>* キャンペーンの同期が機能していることを確認します
>* キャンペーンが Microsoft Dynamics でアクティブではありません


リードと連絡先ごとに、キャンペーン固有の静的マーケティングリストが自動的に作成され、人物が追加されます。これは 1 回限りのアクションで、以降のキャンペーンの同期では、同じマーケティングリストが使用されます。静的なマーケティングリスト名に採用されている命名規格は、リードの場合は `Mkto-leads-<uniqueID>`、連絡先の場合は `Mkto-contacts-<uniqueID>` です。

これらの Marketo で生成されたマーケティングリストを他のキャンペーンに関連付けると、混乱を招く可能性があります。例：1 つ目のキャンペーンに追加すると、2 つ目のキャンペーンにも追加されます。同様に、Marketo で生成されたマーケティングリストの関連付けを Dynamics のキャンペーンから解除することもお勧めしません。

## Dynamics キャンペーンからの削除 {#remove-from-dynamics-campaign}

このフローステップは、Marketo スマートキャンペーンで Microsoft キャンペーンから人物を削除するために使用できます。「Microsoft キャンペーンに追加」フローアクションによってキャンペーンに以前に追加されたリードのみが削除されます。

>[!NOTE]
>
>このフローアクションは、トリガーキャンペーンでのみ使用できます。

スマートキャンペーンで、ユーザーを削除する Dynamics キャンペーンを見つけて選択します。

![](assets/add-or-remove-people-from-your-dynamics-campaign-2.png)

>[!NOTE]
>
>キャンペーンリストに Dynamics キャンペーンが表示されない場合：
>
>* キャンペーンの同期が機能していることを確認します
>* キャンペーンが Microsoft Dynamics でアクティブではありません

