---
description: フローステップを使用して、Microsoft Dynamics キャンペーンにユーザーを追加または削除する方法を説明します。 MarketoをDynamics キャンペーンと同期します。
title: '[!DNL Dynamics] Campaign での人物の追加または削除'
exl-id: 4fea2f7c-0655-4816-8640-76878f760b6e
feature: Smart Campaigns, Microsoft Dynamics
TQID: 'https://experienceleague.adobe.com/b6tUqixPGr7ZWTUKVg4L6EKryziHA2IwzpuTepWWEwU'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
    internal-label: Smart Campaigns
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
subfeature_v2:
  - id: ad89fb33-8541-4339-afe7-bb13d1633714
    internal-label: Flow Step
  - id: d5c7388a-594e-4d15-9b39-98d6ce479e8b
    internal-label: Microsoft Dynamics
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
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

リード用と取引先責任者用に、それぞれ人物を追加するためのキャンペーン固有の静的マーケティングリストが自動的に作成されます。 これは 1 回限りのアクションで、以降のキャンペーンの同期では、同じマーケティングリストが使用されます。 静的なマーケティングリスト名に採用されている命名規格は、リードの場合は `Mkto-leads-<uniqueID>`、連絡先の場合は `Mkto-contacts-<uniqueID>` です。

これらの Marketo で生成されたマーケティングリストを他のキャンペーンに関連付けると、混乱を招く可能性があります。 例：1 つ目のキャンペーンに追加すると、2 つ目のキャンペーンにも追加されます。 同様に、Marketo で生成されたマーケティングリストの関連付けを [!DNL Dynamics] のキャンペーンから解除することもお勧めしません。

## Dynamics キャンペーンからの削除 {#remove-from-dynamics-campaign}

このフローステップは、Marketo スマートキャンペーンで Microsoft キャンペーンから人物を削除するために使用できます。 「Microsoft キャンペーンに追加」フローアクションによってキャンペーンに以前に追加されたリードのみが削除されます。

>[!NOTE]
>
>このフローアクションは、トリガーキャンペーンでのみ使用できます。

スマートキャンペーンで、メンバーを削除する対象の Dynamics キャンペーンを見つけて選択します。

![](assets/add-or-remove-people-from-your-dynamics-campaign-2.png)

>[!NOTE]
>
>キャンペーンリストに[!DNL Dynamics] キャンペーンが表示されない場合：
>
>* Campaign Syncが機能することを確認します
>* キャンペーンが [!DNL Microsoft Dynamics] でアクティブではありません
