---
description: キャンペーンへのユーザーの追加またはキャンペ  [!DNL Dynamics]  ンからのユーザーの削除 – Marketo ドキュメント – 製品ドキュメント
title: キャンペーンにユーザーを追加またはキャンペ  [!DNL Dynamics]  ンから削除
exl-id: 4fea2f7c-0655-4816-8640-76878f760b6e
feature: Smart Campaigns, Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 54%

---

# [!DNL Dynamics] キャンペーンへのユーザーの追加または削除 {#add-or-remove-people-from-your-dynamics-campaign}

## Dynamics キャンペーンへの追加 {#add-to-dynamics-campaign}

このフローステップは、Marketo Engage スマートキャンペーンで使用して、人物をリードまたは連絡先としてMicrosoft キャンペーンに追加できます。 Dynamics にまだ存在しない場合、リードは自動的に同期され、キャンペーンに追加されます。

>[!NOTE]
>
>このフローアクションは、トリガーキャンペーンでのみ使用できます。

スマートキャンペーンで、ユーザーを追加する Dynamics キャンペーンを検索して選択します。

![](assets/add-or-remove-people-from-your-dynamics-campaign-1.png)

>[!NOTE]
>
>キャンペーンリストに Dynamics キャンペーンが表示されない場合：
>
>* キャンペーンの同期が機能していることを確認します
>* キャンペーンは [!DNL Microsoft Dynamics] でアクティブではありません

リードと連絡先ごとに、キャンペーン固有の静的マーケティングリストが自動的に作成され、人物が追加されます。これは 1 回限りのアクションで、以降のキャンペーンの同期では、同じマーケティングリストが使用されます。静的なマーケティングリスト名に採用されている命名規格は、リードの場合は `Mkto-leads-<uniqueID>`、連絡先の場合は `Mkto-contacts-<uniqueID>` です。

これらの Marketo で生成されたマーケティングリストを他のキャンペーンに関連付けると、混乱を招く可能性があります。例：1 つ目のキャンペーンに追加すると、2 つ目のキャンペーンにも追加されます。同様に、Marketoで生成されたマーケティングリストと [!DNL Dynamics] のキャンペーンを関連付けないこともお勧めします。

## Dynamics キャンペーンからの削除 {#remove-from-dynamics-campaign}

このフローステップは、Marketo スマートキャンペーンで Microsoft キャンペーンから人物を削除するために使用できます。これにより、フローアクション「Microsoft キャンペーンに追加」を通じてキャンペーンに以前に追加されたリードのみがキャンペーンから削除されます。

>[!NOTE]
>
>このフローアクションは、トリガーキャンペーンでのみ使用できます。

スマートキャンペーンで、ユーザーを削除する Dynamics キャンペーンを検索して選択します。

![](assets/add-or-remove-people-from-your-dynamics-campaign-2.png)

>[!NOTE]
>
>キャンペーンリストに [!DNL Dynamics] キャンペーンが表示されない場合：
>
>* キャンペーンの同期が機能していることを確認します
>* キャンペーンは [!DNL Microsoft Dynamics] でアクティブではありません
