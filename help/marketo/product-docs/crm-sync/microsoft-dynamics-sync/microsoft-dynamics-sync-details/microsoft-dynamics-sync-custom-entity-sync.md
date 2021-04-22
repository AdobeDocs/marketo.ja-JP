---
unique-page-id: 3571846
description: Microsoft Dynamics Sync — カスタムエンティティ同期 —Marketoドキュメント — 製品ドキュメント
title: Microsoft Dynamics Sync — カスタムエンティティ同期
exl-id: 1e175bd4-509f-4c1f-a41d-456629e4a8fb
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 0%

---

# Microsoft Dynamics同期：カスタムエンティティ同期{#microsoft-dynamics-sync-custom-entity-sync}

DynamicsのデータをMarketoで使用できるようにするために、初期のカスタムエンティティ同期を有効にする必要がある場合は、次の方法で行います。

>[!NOTE]
>
>**必要な管理者権限**

>[!PREREQUISITES]
>
>カスタムオブジェクトを使用するには、Dynamicsの[リード](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md)、[連絡先](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md)、または[アカウント](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md)オブジェクトに関連付ける必要があります。

>[!CAUTION]
>
>カスタムエンティティの同期を開始する前に、初期同期が完了している（電子メールで通知される）ことを確認します。

1. 「管理者」セクションに移動します。

   ![](assets/image2014-10-20-14-3a32-3a16.png)

1. 「**同期を無効にする**」をクリックして、標準のグローバル同期を一時的に無効にします。

   ![](assets/image2015-11-10-9-3a0-3a6.png)

1. カスタムエンティティの同期（2_0_0_2の後）をサポートするバージョンのMicrosoft Dynamicsをインストールします。 [MIcrosoft DynamicsのMarketoプラグインリリース](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/marketo-plugin-releases-for-microsoft-dynamics.md)を参照してください。

1. 同期するエンティティに対して、Marketo同期ユーザに読み取りアクセス権を与えます。

1. [データベースの管理]で、**Dynamicsエンティティの同期**&#x200B;リンクをクリックします。

   ![](assets/image2015-11-10-9-3a6-3a55.png)

1. 「**スキーマ**&#x200B;を同期」リンクをクリックして、使用可能なカスタムエンティティのリストを表示します。

   ![](assets/image2015-11-10-9-3a41-3a37.png)

1. リストの同期後、同期するフィールドと、スマートリストで[制約](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md)やトリガーとして使用するフィールドを選択します。 完了したら、「**同期を有効にする**」をクリックします。

   ![](assets/image2014-10-20-14-3a32-3a55.png)

1. グローバル同期を再度有効にします。

   ![](assets/image2015-11-10-9-3a48-3a35.png)

   >[!NOTE]
   >
   >Marketoは、1レベルまたは2レベルの深さの標準エンティティにリンクされたカスタムエンティティのみをサポートします。

   >[!NOTE]
   >
   >エンティティ名は最大&#x200B;**33文字**&#x200B;まで入力できます。

いいぞ！
