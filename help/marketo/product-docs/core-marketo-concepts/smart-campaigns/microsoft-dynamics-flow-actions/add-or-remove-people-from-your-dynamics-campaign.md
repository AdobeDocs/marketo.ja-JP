---
description: フローステップを使用して、Microsoft Dynamics キャンペーンにユーザーを追加または削除する方法を説明します。 MarketoをDynamics キャンペーンと同期します。
title: ' [!DNL Dynamics]  Campaign での人物の追加または削除'
exl-id: 4fea2f7c-0655-4816-8640-76878f760b6e
feature: Smart Campaigns, Microsoft Dynamics
source-git-commit: 60c5603fa29bb1039b9d477633beb2c6f5c63486
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 83%

---

# [!DNL Dynamics] Campaign での人物の追加または削除 {#add-or-remove-people-from-your-dynamics-campaign}

## Dynamics キャンペーンへの追加 {#add-to-dynamics-campaign}

このフローステップは、Marketo Engage スマートキャンペーンで人物を Microsoft キャンペーンのリードまたは取引先責任者として追加するのに使用できます。 Dynamics にまだ存在しない場合、リードは自動的に同期され、キャンペーンに追加されます。

>[!NOTE]
>
>このフローアクションは、トリガーキャンペーンでのみ使用できます。

スマートキャンペーンで、人物を追加する Dynamics キャンペーンを見つけて選択します。

![](assets/add-or-remove-people-from-your-dynamics-campaign-1.png)

>[!NOTE]
>
>キャンペーンリストにDynamics キャンペーンが表示されない場合：
>
>* Campaign Syncが機能することを確認します
>* キャンペーンが [!DNL Microsoft Dynamics] でアクティブではありません

リードと連絡先ごとに、キャンペーン固有の静的マーケティングリストが自動的に作成され、人物が追加されます。 これは 1 回限りのアクションで、以降のキャンペーンの同期では、同じマーケティングリストが使用されます。 静的なマーケティングリスト名に採用されている命名規格は、リードの場合は `Mkto-leads-<uniqueID>`、連絡先の場合は `Mkto-contacts-<uniqueID>` です。

これらの Marketo で生成されたマーケティングリストを他のキャンペーンに関連付けると、混乱を招く可能性があります。 例：1 つ目のキャンペーンに追加すると、2 つ目のキャンペーンにも追加されます。 同様に、Marketo で生成されたマーケティングリストの関連付けを [!DNL Dynamics] のキャンペーンから解除することもお勧めしません。

## Dynamics キャンペーンからの削除 {#remove-from-dynamics-campaign}

このフローステップは、Marketo スマートキャンペーンで Microsoft キャンペーンから人物を削除するために使用できます。 「Microsoft キャンペーンに追加」フローアクションによってキャンペーンに以前に追加されたリードのみが削除されます。

>[!NOTE]
>
>このフローアクションは、トリガーキャンペーンでのみ使用できます。

スマートキャンペーンで、人物を削除する Dynamics キャンペーンを見つけて選択します。

![](assets/add-or-remove-people-from-your-dynamics-campaign-2.png)

>[!NOTE]
>
>キャンペーンリストに[!DNL Dynamics] キャンペーンが表示されない場合：
>
>* Campaign Syncが機能することを確認します
>* キャンペーンが [!DNL Microsoft Dynamics] でアクティブではありません
