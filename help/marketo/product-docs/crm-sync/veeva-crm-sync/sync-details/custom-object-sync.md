---
description: Veeva CRMからMarketo Engageへのカスタムオブジェクト同期を設定する方法について説明します。 管理画面でカスタムオブジェクトを有効にし、スマートリストとトリガーで使用します。
title: カスタムオブジェクト同期
hide: true
exl-id: 68bc14e7-dfc9-4dce-b159-24d734ee3c6f
feature: Veeva CRM
TQID: https://experienceleague.adobe.com/RmyCIMm3TKbcO3nPcqyZqbWZl1dnJ6Au4HsuURJjcKU
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483
subfeature_v2: id: d0251300-e25f-466f-9856-7e11ce8fa7aa
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 217
ht-degree: 87%

---

# カスタムオブジェクト同期 {#custom-object-sync}

[!DNL Veeva] CRM インスタンスで作成されたカスタムオブジェクトも、Marketo Engage の一部にすることができます。 その設定方法を説明しましょう。

>[!NOTE]
>
>**管理者権限が必要**

>[!PREREQUISITES]
>
>カスタムオブジェクトを使用するには、[!DNL Veeva] CRM で取引先責任者またはアカウントオブジェクトに関連付けられている必要があります。

## カスタムオブジェクトの有効化 {#enable-custom-object}

1. Marketo で、「**[!UICONTROL 管理者]**」をクリックして、「**[!UICONTROL Veeva オブジェクト同期]**」をクリックします。

   ![](assets/custom-object-sync-1.png)

1. これが最初のカスタムオブジェクトの場合は、「**[!UICONTROL スキーマを同期]**」をクリックします。

   ![](assets/custom-object-sync-2.png)

1. 「**[!UICONTROL グローバル同期を無効にする]**」をクリックします。

   ![](assets/custom-object-sync-3.png)

   >[!NOTE]
   >
   >[!DNL Veeva] カスタムオブジェクトスキーマの初期同期には、数分かかる場合があります。

1. 同期するカスタムオブジェクトをキャンバスにドラッグします。

   ![](assets/custom-object-sync-4.png)

   >[!NOTE]
   >
   >カスタムオブジェクトには一意の名前が必要です。 Marketo では、同名の 2 つの異なるカスタムオブジェクトはサポートされていません。

1. 「**[!UICONTROL 同期を有効にする]**」をクリックします。

   ![](assets/custom-object-sync-5.png)

1. 「**[!UICONTROL 同期を有効にする]**」をもう一度クリックします。

   ![](assets/custom-object-sync-6.png)

1. 「**[!UICONTROL Veeva]**」タブに戻ります。

   ![](assets/custom-object-sync-7.png)

1. 「**[!UICONTROL 同期を有効にする]**」をクリックします。

   ![](assets/custom-object-sync-8.png)

1. すべての [!DNL Veeva] カスタムオブジェクトを表示するには、「**[!UICONTROL 管理者]**」をクリックし、「**[!UICONTROL Veeva オブジェクト同期]**」をクリックします。

   ![](assets/custom-object-sync-9.png)

   >[!NOTE]
   >
   >Marketo では、1 レベルから 2 レベルの深さの標準エンティティにリンクされたカスタムエンティティのみがサポートされています。

これで完了です。 カスタムオブジェクトのデータをスマートキャンペーンとスマートリストで使用できるようになりました。

>[!MORELIKETHIS]
>
>* [通話と通話の主要メッセージの同期](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
>* [スマートリスト／トリガー制約としてのカスタムオブジェクトフィールドの追加／削除](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}
