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


# Microsoft Dynamics OnlineでのMarketor Sales Insightのインストールと構成 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics-online}

Marketo Sales Insightは、マーケティングチームが持つ豊富なデータをセールスチームに「窓口」として提供する素晴らしいツールです。 Microsoft Dynamics Onlineにインストールして構成する方法を次に示します。

>[!PREREQUISITES]
>
>Marketoと [Microsoftの統合を完了します](http://docs.marketo.com/x/E4A2)。
>
>[お使いのバージョンのMicrosoft Dynamics CRMに適したソリューション](http://docs.marketo.com/x/LoJo) をダウンロードしてください。

## ソリューションのインポート {#import-solution}

>[!NOTE]
>
>統合インターフェイスを使用している場合は、下の手順1より前に、右上隅の設定アイコンをクリックし、「 **詳細設定**」を選択します。

1. Microsoft Dynamics CRMで、「 **設定**」をクリックします。

   ![](assets/image2014-12-12-9-3a4-3a56-1.png)

1. [設定]で、[ **カスタマイズ**]をクリックします。

   ![](assets/image2015-4-29-14-3a22-3a1-1.png)

1. 「 **ソリューション**」をクリックします。

   ![](assets/image2014-12-12-9-3a5-3a17-1.png)

   >[!NOTE]
   >
   >**Reminder**
   >
   >
   >先に進む前に、Marketoソリューションを既にインストールして設定しておく必要があります。

1. 「 **読み込み**」をクリックします。

   ![](assets/image2014-12-12-9-3a5-3a27-1.png)

1. 新しいウィンドウで、「 **参照**」をクリックします。

   ![](assets/image2014-12-12-9-3a5-3a36-1.png)

1. ダウンロードしたソリューションをコンピューターで探し、インストールします。
1. 「 **次へ**」をクリックします。

   ![](assets/seven.png)

1. ソリューションがアップロードされます。 必要に応じて、パッケージの内容を表示できます。 「 **次へ**」をクリックします。

   ![](assets/image2014-12-12-9-3a6-3a10-1.png)

1. チェックボックスをオンのままにして、「 **読み込み**」をクリックします。

   ![](assets/image2014-12-12-9-3a6-3a19-1.png)

1. ログファイルを自由にダウンロードして、「 **閉じる**」をクリックします。

   ![](assets/image2014-12-12-9-3a6-3a29-1.png)

1. すごい！ 解決策を今すぐ見てみましょう。 表示されていない場合は、画面を更新します。

   ![](assets/eleven.png)

1. 「 **公開のカスタマイズ**」をクリックします。

   >[!NOTE]
   >
   >グローバルMS Dynamicsの同期を有効にしてください。

## MarketorとSales Insightの接続 {#connect-marketo-and-sales-insight}

MarketorのインスタンスをDynamicsのSales Insightに結び付けます。 その方法を次に示します。

>[!NOTE]
>
>**必要な管理者権限**

1. Marketingにログインし、「**Admin **」セクションに移動します。

   ![](assets/image2014-12-12-9-3a6-3a50-1.png)

1. 「Sales Insight」セクションで、「 **Edit API Configuration**」をクリックします。

   ![](assets/image2014-12-12-9-3a7-3a0-1.png)

1. 後の手順で使用するた **めに、** Marketo Host **、** API URL **、** API User Idをコピーします。 任意のAPI秘密キーを入力し、「 **保存**」をクリックします。

   >[!CAUTION]
   >
   >API秘密鍵にアンパサンド(&amp;)を使用しないでください。

   ![](assets/image2014-12-12-9-3a7-3a9-1.png)

   >[!NOTE]
   >
   >Sales Insightのリードと連絡先の ** 両方が機能するには、次のフィールドをMarketorと同期する必要があります。
   >
   >    
   >    
   >    * 優先度
   >    * 緊急度
   >    * 相対スコア

   >    
   >    
   >これらのフィールドのいずれかが見つからない場合は、Marketorに、見つからないフィールドの名前のエラーメッセージが表示されます。 これを修正するには、 [次の手順を実行します](../../../../product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md)。

1. Microsoft Dynamicsに戻り、「 **設定**」に移動します。

   ![](assets/image2014-12-12-9-3a7-3a25-1.png)

1. 「 **設定**」で、「 **Marketto API Config**」をクリックします。

   ![](assets/image2014-12-12-9-3a7-3a34-1.png)

1. 「 **新規**」をクリックします。

   ![](assets/image2014-12-12-9-3a8-3a8-1.png)

1. 以前にMarketorから取得した情報を入力し、「 **保存**」をクリックします。

   ![](assets/image2014-12-12-9-3a8-3a17-1.png)

## 同期を有効にする {#enable-sync}

1. Marketorで、「 **管理者**」をクリックします。

   ![](assets/enable-one.png)

1. 「統合」で、「 **Microsoft Dynamics**」を選択します。

   ![](assets/enable-two.png)

1. 「同期を **有効にする**」をクリックします。

   ![](assets/enable-three.png)

1. 「フィールドの同期の詳細」の **横にある「編集** 」をクリックします。

   ![](assets/enable-four.png)

1. これは *自動的に* 、以前無効にされたMSIフィールド（緊急度、相対スコア、優先度）を選択します。 「 **Save** to開始syncing data」をクリックするだけで済みます。

   ![](assets/enable-five.png)

## ユーザーアクセスの設定 {#set-user-access}

最後に、特定のユーザーに、Marketor Sales Insightの使用に対するアクセス権を与える必要があります。

1. 「 **設定**」に移動します。

   ![](assets/image2014-12-12-9-3a8-3a34-1.png)

1. 「 **セキュリティ**」に移動します。

   ![](assets/image2015-4-29-14-3a56-3a33-1.png)

1. 「 **ユーザー**」をクリックします。

   ![](assets/image2015-4-29-14-3a57-3a46-1.png)

1. Sales Insightへのアクセス権を付与するユーザーを選択し、「ロールの **管理**」をクリックします。

   ![](assets/image2015-4-29-14-3a59-3a31-1.png)

1. Marketo Sales Insightロールを選択し、「 **OK**」をクリックします。

   ![](assets/image2014-12-12-9-3a9-3a22-1.png)

   お前は全部終わらなきゃ！ 最後に、テストを行うには、Marketor Sales Insightにアクセスし、リードや連絡先を調べるユーザーとしてDynamicsにログインします。

   ![](assets/image2015-4-29-15-3a2-3a27-1.png)

>[!NOTE]
>
>**関連記事**
>
>[リード/接触レコードの星と炎の設定](http://docs.marketo.com/x/BICMAg)

