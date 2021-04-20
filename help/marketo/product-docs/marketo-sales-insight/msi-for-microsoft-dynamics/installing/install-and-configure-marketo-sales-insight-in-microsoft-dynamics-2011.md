---
unique-page-id: 3571735
description: Microsoft Dynamics 2011 -Marketoドキュメント — 製品ドキュメントで、Marketo販売インサイトをインストールおよび構成します
title: Microsoft Dynamics 2011でのMarketo販売インサイトのインストールと構成
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 1%

---


# Microsoft Dynamics 2011でのMarketo販売インサイトのインストールと構成{#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo・セールス・インサイトは、セールス・チームにとって素晴らしいツールです。 Microsoft Dynamics 2011オンプレミスでのインストールと構成の手順を説明します。

>[!PREREQUISITES]
>
>Marketoとマイクロソフトの統合を完了します。
>
>[お使いのバージョンのMicrosoft Dynamics CRMに適した](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) ソリューションをダウンロードしてください。

## ソリューションのインポート{#import-solution}

1. Microsoft Dynamics CRMにサインインします。 左下のメニューで[**設定**]をクリックします。

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. ツリーで&#x200B;**ソリューション**&#x200B;を選択します。

   ![](assets/image2015-5-4-10-3a41-3a56.png)

1. **インポート** (![](assets/image2015-5-4-10-3a45-3a44.png))をクリックします。

   ![](assets/image2015-5-4-10-3a42-3a38.png)

   >[!NOTE]
   >
   >先に進む前に、[Marketoソリューションをインストールし、](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2011.md)設定しておく必要があります。

1. 「**参照**」をクリックします。 [ダウンロード](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md)したMarketoセールスインサイトソリューションを選択します。 「**次へ**」をクリックします。

   ![](assets/image2015-5-4-10-3a55-3a15.png)

1. ソリューションの詳細を確認し、「**次へ**」をクリックします。

   ![](assets/image2015-5-4-10-3a57-3a31.png)

1. 「SDKメッセージ」オプションがオンになっていることを確認します。 「**次へ**」をクリックします。

   ![](assets/image2015-5-4-11-3a43-3a37.png)

1. 次に、インポートが終了するのを待ちます。

   ![](assets/image2015-5-4-11-3a0-3a58.png)

1. 「**閉じる**」をクリックします。

   ![](assets/crmhand.png)

1. Marketoのセールス・インサイトが、ソリューション・リストに表示されます。 やった！

   ![](assets/image2015-5-4-11-3a2-3a37.png)

1. 「Marketo販売インサイト」を選択し、「**すべてのカスタマイズを発行**(![](assets/image2015-5-4-11-3a7-3a8.png))」をクリックします。

   ![](assets/image2015-5-4-11-3a8-3a27.png)

## MarketoとSales Insightを接続{#connect-marketo-and-sales-insight}

>[!NOTE]
>
>**必要な管理者権限**

1. Marketoにログインし、**管理者**&#x200B;をクリックします。

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. 「**Sales Insight**」セクションで、「**Edit API Configuration**」をクリックします。

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. 後の手順で使用する&#x200B;**Marketoホスト**、**API URL**、**APIユーザーID**&#x200B;をコピーします。 任意の&#x200B;**API秘密キー**&#x200B;を入力し、「**保存**」をクリックします。

   >[!CAUTION]
   >
   >API秘密鍵にアンパサンド(&amp;)を使用しないでください。

   ![](assets/image2015-5-4-11-3a16-3a3.png)

   >[!NOTE]
   >
   >Sales Insightを機能させるには、次のフィールドをMarketoと同期して、_リードと連絡先_&#x200B;の両方を行う必要があります。
   >
   >* 優先順位
   >* 緊急度
   >* 相対スコア

   >
   >これらのフィールドのいずれかが見つからない場合は、Marketoに、見つからないフィールドの名前のエラーメッセージが表示されます。 この問題を修正するには、[この手順](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md)を実行します。

1. [ダイナミクス]に戻り、[**設定**]を選択します。

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. ツリーで&#x200B;**MarketoAPI Config**&#x200B;を選択します。

   ![](assets/image2015-5-4-11-3a22-3a41.png)

1. 「**デフォルト設定**」をクリックします。

   ![](assets/image2015-5-4-11-3a26-3a10.png)

1. 先ほどMarketoから受け取った情報を入力します。

   ![](assets/image2015-5-4-11-3a27-3a16.png)

1. 「**保存**」をクリックします。

   ![](assets/image2015-5-4-11-3a28-3a13.png)

## ユーザーアクセスの設定{#set-user-access}

特定のユーザーにSales Insightへのアクセス権を与えるユーザーロールを設定します。

1. **設定**&#x200B;を選択します。

   ![](assets/image2015-5-4-11-3a30-3a54.png)

1. ツリーで[**管理**]を選択します。

   ![](assets/image2015-5-4-11-3a31-3a39.png)

1. 「**ユーザー**」をクリックします。

   ![](assets/image2015-5-4-11-3a32-3a25.png)

1. アクセス権を付与するユーザーを選択し、**ロールの管理**&#x200B;をクリックします。

   ![](assets/image2015-5-4-11-3a35-3a8.png)

1. **Marketo販売インサイト**&#x200B;のロールを選択し、「**OK**」をクリックします。

   ![](assets/image2015-5-4-11-3a36-3a59.png)

   それだ！ すべてのユーザーがアクセス権を持つと、リード/連絡先の詳細表示の「販売インサイト」セクションを表示できます。

   ![](assets/image2015-5-4-11-3a39-3a23.png)

   おめでとう。 これで、Marketo・セールス・インサイトの機能が解放されました。

>[!MORELIKETHIS]
>
>[リード/接触レコードの星と炎の設定](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
