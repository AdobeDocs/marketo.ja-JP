---
unique-page-id: 3571737
description: Microsoft Dynamics 2013 - Marketto Docs — 製品ドキュメントで、Marketto Sales Insightのインストールと設定を行います
title: Microsoft Dynamics 2013でのMarketo Sales Insightのインストールと構成
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '444'
ht-degree: 0%

---


# Microsoft Dynamics 2013のMarketo Sales Insightのインストールと設定{#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insightは、マーケティングチームが持つ豊富なデータをセールスチームに「窓口」として提供する素晴らしいツールです。 以下に、インストールおよび設定の方法を示します。

>[!PREREQUISITES]
>
>[MarketoとMicrosoftの統合](http://docs.marketo.com/x/EIA2)を完了します。
>
>[お使いのバージョンのMicrosoft Dynamics CRMに適した](http://docs.marketo.com/x/LoJo) ソリューションをダウンロードしてください。

## ソリューションのインポート{#import-solution}

次に、Marketo Sales InsightソリューションをMicrosoft Dynamicsにインポートします。

1. **Microsoft Dynamics CRM**&#x200B;の下の&#x200B;**設定**&#x200B;をクリックします。

   ![](assets/image2014-12-12-9-3a4-3a56.png)

1. 「**設定**」で、「**カスタマイズ**」をクリックします。

   ![](assets/image2014-12-12-9-3a5-3a6.png)

1. 「**ソリューション**」をクリックします。

   ![](assets/image2014-12-12-9-3a5-3a17.png)

   >[!NOTE]
   >
   >**Reminder**
   >
   >
   >次に進む前に、Marketoを既にインストールし、設定しておく必要があります

1. 「**インポート**」をクリックします。

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. 新しいウィンドウで、**参照**&#x200B;をクリックします。

   ![](assets/image2014-12-12-9-3a5-3a36.png)

1. 上記でダウンロードしたソリューションを探して選択します。

   ![](assets/image2014-12-12-9-3a5-3a45.png)

1. 「**次へ**」をクリックします。

   ![](assets/image2014-12-12-9-3a5-3a55.png)

1. ソリューションがアップロードされます。 必要に応じて、パッケージの内容を表示できます。 「**次へ**」をクリックします。

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. チェックボックスをオンのままにして、「**読み込み**」をクリックします。

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. ログファイルは自由にダウンロードできます。 「**閉じる**」をクリックします。

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. すごい！ 解決策を今すぐ見てみましょう。 表示されていない場合は、画面を更新します。

   ![](assets/image2014-12-12-9-3a6-3a40.png)

## MarketoとSales Insightの接続{#connect-marketo-and-sales-insight}

MarketorのインスタンスをDynamicsのSales Insightに結び付けます。

>[!NOTE]
>
>管理者権限が必要です。

1. Marketoにログインし、**管理者**&#x200B;セクションに移動します。

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. 「**Sales Insight**」セクションで、「**Edit API Configuration**」をクリックします。

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. 後の手順で使用するために、**Marketo Host**、**API URL**&#x200B;および&#x200B;**APIユーザーID**&#x200B;をコピーします。 任意の&#x200B;**API秘密キー**&#x200B;を入力し、**「保存**」をクリックします。

   >[!CAUTION]
   >
   >API秘密鍵にアンパサンド(&amp;)を使用しないでください。

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >Sales Insightを機能させるには、次のフィールドをMarketoと&#x200B;*リードと連絡先*&#x200B;の両方で同期する必要があります。
   >
   >    
   >    
   >    * 優先度
   >    * 緊急度
   >    * 相対スコア

   >    
   >    
   >これらのフィールドのいずれかが見つからない場合は、Marketorに、見つからないフィールドの名前のエラーメッセージが表示されます。 この問題を修正するには、[この手順](../../../../product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md)を実行します。

1. Microsoft Dynamicsに戻り、**設定**&#x200B;に戻ります。

   ![](assets/image2014-12-12-9-3a7-3a25.png)

1. 「**設定**」で、「**Marketto API Config**」をクリックします。

   ![](assets/image2014-12-12-9-3a7-3a34.png)

1. 「**新規**」をクリックします。

   ![](assets/image2014-12-12-9-3a8-3a8.png)

1. 以前にMarketoから取得した情報を入力し、「**保存**」をクリックします。

   ![](assets/image2014-12-12-9-3a8-3a17.png)

## ユーザーアクセスの設定{#set-user-access}

最後に、特定のユーザーにMarketor Sales Insightへのアクセスを与えることができます。

1. **設定**&#x200B;に移動します。

   ![](assets/image2014-12-12-9-3a8-3a34.png)

1. 「**ユーザー**」をクリックします。

   ![](assets/image2014-12-12-9-3a8-3a42.png)

1. Sales Insightへのアクセス権を付与するユーザーを選択し、**ロールの管理**&#x200B;をクリックします。

   ![](assets/image2014-12-12-9-3a9-3a13.png)

1. **Marketto Sales Insight**&#x200B;ロールを選択し、「**OK**」をクリックします。

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   お前は全部終わらなきゃ！ 最後に、テストを行うには、Marketor Sales Insightにアクセスし、リードや連絡先を調べるユーザーとしてDynamicsにログインします。

   ![](assets/image2014-12-12-9-3a9-3a31.png)

これで、Marketo Sales Insightのセールスチームの機能がロック解除されました。

>[!NOTE]
>
>**関連記事**
>
>[リード/接触レコードの星と炎の設定](http://docs.marketo.com/x/BICMAg)

