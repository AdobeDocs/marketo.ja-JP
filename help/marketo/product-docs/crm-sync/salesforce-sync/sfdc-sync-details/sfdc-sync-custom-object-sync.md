---
unique-page-id: 2953471
description: SFDC同期 — カスタムオブジェクト同期 — Marketto Docs — 製品ドキュメント
title: SFDC同期 — カスタムオブジェクト同期
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---


# SFDC同期：カスタムオブジェクト同期{#sfdc-sync-custom-object-sync}

Salesforceインスタンスで作成されたカスタムオブジェクトは、Marketoの一部にすることもできます。  設定方法を次に示します。

>[!NOTE]
>
>**必要な管理者権限**

>[!PREREQUISITES]
>
>カスタムオブジェクトを使用するには、Salesforceの[リード](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-field-sync.md)、[連絡先](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md)、または[アカウント](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md)オブジェクトに関連付ける必要があります。

## カスタムオブジェクトを有効にする{#enable-custom-object}

1. 「**管理者**」をクリックし、「**Salesforceオブジェクト同期**」リンクをクリックします。

   ![](assets/image2015-11-19-10-3a28-3a5.png).

1. これが最初のカスタムオブジェクトの場合は、[**スキーマを同期**]をクリックします。

   ![](assets/rtaimage-2.png)

1. 「**グローバル同期を無効にする**」をクリックします。

   ![](assets/image2015-4-22-10-3a45-3a0.png)

   >[!NOTE]
   >
   >Salesforceカスタムオブジェクトスキーマの初期同期には、数分かかる場合があります。

   ![](assets/image2015-4-22-10-3a45-3a18.png)

1. 同期するカスタムオブジェクトをキャンバスにドラッグします。

   ![](assets/image2015-4-22-10-3a45-3a30.png)

   >[!NOTE]
   >
   >カスタムオブジェクトには、一意の名前を付ける必要があります。 Marketorは、同じ名前を持つ2つの異なるカスタムオブジェクトをサポートしていません。

1. 「**同期を有効にする**」をクリックします。

   ![](assets/image2015-4-22-10-3a45-3a50.png)

1. 「**同期を有効にする**」を再度クリックします。

   ![](assets/image2015-4-22-10-3a46-3a10.png)

   >[!NOTE]
   >
   >グローバル同期を再度有効にするのを忘れないでください。

1. **Salesforce**&#x200B;タブに戻ります。

   ![](assets/image2015-4-22-10-3a46-3a25.png)

1. 「**同期を有効にする**」をクリックします。

   ![](assets/image2015-4-22-10-3a50-3a26.png)

1. すべてのSalesforceカスタムオブジェクトを表示するには、**管理者**&#x200B;をクリックし、**Salesforceオブジェクト同期**&#x200B;リンク（上記の手順1と同じ）をクリックします。

   ![](assets/image2016-6-23-9-3a28-3a23.png)

   >[!NOTE]
   >
   >マーケティング担当者は、1 ～ 2レベルの深さの標準エンティティにリンクされたカスタムエンティティのみをサポートしています。

### 次の作業：{#whats-next}

[スマートリスト/トリガー制約としての追加カスタムオブジェクトフィールドの削除](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md)

素晴らしい！ このカスタムオブジェクトのデータをスマートキャンペーンおよびスマートリストで使用できるようになりました。
