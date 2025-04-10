---
unique-page-id: 4719300
description: スマートリスト／トリガー制約としてのカスタムオブジェクトフィールドの追加／の削除 - Marketo ドキュメント - 製品ドキュメント
title: スマートリスト／トリガー制約としてのカスタムオブジェクトフィールドの追加／の削除
exl-id: 639e73eb-9a8c-4b10-8e97-892abf5c5db0
feature: Salesforce Integration
source-git-commit: 6293a11b9d48a20da4cb2448c8374c469679abdb
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 72%

---

# スマートリスト／トリガー制約としてのカスタムオブジェクトフィールドの追加／の削除 {#add-remove-custom-object-field-as-smart-list-trigger-constraints}

Marketo Engageでは、Salesforceのカスタムオブジェクト同期をきめ細かく制御できます。 これにより、カスタムオブジェクトフィルターで制約として使用できるフィールドを選択し、スマートキャンペーンでトリガーとして使用できます。

>[!NOTE]
>
>**管理者権限が必要**

1. **[!UICONTROL 管理者]** エリアに移動しました。

   ![](assets/add-remove-custom-object-field-1.png)

1. 「**[!UICONTROL Salesforce オブジェクト同期]**」をクリックします。

   ![](assets/image2015-12-11-15-3a11-3a41.png)

1. **[!UICONTROL Salesforce オブジェクト同期]**&#x200B;が左の列に表示されます。

   ![](assets/image2015-12-11-15-3a15-3a15.png)

1. 変更するオブジェクトを選択します。

   ![](assets/image2014-12-10-13-3a10-3a11.png)

1. 「**[!UICONTROL 表示可能なフィールドを編集]**」をクリックします。

   >[!TIP]
   >
   >**[!UICONTROL 表示フィールドを編集]** ボタンがグレー表示されている場合は、そのオブジェクトは現在、スマートリストまたはスマートキャンペーンで使用されています。 続行するには、すべての関連付けを削除します。

   ![](assets/image2014-12-10-13-3a10-3a25.png)

1. グローバル同期が有効な場合は、「**[!UICONTROL グローバル同期を無効にする]**」をクリックします。

   ![](assets/image2014-12-10-13-3a10-3a36.png)

1. 必要なフィルター／トリガー制約の横にあるチェックボックスをオンにし、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2014-12-10-13-3a10-3a47.png)

   >[!NOTE]
   >
   >すべてのフィールドは、フィルターの制約としてデフォルトで選択されます。

1. 「**[!UICONTROL フィールド]**」タブをクリックして、変更を確定します。

   ![](assets/image2014-12-10-13-3a10-3a56.png)

   >[!NOTE]
   >
   >忘れずにグローバル同期を再度有効にしてください。

これで、スマートリストとスマートキャンペーンがより強力になります。

>[!MORELIKETHIS]
>
>[カスタムオブジェクト同期の有効化／無効化](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-custom-object-sync.md){target="_blank"}
