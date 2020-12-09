---
unique-page-id: 3571846
description: Microsoft Dynamics Sync — カスタムエンティティ同期 — Marketto Docs — 製品ドキュメント
title: Microsoft Dynamics Sync — カスタムエンティティ同期
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 0%

---


# Microsoft Dynamics同期：カスタムエンティティ同期 {#microsoft-dynamics-sync-custom-entity-sync}

DynamicsのデータをMarketoで使用できるようにするために、最初のカスタムエンティティ同期を有効にする必要がある場合は、次の方法を使用します。

>[!NOTE]
>
>**必要な管理者権限**

>[!PREREQUISITES]
>
>カスタムオブジェクトを使用するには、Dynamicsの [リード](microsoft-dynamics-sync-lead-sync.md)、 [連絡先](microsoft-dynamics-sync-contact-sync.md)、または [](microsoft-dynamics-sync-account-sync.md)アカウントオブジェクトに関連付ける必要があります。

>[!CAUTION]
>
>カスタムエンティティの同期を開始する前に、初期同期が完了している（電子メールで通知される）ことを確認します。

1. 「管理者」セクションに移動します。

   ![](assets/image2014-10-20-14-3a32-3a16.png)

1. 「同期を **無効にする** 」をクリックして、標準のグローバル同期を一時的に無効にします。

   ![](assets/image2015-11-10-9-3a0-3a6.png)

1. カスタムエンティティの同期（2_0_0_2の後）をサポートするバージョンのMicrosoft Dynamicsをインストールします。 Microsoft Dynamicsの [Marketoプラグインリリースを参照してください](../../../../product-docs/crm-sync/microsoft-dynamics-sync/marketo-plugin-releases-for-microsoft-dynamics.md)。
1. 同期する予定のエンティティに対する読み取りアクセス権を、マーケティング担当者に付与します。
1. [データベースの管理]で、[** Dynamicsエンティティ同期**]リンクをクリックします。

   ![](assets/image2015-11-10-9-3a6-3a55.png)

1. 「 **同期スキーマ** 」リンクをクリックして、使用可能なカスタムエンティティのリストを表示します。

   ![](assets/image2015-11-10-9-3a41-3a37.png)

1. リストの同期後、同期するフィールドと、スマートリストで [制約](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md) /トリガーとして使用するフィールドを選択します。 完了したら、「同期を **有効にする**」をクリックします。

   ![](assets/image2014-10-20-14-3a32-3a55.png)

1. グローバル同期を再度有効にします。

   ![](assets/image2015-11-10-9-3a48-3a35.png)

   >[!NOTE]
   >
   >マーケティング担当者は、1 ～ 2レベルの深さの標準エンティティにリンクされたカスタムエンティティのみをサポートしています。

   >[!NOTE]
   >
   >エンティティ名は最大** 33文字**まで指定できます。

いいぞ！