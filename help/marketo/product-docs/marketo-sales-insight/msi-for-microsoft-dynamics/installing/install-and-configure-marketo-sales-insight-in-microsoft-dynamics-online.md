---
unique-page-id: 37355602
description: Marketo セールスインサイトの Microsoft Dynamics Online へのインストールおよび設定 - Marketo ドキュメント - 製品ドキュメント
title: Marketo セールスインサイトの Microsoft Dynamics Online へのインストールおよび設定
exl-id: 3b58b109-96f9-427e-be5c-a8db270ffe69
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 100%

---

# [!DNL Microsoft Dynamics Online] での [!DNL Marketo Sales Insight] のインストールと設定 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics-online}

[!DNL Marketo Sales Insight] は、マーケティングチームが持つ豊富なデータをセールスチームに「窓」として提供する素晴らしいツールです。[!DNL Microsoft Dynamics Online] にインストールし、設定する方法は以下のとおりです。

>[!PREREQUISITES]
>
>Marketo と Microsoft の統合を完了します。
>
>お使いのバージョンの [!DNL Microsoft Dynamics CRM] に[適したソリューションをダウンロードします](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md)。

## ソリューションの読み込み {#import-solution}

>[!NOTE]
>
>統合インターフェイスを使用している場合は、下の手順 1 より前に、右上隅の「設定」アイコンをクリックし、「**[!UICONTROL 詳細設定]**」を選択します。

1. Microsoft Dynamics CRM で、「**[!UICONTROL 設定]**」をクリックします。

   ![](assets/image2014-12-12-9-3a4-3a56-1.png)

1. 「設定」で、「**[!UICONTROL カスタマイズ]**」をクリックします。

   ![](assets/image2015-4-29-14-3a22-3a1-1.png)

1. 「**[!UICONTROL ソリューション]**」をクリックします。

   ![](assets/image2014-12-12-9-3a5-3a17-1.png)

   >[!NOTE]
   >
   >次に進む前に、あらかじめ Marketo ソリューションをインストールして設定しておく必要があります。

1. 「**[!UICONTROL インポート]**」をクリックします。

   ![](assets/image2014-12-12-9-3a5-3a27-1.png)

1. 新しいウィンドウで、「**[!UICONTROL 参照]**」をクリックします。

   ![](assets/image2014-12-12-9-3a5-3a36-1.png)

1. お使いのコンピューターで、ダウンロードしたソリューションを探してインストールします。

1. 「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/seven.png)

1. ソリューションがアップロードされます。必要に応じて、パッケージの内容を表示できます。「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/image2014-12-12-9-3a6-3a10-1.png)

1. ボックスがチェックされていることを確認して、「**[!UICONTROL インポート]**」をクリックします。

   ![](assets/image2014-12-12-9-3a6-3a19-1.png)

1. ログファイルを任意にダウンロードして、「**[!UICONTROL 閉じる]**」をクリックします。

   ![](assets/image2014-12-12-9-3a6-3a29-1.png)

1. これで完了です。ソリューションがすぐに表示されます。表示されない場合は、画面を更新します。

   ![](assets/eleven.png)

1. 「**[!UICONTROL カスタマイズを公開]**」をクリックします。

   >[!NOTE]
   >
   >必ずグローバル [!DNL MS Dynamics] 同期を有効にしてください。

## Marketo と [!DNL Sales Insight] の接続 {#connect-marketo-and-sales-insight}

Marketo インスタンスを [!DNL Dynamics] で [!DNL Sales Insight] に関連付けましょう。手順は次のとおりです。

>[!NOTE]
>
>**管理者権限が必要**

1. Marketo にログインし、**[!UICONTROL 管理者]**&#x200B;セクションに移動します。

   ![](assets/image2014-12-12-9-3a6-3a50-1.png)

1. 「[!UICONTROL Sales Insight]」セクションで、「**[!UICONTROL API 設定を編集]**」をクリックします。

   ![](assets/image2014-12-12-9-3a7-3a0-1.png)

