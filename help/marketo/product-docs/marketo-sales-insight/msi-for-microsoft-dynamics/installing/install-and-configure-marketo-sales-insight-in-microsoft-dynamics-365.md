---
unique-page-id: 3571739
description: Marketo Sales Insight の Microsoft Dynamics 365 へのインストールと設定 - Marketo ドキュメント - 製品ドキュメント
title: Marketo Sales Insight の Microsoft Dynamics 365 へのインストールと設定
exl-id: c1f06b8c-48fd-4015-9502-7c9693632589
source-git-commit: 17cacaa56a437a568bd0d2cc23020f3f880eaf52
workflow-type: ht
source-wordcount: '458'
ht-degree: 100%

---

# Marketo Sales Insight の Microsoft Dynamics 365 へのインストールと設定 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight は、マーケティングチームが持つ豊富なデータをセールスチームに「窓」として提供するための素晴らしいツールです。インストールと設定方法を次に示します。

>[!PREREQUISITES]
>
>Marketo と Microsoft の統合を完了します。
>
>お使いのバージョンの Microsoft Dynamics CRM に[適したソリューションをダウンロードします](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md)。

## ソリューションのインポート {#import-solution}

1. [Microsoft Office 365](https://login.microsoftonline.com/).にログインします。

   ![](assets/image2015-3-16-15-58-55.png)

1. ![-](assets/image2015-3-16-16-1-13.png) メニューをクリックし、「**CRM**」を選択します。

   ![](assets/image2015-3-16-16-0-10.png)

1. ![--](assets/image2015-5-13-10-5-8.png) メニューをクリックします。ドロップダウンで、「**設定**」を選択し、「**ソリューション**」を選択します。

   ![](assets/image2015-5-13-10-4-1.png)

   >[!NOTE]
   >
   >次に進む前に、あらかじめ Marketo ソリューションを[&#128279;](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md)インストールして設定しておく必要があります。

1. 「**インポート**」をクリックします。

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. 新しいウィンドウで、「**参照**」をクリックします。[手順 1 でダウンロードした Marketo Sales Insight ソリューション](#msi)を選択します。「**次へ**」をクリックします。

   ![](assets/image2015-5-13-15-3a38-3a49.png)

1. ソリューションがアップロードされます。必要に応じて、パッケージの内容を表示できます。「**次へ**」をクリックします。

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. ボックスが&#x200B;**チェック**&#x200B;されていることを確認して、「**インポート**」をクリックします。

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. ログファイルを任意にダウンロードして、「**閉じる**」をクリックします。

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. これで完了です。ソリューションがすぐに表示されます。表示されない場合は、画面を更新します。

   ![](assets/image2015-5-13-15-3a42-3a29.png)

1. 「**すべてのカスタマイズを公開**」をクリックします。

   ![](assets/image2015-11-10-11-3a15-3a40.png)

## Marketo と Sales Insight の接続 {#connect-marketo-and-sales-insight}

Marketo インスタンスを Dynamics の Sales Insight に接続します。その方法をご紹介します。

>[!NOTE]
>
>**管理者権限が必要**

1. Marketo にログインし、**管理者**&#x200B;セクションに移動します。

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. 「**Sales Insight**」セクションで、「**API 設定を編集**」をクリックします。

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. 「**Marketo ホスト**」、「**API URL**」、「**API ユーザー ID**」をコピーして、後の手順で使用します。任意の **API 秘密鍵**&#x200B;を入力し、「**保存**」をクリックします。

   >[!CAUTION]
   >
   >API 秘密鍵にはアンパサンド（&amp;）を使用しないでください。

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >Sales Insight を機能させるには、_リードと連絡先の両方_&#x200B;で、次のフィールドを Marketo と同期する必要があります。
   >
   > * 優先度
   > * 緊急度
   > * 相対スコア
   >
   >これらのフィールドのいずれかが見つからない場合は、見つからないフィールドの名前のエラーメッセージが Marketo に表示されます。これを修正するには、[この手順](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md)を実行します。

1. Microsoft Dynamics に戻り、「設定」の横にある ![](assets/image2015-5-13-15-3a49-3a19.png) アイコンをクリックし、ドロップダウンから「**Marketo API 設定**」を選択します。

   ![](assets/image2015-5-13-16-3a4-3a1.png)

1. 「**デフォルト設定**」をクリックします。

   ![](assets/image2015-5-13-16-3a5-3a2.png)

1. 先ほど Marketo からコピーした情報を入力します。

   ![](assets/image2015-5-13-16-3a7-3a6.png)

1. 右下隅にある ![](assets/image2015-5-13-16-3a8-3a51.png) アイコンをクリックして、変更を保存します。

## ユーザーアクセスの設定 {#set-user-access}

Sales Insight を使用するには、ユーザーに権限を付与する必要があります。

1. ![](assets/image2015-5-13-10-3a5-3a8.png) メニューをクリックします。ドロップダウンメニューで「**設定**」を選択し、「**セキュリティ**」を選択します。

   ![](assets/image2015-5-13-16-3a12-3a12.png)

1. 「**ユーザー**」をクリックします。

   ![](assets/image2015-4-29-14-3a57-3a46.png)

1. Sales Insight へのアクセス権を付与するユーザーを選択し、「**役割の管理**」をクリックします。

   ![](assets/image2015-4-29-14-3a59-3a31.png)

1. **Marketo Sales Insight** の役割を選択し、「**OK**」をクリックします。

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   これですべて完了です。最後に、Marketo Sales Insight にアクセスし、リードや連絡先を調べるユーザーとして Dynamics にログインし、テストを実施します。

   ![](assets/image2015-4-29-15-3a2-3a27.png)

これで、セールスチームに Marketo Sales Insight を活用してもらえるようになりました。

>[!MORELIKETHIS]
>
>[リード／連絡先レコードの星と炎の設定](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
