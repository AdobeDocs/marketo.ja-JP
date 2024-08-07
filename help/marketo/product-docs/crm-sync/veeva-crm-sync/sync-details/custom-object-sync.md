---
description: カスタムオブジェクト同期 - Marketo ドキュメント - 製品ドキュメント
title: カスタムオブジェクト同期
hide: true
hidefromtoc: true
exl-id: 68bc14e7-dfc9-4dce-b159-24d734ee3c6f
feature: Veeva CRM
source-git-commit: bebf61037f37a06b40b4d9c1df872f1cf62a1403
workflow-type: tm+mt
source-wordcount: '201'
ht-degree: 90%

---

# カスタムオブジェクト同期 {#custom-object-sync}

Veeva CRM インスタンスで作成されたカスタムオブジェクトも、Marketo Engage の一部にすることができます。その設定方法を説明します。

>[!NOTE]
>
>**管理者権限が必要**

>[!PREREQUISITES]
>
>カスタムオブジェクトを使用するには、Veeva CRM で取引先責任者またはアカウントオブジェクトに関連付けられている必要があります。

## カスタムオブジェクトの有効化 {#enable-custom-object}

1. Marketo で、「**[!UICONTROL 管理者]**」をクリックして、「**[!UICONTROL Veeva オブジェクト同期]**」をクリックします。

   ![](assets/custom-object-sync-1.png)

1. これが最初のカスタムオブジェクトの場合は、「**[!UICONTROL スキーマを同期]**」をクリックします。

   ![](assets/custom-object-sync-2.png)

1. 「**[!UICONTROL グローバル同期を無効にする]**」をクリックします。

   ![](assets/custom-object-sync-3.png)

   >[!NOTE]
   >
   >Veeva カスタムオブジェクトスキーマの初回同期には、数分かかる場合があります。

1. 同期するカスタムオブジェクトをキャンバスにドラッグします。

   ![](assets/custom-object-sync-4.png)

   >[!NOTE]
   >
   >カスタムオブジェクトには一意の名前が必要です。Marketo では、同名の 2 つの異なるカスタムオブジェクトはサポートされていません。

1. 「**[!UICONTROL 同期を有効にする]**」をクリックします。

   ![](assets/custom-object-sync-5.png)

1. 「**[!UICONTROL 同期を有効にする]**」を再度クリックします。

   ![](assets/custom-object-sync-6.png)

1. 「**[!UICONTROL Veeva]**」タブに戻ります。

   ![](assets/custom-object-sync-7.png)

1. 「**[!UICONTROL 同期を有効にする]**」をクリックします。

   ![](assets/custom-object-sync-8.png)

1. Veeva のカスタムオブジェクトをすべて表示するには、**[!UICONTROL Admin]** と **[!UICONTROL Veeva Objects Sync]** をクリックします。

   ![](assets/custom-object-sync-9.png)

   >[!NOTE]
   >
   >Marketo では、1 レベルから 2 レベルの深さの標準エンティティにリンクされたカスタムエンティティのみがサポートされています。

これで完了です。カスタムオブジェクトのデータをスマートキャンペーンとスマートリストで使用できるようになりました。

>[!MORELIKETHIS]
>
>* [ コールとコールのキーメッセージの同期 ](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
>* [スマートリスト／トリガー制約としてのカスタムオブジェクトフィールドの追加／の削除](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}
