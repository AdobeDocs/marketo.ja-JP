---
unique-page-id: 3571735
description: Marketo セールスインサイトの Microsoft Dynamics 2011 へのインストールと設定 - Marketo ドキュメント - 製品ドキュメント
title: Marketo セールスインサイトの Microsoft Dynamics 2011 へのインストールと設定
exl-id: 40622dcc-7129-4392-95dc-ca829c15c3a6
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '371'
ht-degree: 100%

---

# [!DNL Microsoft Dynamics 2011] での [!DNL Marketo Sales Insight] のインストールと設定 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

[!DNL Marketo Sales Insight] は、セールスチームが使えるとても便利なツールです。[!DNL Microsoft Dynamics 2011] オンプレミスで Marketo セールスインサイトをインストールし、設定する方法を、以下に順を追って説明します。

>[!PREREQUISITES]
>
>Marketo と Microsoft の統合を完了します。
>
>お使いのバージョンの [!DNL Microsoft Dynamics] CRM に[適したソリューションをダウンロードします](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md)。

## ソリューションの読み込み {#import-solution}

1. [!DNL Microsoft Dynamics] CRM にログインします。左下のメニューで「**[!UICONTROL 設定]**」をクリックします。

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. ツリーで「**[!UICONTROL ソリューション]**」を選択します。

   ![](assets/image2015-5-4-10-3a41-3a56.png)

1. **インポート**（![](assets/image2015-5-4-10-3a45-3a44.png)）をクリックします。

   ![](assets/image2015-5-4-10-3a42-3a38.png)

   >[!NOTE]
   >
   >次に進む前に、あらかじめ Marketo ソリューションを[インストールして設定](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2011.md)しておく必要があります。

1. 「**[!UICONTROL 参照]**」をクリックします。[ダウンロード](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md)した [!DNL Marketo Sales Insight] ソリューションを選択します。「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/image2015-5-4-10-3a55-3a15.png)

1. ソリューションの詳細を確認し、「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/image2015-5-4-10-3a57-3a31.png)

1. 「SDK メッセージ」オプションがオンになっていることを確認します。「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/image2015-5-4-11-3a43-3a37.png)

1. インポートが完了するまで待ちます。

   ![](assets/image2015-5-4-11-3a0-3a58.png)

1. 「**[!UICONTROL 閉じる]**」をクリックします。

   ![](assets/crmhand.png)

1. [!DNL Marketo Sales Insight] がソリューションリストに表示されます。これで完了です。

   ![](assets/image2015-5-4-11-3a2-3a37.png)

1. 「[!DNL Marketo Sales Insight]」を選択し、「**すべてのカスタマイズを公開**」（![](assets/image2015-5-4-11-3a7-3a8.png)）をクリックします。

   ![](assets/image2015-5-4-11-3a8-3a27.png)

## Marketo と Sales Insight の接続  {#connect-marketo-and-sales-insight}

>[!NOTE]
>
>**管理者権限が必要**

1. Marketo にログインし、**[!UICONTROL 管理]**&#x200B;をクリックします。

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. **[!UICONTROL Sales Insight]** セクションで、「**[!UICONTROL API 設定を編集]**」をクリックします。

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. 「**[!UICONTROL Marketo ホスト]**」、「**[!UICONTROL API URL]**」、「**[!UICONTROL API ユーザー ID]**」をコピーして、後の手順で使用します。任意の **[!UICONTROL API 秘密鍵]**&#x200B;を入力し、「**[!UICONTROL 保存]**」をクリックします。

   >[!CAUTION]
   >
   >API 秘密鍵にはアンパサンド（&amp;）を使用しないでください。

   ![](assets/image2015-5-4-11-3a16-3a3.png)

   >[!NOTE]
   >
   >Sales Insight を機能させるには、_リードと連絡先の両方_&#x200B;で、次のフィールドを Marketo と同期する必要があります。
   >
   >* 優先度
   >* 緊急度
   >* 相対スコア
   >
   >これらのフィールドのいずれかが見つからない場合は、見つからないフィールドの名前のエラーメッセージが Marketo に表示されます。これを修正するには、[この手順](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md)を実行します。

1. Dynamics に戻り、「**[!UICONTROL 設定]**」を選択します。

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. ツリーで「**[!UICONTROL Marketo API 設定]**」を選択します。

   ![](assets/image2015-5-4-11-3a22-3a41.png)

1. 「**[!UICONTROL デフォルト設定]**」をクリックします。

   ![](assets/image2015-5-4-11-3a26-3a10.png)

1. 先ほど Marketo から取得した情報を入力します。

   ![](assets/image2015-5-4-11-3a27-3a16.png)

1. 「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2015-5-4-11-3a28-3a13.png)

## ユーザーアクセスの設定 {#set-user-access}

特定のユーザに [!DNL Sales Insight] へのアクセス権を付与するユーザのロールを設定します。

1. 「**[!UICONTROL 設定]**」を選択します。

   ![](assets/image2015-5-4-11-3a30-3a54.png)

1. ツリーで&#x200B;**[!UICONTROL 「管理」]**&#x200B;を選択します。

   ![](assets/image2015-5-4-11-3a31-3a39.png)

1. 「**[!UICONTROL ユーザー]**」をクリックします。

   ![](assets/image2015-5-4-11-3a32-3a25.png)

1. アクセス権を付与するユーザーを選択し、「**[!UICONTROL 役割を管理]**」をクリックします。

   ![](assets/image2015-5-4-11-3a35-3a8.png)

1. **[!UICONTROL Marketo セールスインサイト]**&#x200B;のロールを選択し、「**[!UICONTROL OK]**」をクリックします。

   ![](assets/image2015-5-4-11-3a36-3a59.png)

   これで完了です。これで、アクセス権を持つユーザーすべてが、リード／取引先責任者の詳細ビューで Sales Insight のセクションを閲覧できるようになりました。

   ![](assets/image2015-5-4-11-3a39-3a23.png)

   おめでとうございます。これで、[!DNL Marketo Sales Insight] を活用できるようになりました。

>[!MORELIKETHIS]
>
>[リード／取引先責任者レコードの星と炎の設定](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
