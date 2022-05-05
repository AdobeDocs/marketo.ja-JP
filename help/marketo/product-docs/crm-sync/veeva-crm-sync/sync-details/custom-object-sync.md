---
description: カスタムオブジェクト同期 — Marketoドキュメント — 製品ドキュメント
title: カスタムオブジェクト同期
hide: true
hidefromtoc: true
exl-id: 68bc14e7-dfc9-4dce-b159-24d734ee3c6f
source-git-commit: 2ce44b7c44517a6fdb3f616a3d69b25158ea4ec9
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 29%

---

# カスタムオブジェクト同期 {#custom-object-sync}

Veeva CRM インスタンスで作成されたカスタムオブジェクトもMarketo Engageの一部です。 設定方法を次に示します。

>[!NOTE]
>
>**管理者権限が必要**

>[!PREREQUISITES]
>
>カスタムオブジェクトを使用するには、Veeva CRM の連絡先またはアカウントオブジェクトに関連付ける必要があります。

## カスタムオブジェクトの有効化 {#enable-custom-object}

1. Marketoで、 **管理者**&#x200B;を、 **Veeva オブジェクト同期**.

   ![](assets/custom-object-sync-1.png)

1. これが最初のカスタムオブジェクトの場合は、「**スキーマを同期**」をクリックします。

   ![](assets/custom-object-sync-2.png)

1. 「**グローバル同期を無効にする**」をクリックします。

   ![](assets/custom-object-sync-3.png)

   >[!NOTE]
   >
   >Veeva カスタムオブジェクトスキーマの初期同期には、数分かかる場合があります。

1. 同期するカスタムオブジェクトをキャンバスにドラッグします。

   ![](assets/custom-object-sync-4.png)

   >[!NOTE]
   >
   >カスタムオブジェクトには一意の名前が必要です。Marketo では、同名の 2 つの異なるカスタムオブジェクトはサポートされていません。

1. 「**同期を有効にする**」をクリックします。

   ![](assets/custom-object-sync-5.png)

1. 「**同期を有効にする**」を再度クリックします。

   ![](assets/custom-object-sync-6.png)

1. に戻ります。 **Veeva** タブをクリックします。

   ![](assets/custom-object-sync-7.png)

1. 「**同期を有効にする**」をクリックします。

   ![](assets/custom-object-sync-8.png)

1. すべての Veeva カスタムオブジェクトを表示するには、[ 管理者と Veeva オブジェクトの同期 ] をクリックします。

   ![](assets/custom-object-sync-9.png)

   >[!NOTE]
   >
   >Marketoでは、1 ～ 2 レベルの深さの標準エンティティにリンクされたカスタムエンティティのみがサポートされます。

これで完了です。スマートキャンペーンとスマートリストで、このカスタムオブジェクトのデータを使用できるようになりました。

>[!MORELIKETHIS]
>
>* [通話と通話の主要メッセージの同期](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target=&quot;_blank&quot;}
>* [スマートリスト/トリガー制約としてのカスタムオブジェクトフィールドの追加/削除](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target=&quot;_blank&quot;}

