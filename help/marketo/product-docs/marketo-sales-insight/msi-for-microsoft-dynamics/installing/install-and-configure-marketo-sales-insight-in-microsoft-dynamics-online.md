---
unique-page-id: 37355602
description: Microsoft Dynamics Online - Marketto Docs — 製品ドキュメントで、Marketto Sales Insightのインストールと設定を行います。
title: Microsoft Dynamics OnlineでのMarketor Sales Insightのインストールと構成
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---


# Microsoft Dynamics OnlineでのMarketo Sales Insightのインストールと設定{#install-and-configure-marketo-sales-insight-in-microsoft-dynamics-online}

Marketo Sales Insightは、マーケティングチームが持つ豊富なデータをセールスチームに「窓口」として提供する素晴らしいツールです。 Microsoft Dynamics Onlineにインストールして構成する方法を次に示します。

>[!PREREQUISITES]
>
>[MarketoとMicrosoftの統合](http://docs.marketo.com/x/E4A2)を完了します。
>
>[お使いのバージョンのMicrosoft Dynamics CRMに適した](http://docs.marketo.com/x/LoJo) ソリューションをダウンロードしてください。

## ソリューションのインポート{#import-solution}

>[!NOTE]
>
>統合インターフェイスを使用している場合は、下の手順1より前に、右上隅の設定アイコンをクリックし、「**詳細設定**」を選択します。

1. Microsoft Dynamics CRMで、**設定**&#x200B;をクリックします。

   ![](assets/image2014-12-12-9-3a4-3a56-1.png)

1. 「設定」(SETTINGS)で、「**カスタマイズ**」をクリックします。

   ![](assets/image2015-4-29-14-3a22-3a1-1.png)

1. 「**ソリューション**」をクリックします。

   ![](assets/image2014-12-12-9-3a5-3a17-1.png)

   >[!NOTE]
   >
   >**Reminder**
   >
   >
   >先に進む前に、Marketoソリューションを既にインストールして設定しておく必要があります。

1. 「**インポート**」をクリックします。

   ![](assets/image2014-12-12-9-3a5-3a27-1.png)

1. 新しいウィンドウで、**参照**&#x200B;をクリックします。

   ![](assets/image2014-12-12-9-3a5-3a36-1.png)

1. ダウンロードしたソリューションをコンピューターで探し、インストールします。
1. 「**次へ**」をクリックします。

   ![](assets/seven.png)

1. ソリューションがアップロードされます。 必要に応じて、パッケージの内容を表示できます。 「**次へ**」をクリックします。

   ![](assets/image2014-12-12-9-3a6-3a10-1.png)

1. チェックボックスをオンのままにして、「**読み込み**」をクリックします。

   ![](assets/image2014-12-12-9-3a6-3a19-1.png)

1. ログファイルを自由にダウンロードして、**閉じる**&#x200B;をクリックします。

   ![](assets/image2014-12-12-9-3a6-3a29-1.png)

1. すごい！ 解決策を今すぐ見てみましょう。 表示されていない場合は、画面を更新します。

   ![](assets/eleven.png)

1. 「**パブリッシュのカスタマイズ**」をクリックします。

   >[!NOTE]
   >
   >グローバルMS Dynamicsの同期を有効にしてください。

## MarketoとSales Insightの接続{#connect-marketo-and-sales-insight}

MarketorのインスタンスをDynamicsのSales Insightに結び付けます。 その方法を次に示します。

>[!NOTE]
>
>**必要な管理者権限**

1. Marketingにログインし、「**Admin **」セクションに移動します。

   ![](assets/image2014-12-12-9-3a6-3a50-1.png)

1. 「Sales Insight」セクションで、「**Edit API Configuration**」をクリックします。

   ![](assets/image2014-12-12-9-3a7-3a0-1.png)

1. 後の手順で使用するために、**Marketo Host**、**API URL**&#x200B;および&#x200B;**APIユーザーID**&#x200B;をコピーします。 任意のAPI秘密鍵を入力し、「**保存**」をクリックします。

   >[!CAUTION]
   >
   >API秘密鍵にアンパサンド(&amp;)を使用しないでください。

   ![](assets/image2014-12-12-9-3a7-3a9-1.png)

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

   ![](assets/image2014-12-12-9-3a7-3a25-1.png)

1. 「**設定**」で、「**Marketto API Config**」をクリックします。

   ![](assets/image2014-12-12-9-3a7-3a34-1.png)

1. 「**新規**」をクリックします。

   ![](assets/image2014-12-12-9-3a8-3a8-1.png)

1. 以前にMarketoから取得した情報を入力し、「**保存**」をクリックします。

   ![](assets/image2014-12-12-9-3a8-3a17-1.png)

## 同期を有効にする{#enable-sync}

1. Marketoで、「**管理者**」をクリックします。

   ![](assets/enable-one.png)

1. [統合]で[**Microsoft Dynamics**]を選択します。

   ![](assets/enable-two.png)

1. 「**同期を有効にする**」をクリックします。

   ![](assets/enable-three.png)

1. 「フィールド同期の詳細」の横の「**編集**」をクリックします。

   ![](assets/enable-four.png)

1. これにより、以前無効にされたMSIフィールド（緊急性、相対スコア、優先度）が&#x200B;*自動的に*&#x200B;選択されます。 「**保存**」をクリックすると、開始同期データが表示されます。

   ![](assets/enable-five.png)

## ユーザーアクセスの設定{#set-user-access}

最後に、特定のユーザーに、Marketor Sales Insightの使用に対するアクセス権を与える必要があります。

1. **設定**&#x200B;に移動します。

   ![](assets/image2014-12-12-9-3a8-3a34-1.png)

1. **セキュリティ**&#x200B;に移動します。

   ![](assets/image2015-4-29-14-3a56-3a33-1.png)

1. 「**ユーザー**」をクリックします。

   ![](assets/image2015-4-29-14-3a57-3a46-1.png)

1. Sales Insightへのアクセスを許可するユーザーを選択し、**ロールの管理**&#x200B;をクリックします。

   ![](assets/image2015-4-29-14-3a59-3a31-1.png)

1. Marketo Sales Insightロールを選択し、「**OK**」をクリックします。

   ![](assets/image2014-12-12-9-3a9-3a22-1.png)

   お前は全部終わらなきゃ！ 最後に、テストを行うには、Marketor Sales Insightにアクセスし、リードや連絡先を調べるユーザーとしてDynamicsにログインします。

   ![](assets/image2015-4-29-15-3a2-3a27-1.png)

>[!NOTE]
>
>**関連記事**
>
>[リード/接触レコードの星と炎の設定](http://docs.marketo.com/x/BICMAg)

