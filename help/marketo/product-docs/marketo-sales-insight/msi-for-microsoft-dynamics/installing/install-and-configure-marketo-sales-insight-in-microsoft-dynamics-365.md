---
unique-page-id: 3571739
description: Microsoft Dynamics 365 -Marketoドキュメント — 製品ドキュメントで、Marketo販売インサイトをインストールおよび構成します
title: Microsoft Dynamics 365でのMarketo販売インサイトのインストールと構成
exl-id: c1f06b8c-48fd-4015-9502-7c9693632589
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 1%

---

# Microsoft Dynamics 365でのMarketo販売インサイトのインストールと構成{#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo・セールス・インサイトは、マーケティング・チームが持つ豊富なデータをセールス・チームに「窓口」として提供する素晴らしいツールです。 以下に、のインストールと設定方法を示します。

>[!PREREQUISITES]
>
>Marketoとマイクロソフトの統合を完了します。
>
>[お使いのバージョンのMicrosoft Dynamics CRMに適した](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) ソリューションをダウンロードしてください。

## ソリューションのインポート{#import-solution}

1. [Microsoft Office 365](https://login.microsoftonline.com/)にログインします。

   ![](assets/image2015-3-16-15-58-55.png)

1. ![—](assets/image2015-3-16-16-1-13.png)メニューをクリックし、**CRM**&#x200B;を選択します。

   ![](assets/image2015-3-16-16-0-10.png)

1. ![—](assets/image2015-5-13-10-5-8.png)メニューをクリックします。 ドロップダウンで、「**設定**」を選択し、「**ソリューション**」を選択します。

   ![](assets/image2015-5-13-10-4-1.png)

   >[!NOTE]
   >
   >先に進む前に、[をインストールし、Marketoソリューション](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-1-of-3-install.md)を設定しておく必要があります。

1. 「**インポート**」をクリックします。

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. 新しいウィンドウで、**参照**&#x200B;をクリックします。 手順1](#msi)でダウンロードした[Marketo販売インサイトソリューションを選択します。 「**次へ**」をクリックします。

   ![](assets/image2015-5-13-15-3a38-3a49.png)

1. ソリューションがアップロードされます。 必要に応じて、パッケージの内容を表示できます。 「**次へ**」をクリックします。

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. **チェック済み**&#x200B;のままにして、**読み込み**&#x200B;をクリックします。

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. ログファイルは自由にダウンロードできます。 「**閉じる**」をクリックします。

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. やりましたね！解決策を今すぐ見てみましょう。 表示されていない場合は、画面を更新します。

   ![](assets/image2015-5-13-15-3a42-3a29.png)

1. 「**すべてのカスタマイズを発行**」をクリックします。

   ![](assets/image2015-11-10-11-3a15-3a40.png)

## MarketoとSales Insightを接続{#connect-marketo-and-sales-insight}

MarketoインスタンスをDynamicsのSales Insightに結び付けます。 方法を次に示します。

>[!NOTE]
>
>**必要な管理者権限**

1. Marketoにログインし、**管理者**&#x200B;セクションに移動します。

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. 「**Sales Insight**」セクションで、「**Edit API Configuration**」をクリックします。

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. **Marketoホスト**、**API URL**、**APIユーザーID**&#x200B;をコピーして、後の手順で使用します。 任意の&#x200B;**API秘密キー**&#x200B;を入力し、「**保存**」をクリックします。

   >[!CAUTION]
   >
   >API秘密鍵にアンパサンド(&amp;)を使用しないでください。

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >Sales Insightを機能させるには、次のフィールドをMarketoと同期して、_リードと連絡先_&#x200B;の両方を行う必要があります。
   >
   > * 優先順位
   > * 緊急度
   > * 相対スコア

   >
   >これらのフィールドのいずれかが見つからない場合は、Marketoに、見つからないフィールドの名前のエラーメッセージが表示されます。 この問題を修正するには、[この手順](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md)を実行します。

1. Microsoft Dynamicsに戻り、「設定」の横の![](assets/image2015-5-13-15-3a49-3a19.png)アイコンをクリックし、ドロップダウンで&#x200B;**MarketoAPI Config**&#x200B;を選択します。

   ![](assets/image2015-5-13-16-3a4-3a1.png)

1. 「**デフォルト設定**」をクリックします。

   ![](assets/image2015-5-13-16-3a5-3a2.png)

1. 先ほどMarketoからコピーした情報を入力します。

   ![](assets/image2015-5-13-16-3a7-3a6.png)

1. 右下の![](assets/image2015-5-13-16-3a8-3a51.png)アイコンをクリックして、変更を保存します。

## ユーザーアクセスの設定{#set-user-access}

Sales Insightを使用する権限をユーザーに付与する必要があります。

1. ![](assets/image2015-5-13-10-3a5-3a8.png)メニューをクリックします。 ドロップダウンメニューで[**設定**]を選択し、[**セキュリティ**]を選択します。

   ![](assets/image2015-5-13-16-3a12-3a12.png)

1. 「**ユーザー**」をクリックします。

   ![](assets/image2015-4-29-14-3a57-3a46.png)

1. Sales Insightへのアクセス権を付与するユーザーを選択し、**ロールの管理**&#x200B;をクリックします。

   ![](assets/image2015-4-29-14-3a59-3a31.png)

1. **Marketo販売インサイト**&#x200B;のロールを選択し、「**OK**」をクリックします。

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   お前は全部終わらなきゃ！ 最後に、テストを行うには、Marketo販売インサイトにアクセスし、リードや連絡先を調べるユーザーとしてDynamicsにログインします。

   ![](assets/image2015-4-29-15-3a2-3a27.png)

これで、営業チームのMarketoセールス・インサイトの力を解除しました。

>[!MORELIKETHIS]
>
>[リード/接触レコードの星と炎の設定](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
