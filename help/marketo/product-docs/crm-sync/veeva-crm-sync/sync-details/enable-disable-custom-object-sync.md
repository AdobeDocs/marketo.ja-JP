---
description: カスタムオブジェクト同期の有効化／無効化 - Marketo ドキュメント - 製品ドキュメント
title: カスタムオブジェクト同期の有効化／無効化
exl-id: 01417fb6-70f5-449b-ad56-42e1c0b2ff68
source-git-commit: 2ce44b7c44517a6fdb3f616a3d69b25158ea4ec9
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 100%

---

# カスタムオブジェクト同期の有効化／無効化 {#enable-disable-custom-object-sync}

Veeva CRM インスタンスで作成されたカスタムオブジェクトも、Marketo Engage の一部にすることができます。その設定方法を説明しましょう。

## カスタムオブジェクト同期の有効化／無効化 {#enable-or-disable-the-custom-object-sync}

>[!NOTE]
>
>**管理者権限が必要**

1. Marketo で、「**管理者**」をクリックして、「**Veeva オブジェクト同期**」をクリックします。

   ![](assets/enable-disable-custom-object-sync-1.png)

1. これが最初のカスタムオブジェクトの場合は、「スキーマを同期」をクリックします。それ以外の場合は、「**スキーマを更新**」をクリックして最新の情報を取得します。

   ![](assets/enable-disable-custom-object-sync-2.png)

1. グローバル同期が実行中の場合は、「**グローバル同期を無効にする**」をクリックして無効化します。

   ![](assets/enable-disable-custom-object-sync-3.png)

   >[!NOTE]
   >
   >Veeva カスタムオブジェクトスキーマの同期には、数分かかる場合があります。

1. 「**スキーマを更新**」をクリックします。

   ![](assets/enable-disable-custom-object-sync-4.png)

同期するオブジェクトを選択し、「同期を有効にする」をクリックします。

![](assets/enable-disable-custom-object-sync-5.png)

>[!TIP]
>
>Marketo では、Veeva CRM の取引先責任者またはアカウントオブジェクトのいずれかと直接の関係がある場合にのみ、カスタムオブジェクトを同期できます。

1. 「**同期を有効にする**」を再度クリックします。

   ![](assets/enable-disable-custom-object-sync-6.png)

1. 「Veeva」タブに戻って、「**同期を有効にする**」をクリックします。

   ![](assets/enable-disable-custom-object-sync-7.png)

## カスタムオブジェクトの使用 {#using-your-custom-objects}

>[!NOTE]
>
>スマートキャンペーンでは、カスタムオブジェクトをトリガーと共に使用することはできません。

1. スマートリストで、「商談あり」フィルターをドラッグして、**true** に設定します。

   ![](assets/enable-disable-custom-object-sync-8.png)

1. オプションで、フィルター制約を使用してフォーカスを絞り込みます。

   ![](assets/enable-disable-custom-object-sync-9.png)

これで完了です。このカスタムオブジェクトのデータをスマートキャンペーンとスマートリストで使用できるようになりました。

>[!MORELIKETHIS]
>
>[スマートリスト／トリガー制約としてのカスタムオブジェクトフィールドの追加／の削除](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target=&quot;_blank&quot;}
