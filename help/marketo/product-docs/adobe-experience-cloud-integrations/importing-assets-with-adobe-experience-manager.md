---
unique-page-id: 37355768
description: Adobe Experience Manager でのアセットの読み込み - Marketo ドキュメント - 製品ドキュメント
title: Adobe Experience Manager でのアセットの読み込み
exl-id: 56ccf38f-3c99-4018-9989-719854e37a20
feature: Integrations
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: ht
source-wordcount: '227'
ht-degree: 100%

---

# Adobe Experience Manager でのアセットの読み込み {#importing-assets-with-adobe-experience-manager}

アセットセレクターを使用すると、Marketo のお客様は、AEM アセットにアクセスし選択して、Marketo [!DNL Design Studio] に読み込むことができます。**管理者権限が必要です**。

>[!AVAILABILITY]
>
>必ずしもすべてのお客様がこの機能を購入済みとは限りません。詳しくは、アドビアカウントチーム（担当のアカウントマネージャー）にお問い合わせください。

>[!PREREQUISITES]
>
>[AEM 設定](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/configuring-adobe-experience-manager-integration.md)を既に実行済みであることを確認します。

>[!IMPORTANT]
>
>現在、この機能は [!DNL Firefox] でのみ完全にサポートされています。[!DNL Safari] ではサポートされていません。また、[!DNL SameSite] の Cookie 設定によっては、最新バージョンの [!DNL Chrome] では動作しない可能性があります。

1. **[!UICONTROL Design Studio]** をクリックします。

   ![](assets/importing-assets-with-adobe-experience-manager-1.png)

1. 新規ドロップダウンをクリックし、「**[!UICONTROL Adobe Experience Manager から読み込む]**」を選択します。

   ![](assets/importing-assets-with-adobe-experience-manager-2.png)

1. 画像を保存するフォルダーを選択します。

   ![](assets/importing-assets-with-adobe-experience-manager-3.png)

1. Adobe Experience Manager にログインします（まだログインしていない場合）。

   ![](assets/importing-assets-with-adobe-experience-manager-4.png)

1. フォルダーを選択します。次に、目的の画像をサムネールをクリックして選択します（最大 10 個選択できます）。終了したら「**[!UICONTROL 選択]**」をクリックします。

   ![](assets/importing-assets-with-adobe-experience-manager-5.png)

   >[!NOTE]
   >
   >画像のサイズは 100 MB を超えることはできません。

1. プロセスの最後に「**[!UICONTROL 読み込み]**」をクリックします。

   ![](assets/importing-assets-with-adobe-experience-manager-6.png)

   これで完了です。「**[!UICONTROL 閉じる]**」をクリックして、Design Studio に戻ります。

   ![](assets/importing-assets-with-adobe-experience-manager-7.png)

## 注意事項 {#things-to-note}

* Marketo は現在、Adobe Experience Manager バージョン 6.4 および 6.5 に対応しています。

* インスタンス内のすべてのユーザーが、読み込んだ画像を表示しアクセスできます。

* 画像は自動的にはアップデートされません。Marketo [!DNL Design Studio] に読み込んだ画像が AEM で更新された場合は、手動で Marketo に再読み込みする必要があります。
