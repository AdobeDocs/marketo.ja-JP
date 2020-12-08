---
unique-page-id: 15695874
description: BrightTALKをMarkettoに接続 — Marketto Docs — 製品ドキュメント
title: BrightTALKをMarketoに接続
translation-type: tm+mt
source-git-commit: 23428a6e0ba9b2108a8f2f7dd6a69929dd069834
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---


# BrightTALKをMarketoに接続 {#connect-brighttalk-to-marketo}

BrightTALKチャネルをMarketoインスタンスに接続する方法を説明します。 これを行うには、両方の管理者である必要があります。

>[!NOTE]
>
>**必要な管理者権限**

## BrightTALKのステップ {#steps-in-brighttalk}

1. business.brighttalk.com/demandcentralにログインし、 [「今すぐ](http://business.brighttalk.com/demandcentral/login) 接続 ****」をクリックします。
1. 「Advanced Markettor Connector」で、「 **接続**」をクリックします。
1. 資格情報画面が開き、次の項目を確認します。クライアントID、クライアントシークレット、IDサービスURL、RESTサービスURL。 この情報を取得するには、Marketoにログインします。

## マーケティングの手順 {#steps-in-marketo}

>[!NOTE]
>
>この時点で、BrightTALKがMarketoインスタンスに与える権限を制限するために、APIのみのユーザーロールとAPIユーザーを設定する必要があります。 この手順の記事は既にあるので、リンクします。

1. [APIのみのユーザーロールの作成](http://docs.marketo.com/x/iwMk)。
1. [手順4で作成したBrightTALK APIロールを使用して](http://docs.marketo.com/x/jwMk)、APIユーザーを作成します。
1. 管理領域に戻ります。

   ![](assets/one.png)

1. 「統合」で、「 **LaunchPoint**」をクリックします。

   ![](assets/two.png)

1. 「 **New** 」ドロップダウンをクリックし、「 **New Service**」を選択します。

   ![](assets/three.png)

1. 任意の表示名を入力します。 「サービス」ドロップダウンをクリックし、「 **Custom** 」を選択します(「BrightTALK」は選択 **しないでください** )。

   ![](assets/four.png)

   >[!CAUTION]
   >
   >ドロップダウンでBrightTALKを選択しないでください。 これは、削除中のフィールドです。選択すると、Marketto/BrightTALK統合に重大な問題が発生する可能性があります。

1. 選択した説明を入力します。 「APIのみのユーザー」ドロップダウンをクリックし、手順5で作成したBrightTALK APIユーザーを選択します。 「 **作成**」をクリックします。

   ![](assets/five.png)

1. 先ほど作成したカスタムサービスの「 **表示の詳細** 」をクリックします。

   ![](assets/six.png)

1. クライアントID **と** クライアントシークレットをコピー（および保存）します ****。 「 **閉じる**」をクリックします。

   ![](assets/eight-1.png)

1. 「統合」で、「 **Webサービス**」を選択します。

   ![](assets/nine-1.png)

1. Rest APIの下で、 **エンドポイント** と **IDをコピー（および保存）します**。

   ![](assets/ten.png)

## BrightTALKのステップ {#steps-in-brighttalk-1}

1. 手順3からBrightTALKコネクタの設定画面に戻り、手順12と14で保存した資格情報を入力します。

   秘密鍵証明書が認証されると、BrightTALKがMarketoに正式に接続されます。 次の手順は、同期 [するデータフィールドを決定することです](http://support.brighttalk.com/hc/en-us/articles/115005131274-BrightTALK-Connector-for-Marketo-Choose-the-Fields-to-Sync)。