1. 「**[!UICONTROL Marketo ホスト]**」、「**[!UICONTROL API URL]**」、「**[!UICONTROL API ユーザー ID]**」をコピーして、後の手順で使用します。任意の API 秘密鍵を入力し、「**[!UICONTROL 保存]**」をクリックします。

   >[!CAUTION]
   >
   >API 秘密鍵にはアンパサンド（&amp;）を使用しないでください。

   ![](assets/image2014-12-12-9-3a7-3a9-1.png)

   >[!NOTE]
   >
   >[!DNL Sales Insight] を機能させるには、_リードと取引先責任者の両方_&#x200B;で、次のフィールドを Marketo と同期する必要があります。
   >
   >* 優先度
   >* 緊急度
   >* 相対スコア
   >
   >これらのフィールドのいずれかが見つからない場合は、見つからないフィールドの名前のエラーメッセージが Marketo に表示されます。これを修正するには、[この手順](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md)を実行します。

1. [!DNL Microsoft Dynamics] に戻り、「**[!UICONTROL 設定]**」に移動します。

   ![](assets/image2014-12-12-9-3a7-3a25-1.png)

1. 「**[!UICONTROL 設定]**」で、「**[!UICONTROL Marketo API 設定]**」をクリックします。

   ![](assets/image2014-12-12-9-3a7-3a34-1.png)

1. 「**[!UICONTROL 新規]**」をクリックします。

   ![](assets/image2014-12-12-9-3a8-3a8-1.png)

1. 先ほど Marketo から取得した情報を入力し、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2014-12-12-9-3a8-3a17-1.png)

## 同期の有効化 {#enable-sync}

1. Marketo で、「**[!UICONTROL 管理者]**」をクリックします。

   ![](assets/enable-one.png)

1. 「統合」で、「**[!UICONTROL Microsoft Dynamics]**」を選択します。

   ![](assets/enable-two.png)

1. 「**[!UICONTROL 同期を有効にする]**」をクリックします。

   ![](assets/enable-three.png)

1. 「[!UICONTROL フィールド同期の詳細]」の横にある「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/enable-four.png)

1. これにより、以前に無効にした MSI フィールド（[!UICONTROL 緊急度]、[!UICONTROL 相対スコア]、[!UICONTROL 優先度]）が&#x200B;_自動的_&#x200B;に選択されます。「**[!UICONTROL 保存]**」をクリックして、データの同期を開始します。

   ![](assets/enable-five.png)

## ユーザアクセスの設定 {#set-user-access}

最後に、[!DNL Marketo Sales Insight] を使用するには、特定のユーザにアクセス権を付与する必要があります。

1. 「**[!UICONTROL 設定]**」に移動します。

   ![](assets/image2014-12-12-9-3a8-3a34-1.png)

1. 「**[!UICONTROL セキュリティ]**」に移動します。

   ![](assets/image2015-4-29-14-3a56-3a33-1.png)

1. 「**[!UICONTROL ユーザ]**」をクリックします。

   ![](assets/image2015-4-29-14-3a57-3a46-1.png)

1. [!DNL Sales Insight] へのアクセス権を付与するユーザを選択し、「**[!UICONTROL ロールを管理]**」をクリックします。

   ![](assets/image2015-4-29-14-3a59-3a31-1.png)

1. [!DNL Marketo Sales Insight] ロールを選択して、「**[!UICONTROL OK]**」をクリックします。

   ![](assets/image2014-12-12-9-3a9-3a22-1.png)

   これですべて完了です。最後に、[!DNL Marketo Sales Insight] にアクセスし、リードや取引先責任者を調べるユーザとして [!DNL Dynamics] にログインし、テストを実施します。

   ![](assets/image2015-4-29-15-3a2-3a27-1.png)

>[!MORELIKETHIS]
>
>[リード／取引先責任者レコードの星と炎の設定](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
