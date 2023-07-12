---
unique-page-id: 37355768
description: Adobe Experience Manager でのアセットの読み込み - Marketo ドキュメント - 製品ドキュメント
title: Adobe Experience Manager でのアセットの読み込み
exl-id: 56ccf38f-3c99-4018-9989-719854e37a20
source-git-commit: dd4fb7dfc92580c58da70d603b6d92bd8f64493c
workflow-type: tm+mt
source-wordcount: '224'
ht-degree: 71%

---

# Adobe Experience Manager でのアセットの読み込み {#importing-assets-with-adobe-experience-manager}

アセットセレクターを使用すると、Marketoのお客様は、AEMアセットにアクセスし、選択し、Marketoに読み込むことができます [!DNL Design Studio]. **管理者権限が必要です**。

>[!AVAILABILITY]
>
>必ずしもすべてのお客様がこの機能を購入済みとは限りません。詳しくは、アドビアカウントチーム（担当のアカウントマネージャー）にお問い合わせください。

>[!PREREQUISITES]
>
>[AEM 設定](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/configuring-adobe-experience-manager-integration.md)を既に実行済みであることを確認します。

>[!IMPORTANT]
>
>現在、この機能はでのみ完全にサポートされています。 [!DNL Firefox]. ではサポートされていません。 [!DNL Safari]最新バージョンの [!DNL Chrome]、 [!DNL SameSite] cookie の設定に基づいて )。

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

* 画像は自動的にはアップデートされません。画像をMarketoに読み込んだ場合 [!DNL Design Studio] がAEMで更新されたので、Marketoに手動で再度読み込む必要があります。
