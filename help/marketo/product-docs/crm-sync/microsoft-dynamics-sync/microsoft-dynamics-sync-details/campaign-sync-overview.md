---
description: Microsoft DynamicsとMarketo間のキャンペーン同期について説明します。 「Microsoft Campaign に追加」および「Microsoft Campaign から削除」フローのアクションとトリガーを使用します。
title: キャンペーン同期の概要
exl-id: d9b748e9-3e0c-40bc-937a-99160aead081
feature: Microsoft Dynamics
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '159'
ht-degree: 85%

---

# キャンペーン同期の概要 {#campaign-sync-overview}

キャンペーン同期の一環として、[!DNL Dynamics] キャンペーンのメンバーシップを操作する自動処理を設定できます。特定の行動やデモグラフィックの条件を満たすリードを Microsoft キャンペーンの一部にできます。

>[!PREREQUISITES]
>
>Marketo 用 [!DNL Dynamics] プラグインを最新バージョンにアップデートします。

次のフローアクションを使用できます。

* [!UICONTROL Microsoft キャンペーンに追加]
* [!UICONTROL Microsoft キャンペーンから削除]

>[!NOTE]
>
>**[!UICONTROL Microsoft キャンペーンから削除]**&#x200B;では、Marketo のフローアクションを使用して追加された人のみが削除されます。

また、次の 2 つのトリガーがあります。

* [!UICONTROL Microsoft キャンペーンに追加済み]
* [!UICONTROL Microsoft キャンペーンから削除済み]

トリガーは、Marketo のフローアクション「[!UICONTROL Microsoft キャンペーンに追加]」および「[!UICONTROL Microsoft キャンペーンから削除済み]」からのアクションに基づいて実行されます。

>[!NOTE]
>
>キャンペーンの同期が機能し、キャンペーンが Microsoft [!DNL Dynamics] で非アクティブでないことを確認します。

>[!MORELIKETHIS]
>
>* [キャンペーン同期の有効化](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/enable-campaign-sync.md)
>* [&#x200B; [!DNL Dynamics]  キャンペーンでの人物の追加または削除](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/add-or-remove-people-from-your-dynamics-campaign.md)
