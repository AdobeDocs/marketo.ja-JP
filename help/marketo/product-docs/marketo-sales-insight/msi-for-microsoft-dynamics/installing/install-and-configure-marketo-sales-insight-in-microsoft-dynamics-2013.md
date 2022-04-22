---
unique-page-id: 3571737
description: Marketo Sales Insight の Microsoft Dynamics 2013 へのインストールと設定 - Marketo ドキュメント - 製品ドキュメント
title: Marketo Sales Insight の Microsoft Dynamics 2013 へのインストールと設定
exl-id: 290db451-47a6-4cfa-a36f-bc12ef7d3482
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '429'
ht-degree: 100%

---

# Marketo Sales Insight の Microsoft Dynamics 2013 へのインストールと設定 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight は、マーケティングチームが持つ豊富なデータをセールスチームに「窓」として提供するための素晴らしいツールです。インストールと設定方法を次に示します。

>[!PREREQUISITES]
>
>Marketo と Microsoft の統合を完了します。
>
>お使いのバージョンの Microsoft Dynamics CRM に[適したソリューションをダウンロードします](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md)。

## ソリューションのインポート {#import-solution}

次に、Marketo Sales Insight ソリューションを Microsoft Dynamics にインポートします。

1. **Microsoft Dynamics CRM** で、「**設定**」をクリックします。

   ![](assets/image2014-12-12-9-3a4-3a56.png)

1. 「**設定**」で、「**カスタマイズ**」をクリックします。

   ![](assets/image2014-12-12-9-3a5-3a6.png)

1. 「**ソリューション**」をクリックします。

   ![](assets/image2014-12-12-9-3a5-3a17.png)

   >[!NOTE]
   >
   >次に進む前に、あらかじめ Marketo をインストールして設定しておく必要があります

1. 「**インポート**」をクリックします。

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. 新しいウィンドウで、「**参照**」をクリックします。

   ![](assets/image2014-12-12-9-3a5-3a36.png)

1. 上記でダウンロードしたソリューションを見つけて選択します。

   ![](assets/image2014-12-12-9-3a5-3a45.png)

1. 「**次へ**」をクリックします。

   ![](assets/image2014-12-12-9-3a5-3a55.png)

1. ソリューションがアップロードされます。必要に応じて、パッケージの内容を表示できます。「**次へ**」をクリックします。

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. ボックスがチェックされていることを確認して、「**インポート**」をクリックします。

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. ログファイルを任意にダウンロードして、「**閉じる**」をクリックします。

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. これで完了です。ソリューションがすぐに表示されます。表示されない場合は、画面を更新します。

   ![](assets/image2014-12-12-9-3a6-3a40.png)

## Marketo と Sales Insight の接続 {#connect-marketo-and-sales-insight}

Marketo インスタンスを Dynamics の Sales Insight に接続します。

>[!NOTE]
>
>管理者権限が必要。

1. Marketo にログインし、「**管理者**」セクションに移動します。

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. **Sales Insight** セクションで、「**API 設定を編集**」をクリックします。

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
   >* 優先度
   >* 緊急度
   >* 相対スコア

   >
   >これらのフィールドのいずれかが見つからない場合は、見つからないフィールドの名前のエラーメッセージが Marketo に表示されます。これを修正するには、[この手順](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md)を実行します。

1. Microsoft Dynamics に戻り、「**設定**」に移動します。

   ![](assets/image2014-12-12-9-3a7-3a25.png)

1. 「**設定**」で、「**Marketo API 設定**」をクリックします。

   ![](assets/image2014-12-12-9-3a7-3a34.png)

1. 「**新規**」をクリックします。

   ![](assets/image2014-12-12-9-3a8-3a8.png)

1. 先ほど Marketo から取得した情報を入力し、「**保存**」をクリックします。

   ![](assets/image2014-12-12-9-3a8-3a17.png)

## ユーザーアクセスの設定 {#set-user-access}

最後に、特定のユーザーに Marketo Sales Insight のアクセス権を付与できます。

1. 「**設定**」に移動します。

   ![](assets/image2014-12-12-9-3a8-3a34.png)

1. 「**ユーザー**」をクリックします。

   ![](assets/image2014-12-12-9-3a8-3a42.png)

1. Sales Insight へのアクセス権を付与するユーザーを選択し、「**役割の管理**」をクリックします。

   ![](assets/image2014-12-12-9-3a9-3a13.png)

1. **Marketo Sales Insight** の役割を選択し、「**OK**」をクリックします。

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   これですべて完了です。最後に、Marketo Sales Insight にアクセスし、リードや連絡先を調べるユーザーとして Dynamics にログインし、テストを実施します。

   ![](assets/image2014-12-12-9-3a9-3a31.png)

これで、セールスチームに Marketo Sales Insight を活用してもらえるようになりました。

>[!MORELIKETHIS]
>
>[リード／連絡先レコードの星と炎の設定](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
