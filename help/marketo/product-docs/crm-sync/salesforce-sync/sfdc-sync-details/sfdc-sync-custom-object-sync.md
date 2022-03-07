---
unique-page-id: 2953471
description: SFDC 同期 - カスタムオブジェクトの同期  - Marketo ドキュメント - 製品ドキュメント
title: SFDC 同期 - カスタムオブジェクトの同期
exl-id: e491e0bc-04a9-4e78-97c3-a25b945d546a
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '214'
ht-degree: 100%

---

# SFDC 同期：カスタムオブジェクトの同期 {#sfdc-sync-custom-object-sync}

Salesforce インスタンスで作成されたカスタムオブジェクトも、Marketo の一部にすることができます。その設定方法を説明しましょう。

>[!NOTE]
>
>**管理者権限が必要**

>[!PREREQUISITES]
>
>カスタムオブジェクトを使用するには、カスタムオブジェクトは Salesforce で[リード](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-field-sync.md)、[連絡先](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md)、[アカウント](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md)オブジェクトのいずれかに関連付けられている必要があります。

## カスタムオブジェクトの有効化  {#enable-custom-object}

1. **管理者**／**Salesforce オブジェクト同期**&#x200B;リンクをクリックします。

   ![](assets/image2015-11-19-10-3a28-3a5.png).

1. これが最初のカスタムオブジェクトの場合は、「**スキーマを同期**」をクリックします。

   ![](assets/rtaimage-2.png)

1. 「**グローバル同期を無効にする**」をクリックします。

   ![](assets/image2015-4-22-10-3a45-3a0.png)

   >[!NOTE]
   >
   >Salesforce カスタムオブジェクトスキーマの初期同期には、数分かかる場合があります。

   ![](assets/image2015-4-22-10-3a45-3a18.png)

1. 同期するカスタムオブジェクトをキャンバスにドラッグします。

   ![](assets/image2015-4-22-10-3a45-3a30.png)

   >[!NOTE]
   >
   >カスタムオブジェクトには一意の名前が必要です。Marketo では、同名の 2 つの異なるカスタムオブジェクトはサポートされていません。

1. 「**同期を有効にする**」をクリックします。

   ![](assets/image2015-4-22-10-3a45-3a50.png)

1. 「**同期を有効にする**」を再度クリックします。

   ![](assets/image2015-4-22-10-3a46-3a10.png)

   >[!NOTE]
   >
   >忘れずにグローバル同期を再度有効にしてください。

1. 「**Salesforce**」タブに戻ります。

   ![](assets/image2015-4-22-10-3a46-3a25.png)

1. 「**同期を有効にする**」をクリックします。

   ![](assets/image2015-4-22-10-3a50-3a26.png)

1. すべての Salesforce カスタムオブジェクトを表示するには、**管理者**／**Salesforce オブジェクト同期**&#x200B;リンクをクリックします（上記の手順 1 と同じ）。

   ![](assets/image2016-6-23-9-3a28-3a23.png)

   >[!NOTE]
   >
   >Marketo では、1 レベルまたは 2 レベルの深さの標準エンティティにリンクされたカスタムエンティティのみがサポートされています。

### 次の手順： {#whats-next}

[スマートリスト／トリガー制約としてのカスタムオブジェクトフィールドの追加／の削除](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md)

これで完了です。これで、このカスタムオブジェクトのデータをスマートキャンペーンとスマートリストで使用できるようになりました。
