---
unique-page-id: 10097584
description: Microsoft Dynamicsの同期ステータスと、スループットとバックログを監視する方法について説明します。 管理者で「同期ステータス」タブと「同期エラー」タブを表示します。
title: 同期ステータス
exl-id: cab1cb1d-2bc7-4466-bab8-c9e03ab269f7
feature: Microsoft Dynamics
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '182'
ht-degree: 86%

---

# 同期ステータス {#sync-status}

「[!UICONTROL 同期ステータス]」タブと「[!UICONTROL 同期エラー]」タブで、同期プロセスの現在のスループットとバックログをタブに保つことができます。

## 「[!UICONTROL 同期ステータス]」タブ {#sync-status-tab}

1. 「**[!UICONTROL 管理者]**」をクリックし、「**[!UICONTROL Microsoft Dynamics]**」をクリックします。

   ![](assets/image2016-1-20-11-3a34-3a14.png)

1. 「**[!UICONTROL 同期ステータス]**」タブをクリックします。

   ![](assets/image2016-5-19-10-3a1-3a11.png)

   このテーブルには、各オブジェクトに対して、まだ同期されていない挿入と更新のバックログが表示されています。

1. 任意の行をダブルクリックして、商談情報を表示します。

   ![](assets/image2016-5-19-10-3a3-3a21.png)

   同期ステータスの詳細は、挿入と更新、および最も古い挿入と更新のレコード別に分類されます。

   ![](assets/image2016-1-22-10-3a51-3a10.png)

1. **[!UICONTROL 表示]**&#x200B;ドロップダウンをクリックして「**[!UICONTROL 過去 1 時間]**」を選択してスループット情報を表示します。

   ![](assets/image2016-5-19-10-3a20-3a7.png)

   過去 1 時間（午後 1～2 時など）に同期されたレコードの数が表示されます。

   ![](assets/image2016-5-19-10-3a22-3a15.png)

   >[!NOTE]
   >
   >「[!UICONTROL 過去 1 時間]」ビューを表示している場合、「[!UICONTROL 挿入]」列と「[!UICONTROL 更新]」列には「N/A」と表示されます。これは期待されている動作です。

## 「[!UICONTROL 同期エラー]」タブ {#sync-errors-tab}

操作、方向、エラーコード、エラーメッセージなどの詳細との同期に失敗したリード（およびその他のオブジェクト）の参照、検索、エクスポートを行います。

![](assets/image2016-5-19-10-3a26-3a35.png)

>[!MORELIKETHIS]
>
>[通知のタイプ](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications/notification-types.md){target="_blank"}
