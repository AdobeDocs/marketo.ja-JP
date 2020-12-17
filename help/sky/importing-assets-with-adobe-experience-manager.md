---
title: importing-assets-with-adobe-experience-manager
description: Adobe Experience Managerでのアセットの読み込み
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '240'
ht-degree: 0%

---


# Adobe Experience Managerでのアセットの読み込み

<br> 

アセット選択を使用すると、[!DNL Marketo]ユーザーはAEMアセットにアクセス、選択、および[!DNL Marketo's] [!UICONTROL Design Studio]への読み込みを実行できます。 これらの手順を実行するには、管理者である必要があります。

>[!NOTE]
>[!DNL Adobe Experience Manager (AEM)] は独立した製品で、個別に購入する必要があります。 詳しくは、カスタマーサクセスマネージャーにお問い合わせください。

>[!IMPORTANT]
>[!DNL Marketo Classic]の[AEM設定](https://docs.marketo.com/x/FwPLAQ)を既に実行済みであることを確認してください。

>[!CAUTION]
>
>現在、この機能はFirefoxでのみ完全にサポートされています。 Safariではサポートされていないため、SameSite Cookieの設定によっては、最新バージョンのChromeでは動作しない場合があります。

1. [!UICONTROL Design Studio]で、「**[!UICONTROL 画像とファイル]**」を選択します。

   ![イメージ1](/help/sky/assets/design-studio/importing-assets-with-adobe-experience-manager/importing-assets-with-adobe-experience-manager-1.png)

1. 「[!UICONTROL 画像とファイル]」ドロップダウンをクリックし、「**[!UICONTROL 画像またはファイルの読み込み]**」を選択します。

   ![イメージ2](/help/sky/assets/design-studio/importing-assets-with-adobe-experience-manager/importing-assets-with-adobe-experience-manager-2.png)

1. [!DNL Adobe Experience Manager]の横のラジオボタンをクリックし、**[!UICONTROL 次へ]**&#x200B;をクリックします。

   ![イメージ3](/help/sky/assets/design-studio/importing-assets-with-adobe-experience-manager/importing-assets-with-adobe-experience-manager-3.png)

1. [!DNL Adobe Experience Manager]にログインします。

   ![画像4](/help/sky/assets/design-studio/importing-assets-with-adobe-experience-manager/importing-assets-with-adobe-experience-manager-4.png)

1. フォルダーを選択します。 目的の画像を選択し（10個まで選択できます）、「**[!UICONTROL 選択]**」をクリックします。

   ![画像5](/help/sky/assets/design-studio/importing-assets-with-adobe-experience-manager/importing-assets-with-adobe-experience-manager-5.png)

   >[!NOTE]
   >
   >画像のサイズは100 MBを超えることはできません。

1. 選択した画像を確認し、保存先フォルダー（[!UICONTROL 画像とファイル]がデフォルト）を選択して、「**[!UICONTROL 次へ]**」をクリックします。

   ![画像6](/help/sky/assets/design-studio/importing-assets-with-adobe-experience-manager/importing-assets-with-adobe-experience-manager-6.png)

それだ！ 「**[!UICONTROL 閉じる]**」をクリックして、「画像とファイル」に戻ります。

![画像7](/help/sky/assets/design-studio/importing-assets-with-adobe-experience-manager/importing-assets-with-adobe-experience-manager-7.png)

## 注意事項

* [!DNL Marketo] 現在、 [!DNL Adobe Experience Manager] バージョン6.4と6.5をサポートしています。
* インスタンス内のすべてのユーザは、読み込んだ画像に表示したり、アクセスしたりできます。
* 画像は自動的に更新されません。 [!DNL Marketo] [!UICONTROL Design Studio]に読み込んだ画像がAEMで更新された場合は、手動で[!DNL Marketo]に再読み込みする必要があります。
