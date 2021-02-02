---
unique-page-id: 4719297
description: カスタムオブジェクト同期の有効化/無効化 — Marketto Docs — 製品ドキュメント
title: カスタムオブジェクト同期の有効化/無効化
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---


# カスタムオブジェクト同期の有効化/無効化{#enable-disable-custom-object-sync}

Salesforceインスタンスで作成されたカスタムオブジェクトは、Marketoの一部にすることもできます。 設定方法を次に示します。

## カスタムオブジェクト同期の有効化/無効化{#enable-disable-custom-object-sync-1}

>[!NOTE]
>
>管理者権限が必要です。

1. 「**管理者**」をクリックします。

   ![](assets/one.png)

1. データベース管理メニューで、**Salesforceオブジェクト同期**&#x200B;をクリックします。

   ![](assets/two-2.png)

1. これが最初のカスタムオブジェクトの場合は、[**スキーマの同期]をクリックします。** それ以外の場合は、「 **スキーマを** 更新」をクリックして最新のスキーマがあることを確認します。

   ![](assets/image2014-12-10-10-3a14-3a44.png)

1. グローバル同期が実行中の場合は、[グローバル同期の無効化]をクリックして無効にする必要があります。****

   ![](assets/image2014-12-10-10-3a14-3a54.png)

   >[!NOTE]
   >
   >Salesforceカスタムオブジェクトスキーマの同期には数分かかる場合があります。

1. 「**スキーマを更新**」をクリックします。

   ![](assets/image2014-12-10-10-3a15-3a7.png)

1. 同期するオブジェクトを選択し、**同期を有効にする**&#x200B;をクリックします。

   >[!TIP]
   >
   >Marketorは、Salesforceのリード、連絡先、またはアカウントオブジェクトと直接関係がある場合にのみ、カスタムオブジェクトを同期できます。

   ![](assets/image2014-12-10-10-3a15-3a30.png)

1. 「**同期を有効にする**」を再度クリックします。

   ![](assets/image2014-12-10-10-3a15-3a40.png)

1. 「**Salesforce**」タブに戻り、「**同期を有効にする**」をクリックします。

   ![](assets/image2014-12-10-10-3a15-3a49.png)

## カスタムオブジェクトの使用{#using-your-custom-objects}

>[!NOTE]
>
>トリガーを持つスマートキャンペーンでは、カスタムオブジェクトを使用できません。

1. スマートリストで、「**Has Opportunity**」フィルターの上にドラッグし、**true**&#x200B;に設定します。

   ![](assets/image2015-8-26-9-3a39-3a28.png)

1. 次に、フィルター制約を使用してフォーカスを絞り込みます。

   ![](assets/image2015-8-24-14-3a18-3a53.png)

   素晴らしい！ これで、このカスタムオブジェクトのデータをスマートキャンペーンとスマートリストで使用できます。

>[!MORELIKETHIS]
>
>[スマートリスト/トリガー制約としての追加カスタムオブジェクトフィールドの削除](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md)
