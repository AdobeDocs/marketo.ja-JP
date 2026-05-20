---
description: Veeva CRMとMarketo Engage間でカスタムオブジェクトの同期を有効または無効にする方法について説明します。 AdminとVeeva Objects Syncを使用して、カスタムオブジェクトを選択および同期します。
title: カスタムオブジェクト同期の有効化／無効化
exl-id: 01417fb6-70f5-449b-ad56-42e1c0b2ff68
feature: Veeva CRM
TQID: https://experienceleague.adobe.com/nsmRk-zf-I5r0hfLxsOnGsTf66X-bYZ7OAUXHrPc-t0
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483
subfeature_v2: id: d0251300-e25f-466f-9856-7e11ce8fa7aa
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 230
ht-degree: 88%

---

# カスタムオブジェクト同期の有効化／無効化 {#enable-disable-custom-object-sync}

[!DNL Veeva] CRM インスタンスで作成されたカスタムオブジェクトも、Marketo Engage の一部にすることができます。 その設定方法を説明しましょう。

## カスタムオブジェクト同期の有効化／無効化 {#enable-or-disable-the-custom-object-sync}

>[!NOTE]
>
>**管理者権限が必要**

1. Marketo で、「**[!UICONTROL 管理者]**」をクリックして、「**[!UICONTROL Veeva オブジェクト同期]**」をクリックします。

   ![](assets/enable-disable-custom-object-sync-1.png)

1. これが最初のカスタムオブジェクトの場合は、「**[!UICONTROL スキーマを同期]**」をクリックします。 それ以外の場合は、「**[!UICONTROL スキーマを更新]**」をクリックして最新の情報を取得します。

   ![](assets/enable-disable-custom-object-sync-2.png)

1. グローバル同期が実行中の場合は、「**[!UICONTROL グローバル同期を無効にする]**」をクリックして無効化します。

   ![](assets/enable-disable-custom-object-sync-3.png)

   >[!NOTE]
   >
   >[!DNL Veeva] カスタムオブジェクトスキーマの同期には、数分かかる場合があります。

1. 「**[!UICONTROL スキーマを更新]**」をクリックします。

   ![](assets/enable-disable-custom-object-sync-4.png)

同期するオブジェクトを選択し、「**[!UICONTROL 同期を有効にする]**」をクリックします。

![](assets/enable-disable-custom-object-sync-5.png)

>[!TIP]
>
>Marketo では、[!DNL Veeva] CRM の取引先責任者またはアカウントオブジェクトのいずれかと直接の関係がある場合にのみ、カスタムオブジェクトを同期できます。

1. 「**[!UICONTROL 同期を有効にする]**」をもう一度クリックします。

   ![](assets/enable-disable-custom-object-sync-6.png)

1. 「[!UICONTROL Veeva]」タブに戻って、「**[!UICONTROL 同期を有効にする]**」をクリックします。

   ![](assets/enable-disable-custom-object-sync-7.png)

## カスタムオブジェクトの使用 {#using-your-custom-objects}

>[!NOTE]
>
>スマートキャンペーンでは、カスタムオブジェクトをトリガーと共に使用することはできません。

1. [!UICONTROL スマートリスト]で、「**[!UICONTROL 商談あり]**」フィルターをドラッグして、**[!UICONTROL True]** に設定します。

   ![](assets/enable-disable-custom-object-sync-8.png)

1. オプションで、フィルター制約を使用してフォーカスを絞り込みます。

   ![](assets/enable-disable-custom-object-sync-9.png)

このカスタムオブジェクトのデータを[!UICONTROL スマートキャンペーン]と[!UICONTROL スマートリスト]で使用できるようになりました。

>[!MORELIKETHIS]
>
>[スマートリスト／トリガー制約としてのカスタムオブジェクトフィールドの追加／削除](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}
