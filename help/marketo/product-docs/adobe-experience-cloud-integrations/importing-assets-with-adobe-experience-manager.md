---
unique-page-id: 37355768
description: Adobe Experience Manager でのアセットの読み込み - Marketo ドキュメント - 製品ドキュメント
title: Adobe Experience Manager でのアセットの読み込み
exl-id: 56ccf38f-3c99-4018-9989-719854e37a20
source-git-commit: 12f45e694dccf1d9e51343b5eb9d743a8c513c1f
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 100%

---

# Adobe Experience Manager でのアセットの読み込み {#importing-assets-with-adobe-experience-manager}

アセットセレクターを使用すると、Marketo の顧客は、AEM のアセットにアクセスして選択し、Marketo Design Studio に読み込むことができます。**管理者権限が必要**。

>[!AVAILABILITY]
>
>この機能を購入しているのは一部の顧客のみです。詳しくは、カスタマーサクセスマネージャーにお問い合わせください。

>[!PREREQUISITES]
>
>[AEM 設定](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/configuring-adobe-experience-manager-integration.md)を既に実行済みであることを確認します。

>[!IMPORTANT]
>
>現在、この機能は Firefox でのみ完全にサポートされています。Safari ではサポートされていません。また、SameSite の Cookie 設定によっては、最新バージョンの Chrome では動作しない可能性があります。

1. **Design Studio** をクリックします。

   ![](assets/importing-assets-with-adobe-experience-manager-1.png)

1. 新規ドロップダウンをクリックし、「**Adobe Experience Manager から読み込む**」を選択します。

   ![](assets/importing-assets-with-adobe-experience-manager-2.png)

1. 画像を保存するフォルダーを選択します。

   ![](assets/importing-assets-with-adobe-experience-manager-3.png)

1. Adobe Experience Manager にログインします（まだログインしていない場合）。

   ![](assets/importing-assets-with-adobe-experience-manager-4.png)

1. フォルダーを選択します。次に、目的の画像をサムネールをクリックして選択します（最大 10 個選択できます）。終了したら「**選択**」をクリックします。

   ![](assets/importing-assets-with-adobe-experience-manager-5.png)

   >[!NOTE]
   >
   >画像のサイズは 100 MB を超えることはできません。

1. プロセスの最後に「**読み込み**」をクリックします。

   ![](assets/importing-assets-with-adobe-experience-manager-6.png)

   これで完了です。「**閉じる**」をクリックして、Design Studio に戻ります。

   ![](assets/importing-assets-with-adobe-experience-manager-7.png)

## 注意事項 {#things-to-note}

* Marketo は現在、Adobe Experience Manager バージョン 6.4 および 6.5 に対応しています。

* インスタンス内のすべてのユーザーが、読み込んだ画像を表示しアクセスできます。

* 画像は自動的にはアップデートされません。Marketo Design Studio に読み込んだ画像が AEM で更新された場合は、手動で Marketo に再読み込みする必要があります。
