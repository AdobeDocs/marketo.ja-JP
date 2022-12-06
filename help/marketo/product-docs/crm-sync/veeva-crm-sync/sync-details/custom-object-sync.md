---
description: カスタムオブジェクト同期 - Marketo ドキュメント - 製品ドキュメント
title: カスタムオブジェクト同期
hide: true
hidefromtoc: true
exl-id: 68bc14e7-dfc9-4dce-b159-24d734ee3c6f
source-git-commit: 2ce44b7c44517a6fdb3f616a3d69b25158ea4ec9
workflow-type: ht
source-wordcount: '205'
ht-degree: 100%

---

# カスタムオブジェクト同期 {#custom-object-sync}

Veeva CRM インスタンスで作成されたカスタムオブジェクトも、Marketo Engage の一部にすることができます。その設定方法を説明しましょう。

>[!NOTE]
>
>**管理者権限が必要**

>[!PREREQUISITES]
>
>カスタムオブジェクトを使用するには、Veeva CRM で取引先責任者またはアカウントオブジェクトに関連付けられている必要があります。

## カスタムオブジェクトの有効化 {#enable-custom-object}

1. Marketo で、「**管理者**」をクリックして、「**Veeva オブジェクト同期**」をクリックします。

   ![](assets/custom-object-sync-1.png)

1. これが最初のカスタムオブジェクトの場合は、「**スキーマを同期**」をクリックします。

   ![](assets/custom-object-sync-2.png)

1. 「**グローバル同期を無効にする**」をクリックします。

   ![](assets/custom-object-sync-3.png)

   >[!NOTE]
   >
   >Veeva カスタムオブジェクトスキーマの初回同期には、数分かかる場合があります。

1. 同期するカスタムオブジェクトをキャンバスにドラッグします。

   ![](assets/custom-object-sync-4.png)

   >[!NOTE]
   >
   >カスタムオブジェクトには一意の名前が必要です。Marketo では、同名の 2 つの異なるカスタムオブジェクトはサポートされていません。

1. 「**同期を有効にする**」をクリックします。

   ![](assets/custom-object-sync-5.png)

1. 「**同期を有効にする**」を再度クリックします。

   ![](assets/custom-object-sync-6.png)

1. 「**Veeva**」タブに戻ります。

   ![](assets/custom-object-sync-7.png)

1. 「**同期を有効にする**」をクリックします。

   ![](assets/custom-object-sync-8.png)

1. すべての Veeva カスタムオブジェクトを表示するには、「管理者」をクリックし、「Veeva オブジェクト同期」をクリックします。

   ![](assets/custom-object-sync-9.png)

   >[!NOTE]
   >
   >Marketo では、1 レベルから 2 レベルの深さの標準エンティティにリンクされたカスタムエンティティのみがサポートされています。

これで完了です。カスタムオブジェクトのデータをスマートキャンペーンとスマートリストで使用できるようになりました。

>[!MORELIKETHIS]
>
>* [通話と通話の主要メッセージの同期](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target=&quot;_blank&quot;}
>* [スマートリスト／トリガー制約としてのカスタムオブジェクトフィールドの追加／の削除](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target=&quot;_blank&quot;}

