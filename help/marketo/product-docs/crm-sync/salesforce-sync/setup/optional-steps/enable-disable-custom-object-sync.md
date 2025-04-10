---
unique-page-id: 4719297
description: カスタムオブジェクト同期の有効化／無効化 - Marketo ドキュメント - 製品ドキュメント
title: カスタムオブジェクト同期の有効化／無効化
exl-id: f17d9135-b33e-48c0-9220-131fb437e9e5
feature: Salesforce Integration
source-git-commit: 6293a11b9d48a20da4cb2448c8374c469679abdb
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 61%

---

# カスタムオブジェクト同期の有効化／無効化 {#enable-disable-custom-object-sync}

Salesforce インスタンスで作成されたカスタムオブジェクトも、Marketo Engage の一部にすることができます。その設定方法を説明しましょう。

## カスタムオブジェクト同期の有効化／無効化 {#enable-disable-custom-object-sync-1}

>[!NOTE]
>
>**管理者権限が必要**

1. 「**[!UICONTROL 管理者]**」領域に移動します。

   ![](assets/enable-disable-custom-object-sync-1.png)

1. データベース管理メニューで、「**[!UICONTROL Salesforce オブジェクト同期]**」をクリックします。

   ![](assets/enable-disable-custom-object-sync-2.png)

1. これが最初のカスタムオブジェクトの場合は、「**[!UICONTROL スキーマを同期]**」をクリックします。 それ以外の場合は、**[!UICONTROL スキーマを更新]** をクリックして、が最新であることを確認します。

   ![](assets/enable-disable-custom-object-sync-3.png)

1. グローバル同期が実行中の場合は、「**[!UICONTROL グローバル同期を無効にする]**」をクリックして無効にする必要があります。

   ![](assets/image2014-12-10-10-3a14-3a54.png)

   >[!NOTE]
   >
   >Salesforce カスタムオブジェクトスキーマの同期には、数分かかる場合があります。

1. 「**[!UICONTROL スキーマを更新]**」をクリックします。

   ![](assets/image2014-12-10-10-3a15-3a7.png)

1. 同期するオブジェクトを選択し、「**[!UICONTROL 同期を有効にする]**」をクリックします。

   >[!TIP]
   >
   >Marketo では、Salesforce のリード、連絡先、アカウントオブジェクトのいずれかと直接の関係がある場合にのみ、カスタムオブジェクトを同期できます。

   ![](assets/image2014-12-10-10-3a15-3a30.png)

1. 「**[!UICONTROL 同期を有効にする]**」を再度クリックします。

   ![](assets/image2014-12-10-10-3a15-3a40.png)

1. 「**[!DNL Salesforce]**」タブに戻り、「**[!UICONTROL 同期を有効にする]** をクリックします。

   ![](assets/image2014-12-10-10-3a15-3a49.png)

## カスタムオブジェクトの使用 {#using-your-custom-objects}

>[!NOTE]
>
>トリガーを含むスマートキャンペーンでは、カスタムオブジェクトを使用できません。

1. スマートリストで「**[!UICONTROL 商談あり]**」フィルターにドラッグして、「**[!UICONTROL true]**」に設定します。

   ![](assets/image2015-8-26-9-3a39-3a28.png)

1. 次に、フィルター制約を使用してフォーカスを絞り込みます。

   ![](assets/image2015-8-24-14-3a18-3a53.png)

   これで完了です。これで、このカスタムオブジェクトのデータをスマートキャンペーンとスマートリストで使用できます。

>[!MORELIKETHIS]
>
>[スマートリスト／トリガー制約としてのカスタムオブジェクトフィールドの追加／削除](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}
