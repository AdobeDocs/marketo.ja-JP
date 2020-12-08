---
unique-page-id: 3571739
description: Microsoft Dynamics 365 - Marketto Docs — 製品ドキュメントで、Marketto Sales Insightのインストールと設定を行います
title: Microsoft Dynamics 365でのMarketo Sales Insightのインストールと構成
translation-type: tm+mt
source-git-commit: dc20aede0894a09e6c0bcd3d1580859b5fecb5f1
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 0%

---


# Microsoft Dynamics 365でのMarketo Sales Insightのインストールと構成 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insightは、マーケティングチームが持つ豊富なデータをセールスチームに「窓口」として提供する素晴らしいツールです。 以下に、のインストールと設定方法を示します。

>[!NOTE]
>
>**前提条件**
>
>Marketoと [Microsoftの統合を完了します](http://docs.marketo.com/x/E4A2)。
>
>[お使いのバージョンのMicrosoft Dynamics CRMに適したソリューション](http://docs.marketo.com/x/LoJo) をダウンロードしてください。

## ソリューションのインポート {#import-solution}

1. [Microsoft Office 365にログインします](https://login.microsoftonline.com/)。

   ![](assets/image2015-3-16-15-58-55.png)

1. 「 ![— 」](assets/image2015-3-16-16-1-13.png) メニューをクリックし、「 **CRM**」を選択します。

   ![](assets/image2015-3-16-16-0-10.png)

1. 「 ![— 」](assets/image2015-5-13-10-5-8.png) メニューをクリックします。 ドロップダウンで、「 **設定**」を選択し、「 **ソリューション**」を選択します。

   ![](assets/image2015-5-13-10-4-1.png)

   >[!NOTE]
   >
   >**Reminder**
   >
   >
   >先に進む前に、Marketo Solution [を既にインストールして設定しておく必要があります](../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-1-of-3-install.md) 。

   「読み込み」をクリックします。
   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. 新しいウィンドウで、「 **参照**」をクリックします。 手順1でダウンロードした [Marketo Sales Insightソリューションを選択し](#msi)ます。 「 **次へ**」をクリックします。

   ![](assets/image2015-5-13-15-3a38-3a49.png)

1. ソリューションがアップロードされます。 必要に応じて、パッケージの内容を表示できます。 「 **次へ**」をクリックします。

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. ボックスを **チェックしたままにして** 、「 **読み込み**」をクリックします。

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. ログファイルは自由にダウンロードできます。 「 **閉じる**」をクリックします。

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. すごい！ 解決策を今すぐ見てみましょう。 表示されていない場合は、画面を更新します。

   ![](assets/image2015-5-13-15-3a42-3a29.png)

1. 「すべてのカスタマイズを **発行**」をクリックします。

   ![](assets/image2015-11-10-11-3a15-3a40.png)

## MarketorとSales Insightの接続 {#connect-marketo-and-sales-insight}

MarketorのインスタンスをDynamicsのSales Insightに結び付けます。 方法を次に示します。

>[!NOTE]
>
>**必要な管理者権限**

1. Marketorにログインし、「 **管理者** 」セクションに移動します。

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. 「 **Sales Insight** 」セクションで、「 **Edit API Configuration**」をクリックします。

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. 後の手順で使用するた **めに、**&#x200B;マーケティング先ホスト **、** API URL **、** APIユーザーIDをコピーします。 任意の **API秘密キーを入力し** 、「 **保存**」をクリックします。

   >[!CAUTION]
   >
   >API秘密鍵にアンパサンド(&amp;)を使用しないでください。

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >Sales Insightのリードと連絡先の ** 両方が機能するには、次のフィールドをMarketorと同期する必要があります。
   >
   > * 優先度
   > * 緊急度
   > * 相対スコア

   >
   >これらのフィールドのいずれかが見つからない場合は、Marketorに、見つからないフィールドの名前のエラーメッセージが表示されます。 これを修正するには、 [次の手順を実行します](../../../../product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md)。

1. Microsoft Dynamicsに戻り、「設定」の横の ![](assets/image2015-5-13-15-3a49-3a19.png) アイコンをクリックし、ドロップダウンで「 **Marketto API Config** 」を選択します。

   ![](assets/image2015-5-13-16-3a4-3a1.png)

1. 「 **デフォルト設定**」をクリックします。

   ![](assets/image2015-5-13-16-3a5-3a2.png)

1. 以前にMarketorからコピーした情報を入力します。

   ![](assets/image2015-5-13-16-3a7-3a6.png)

1. 右下隅の ![](assets/image2015-5-13-16-3a8-3a51.png) アイコンをクリックして、変更を保存します。

## ユーザーアクセスの設定 {#set-user-access}

Sales Insightを使用する権限をユーザーに付与する必要があります。

1. メニューをクリックし ![](assets/image2015-5-13-10-3a5-3a8.png) ます。 ドロップダウンメニューで[ **設定**]を選択し、[ **セキュリティ**]を選択します。

   ![](assets/image2015-5-13-16-3a12-3a12.png)

1. 「 **ユーザー**」をクリックします。

   ![](assets/image2015-4-29-14-3a57-3a46.png)

1. Sales Insightへのアクセス権を付与するユーザーを選択し、「 **Manage Roles**」をクリックします。

   ![](assets/image2015-4-29-14-3a59-3a31.png)

1. 「 **Marketo Sales Insight** 」ロールを選択し、「 **OK**」をクリックします。

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   お前は全部終わらなきゃ！ 最後に、テストを行うには、Marketor Sales Insightにアクセスし、リードや連絡先を調べるユーザーとしてDynamicsにログインします。

   ![](assets/image2015-4-29-15-3a2-3a27.png)

これで、Marketo Sales Insightのセールスチームの機能がロック解除されました。

>[!NOTE]
>
>**関連記事**
>
>[リード/接触レコードの星と炎の設定](http://docs.marketo.com/x/BICMAg)