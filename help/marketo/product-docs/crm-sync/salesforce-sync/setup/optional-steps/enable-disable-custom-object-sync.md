---
unique-page-id: 4719297
description: カスタムオブジェクト同期の有効化／無効化 - Marketo ドキュメント - 製品ドキュメント
title: カスタムオブジェクト同期の有効化／無効化
exl-id: f17d9135-b33e-48c0-9220-131fb437e9e5
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '218'
ht-degree: 100%

---

# カスタムオブジェクト同期の有効化／無効化 {#enable-disable-custom-object-sync}

Salesforce インスタンスで作成されたカスタムオブジェクトも、Marketo の一部にすることができます。その設定方法を説明しましょう。

## カスタムオブジェクト同期の有効化／無効化 {#enable-disable-custom-object-sync-1}

>[!NOTE]
>
>管理者権限が必要。

1. 「**管理者**」をクリックします。

   ![](assets/one.png)

1. データベース管理メニューで、「**Salesforce オブジェクト同期**」をクリックします。

   ![](assets/two-2.png)

1. これが最初のカスタムオブジェクトの場合は、「**スキーマを同期**」をクリックします。それ以外の場合は、「**スキーマを更新**」をクリックして最新の情報を取得します。

   ![](assets/image2014-12-10-10-3a14-3a44.png)

1. グローバル同期が実行中の場合は、「**グローバル同期を無効にする**」をクリックして無効化します。

   ![](assets/image2014-12-10-10-3a14-3a54.png)

   >[!NOTE]
   >
   >Salesforce カスタムオブジェクトスキーマの同期には、数分かかる場合があります。

1. 「**スキーマを更新**」をクリックします。

   ![](assets/image2014-12-10-10-3a15-3a7.png)

1. 同期するオブジェクトを選択し、「**同期を有効にする**」をクリックします。

   >[!TIP]
   >
   >Marketo では、Salesforce のリード、連絡先、アカウントオブジェクトのいずれかと直接の関係がある場合にのみ、カスタムオブジェクトを同期できます。

   ![](assets/image2014-12-10-10-3a15-3a30.png)

1. 「**同期を有効にする**」を再度クリックします。

   ![](assets/image2014-12-10-10-3a15-3a40.png)

1. 「**Salesforce**」タブに戻って、「**同期を有効にする**」をクリックします。

   ![](assets/image2014-12-10-10-3a15-3a49.png)

## カスタムオブジェクトの使用 {#using-your-custom-objects}

>[!NOTE]
>
>スマートキャンペーンでは、カスタムオブジェクトをトリガーと共に使用することはできません。

1. スマートリストで、**商談あり**&#x200B;フィルターをドラッグして、**true** に設定します。

   ![](assets/image2015-8-26-9-3a39-3a28.png)

1. 次に、フィルター制約を使用してフォーカスを絞り込みます。

   ![](assets/image2015-8-24-14-3a18-3a53.png)

   これで完了です。これで、このカスタムオブジェクトのデータをスマートキャンペーンとスマートリストで使用できるようになりました。

>[!MORELIKETHIS]
>
>[スマートリスト／トリガー制約としてのカスタムオブジェクトフィールドの追加／の削除](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md)
