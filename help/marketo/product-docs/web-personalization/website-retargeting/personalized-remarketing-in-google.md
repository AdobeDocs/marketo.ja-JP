---
unique-page-id: 4720810
description: Googleでのパーソナライズされたリマーケティング — Marketto Docs — 製品ドキュメント
title: Googleでのパーソナライズされたリマーケティング
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 0%

---


# Googleでのパーソナライズされたリマーケティング {#personalized-remarketing-in-google}

Personalized Remarketingを使用すると、RTPデータを使用し、Google Display Networkの到達に応じてGoogle Analyticsの能力を活用して、ユーザーと再び関わりを持つことができます。

>[!PREREQUISITES]
>
>* Webパーソナライゼーションデータ [の設定で再ターゲティングを完了します](retargeting-with-web-personalization-data.md) 。
>* Google Analyticsとの [リマーケティングの確認ヘルプ](https://support.google.com/analytics/topic/2611283?hl=en&amp;ref_topic=3413645) ・ドキュメント

>



## Googleでのリマーケティングオーディエンスの作成 {#creating-a-remarketing-audience-in-google}

1. Google Analyticsにログインします。 「 **管理者**」、「 **アカウント**」、「 **プロパティ**」の順にクリックします。 [ **オーディエンス定義** ]および[ **オーディエンス**]をクリックします。

   ![](assets/remarketing-ga-screenshots.jpg)

1. 「 **新規オーディエンス**」をクリックします。

   ![](assets/image2015-1-15-17-3a26-3a40.png)

1. **リンクの設定**:Google Adwordsアカウントへのリンク
1. **オーディエンスの定義**:「新規 **作成**」をクリックします。

   ![](assets/image2015-1-15-17-3a32-3a4.png)

1. オーディエンスビルダーで、「 **Sequences** 」をクリックし、「Custom Variables **」、「Custom Variables」、「イベント」の下の「RTP Data** 」を探します。

>[!TIP]
>
>AnalyticsでRTPデータを見つけてオーディエンスを構築する方法
>
>Google Analytics内：
>
>* カスタム変数：組織、業界
>* イベントカテゴリ:セグメント、Insightera-CTA、RTP-Remarketing
>* イベントラベル：セグメント名、キャンペーン名、セグメント化されたオーディエンス名

>
>
Google Universal Analytics:
>
>* カスタムDimension:組織、業界、カテゴリ(Fortune 500,1000、Global 2000)、グループ(Enterprise、SMB)、ABMリスト(固有のアカウントリスト)
>* イベントカテゴリ:RTPセグメント、RTPキャンペーンRTPリマーケティング
>* イベントラベル：セグメント名、キャンペーン名、セグメント化されたオーディエンス名

>



**RTPセグメント化オーディエンスデータからのリマーケティングオーディエンスの例**

1. 「 **シーケンス」をクリックします。**
1. 「 **イベントラベル」を選択します。**
1. セグメント化されたオーディエンス **（RTPに表示される）の** 名前を入力します。
1. 「 **適用**」をクリックします。

![](assets/image2015-2-10-14-3a51-3a43.png)

**RTP Industry Dataからのオーディエンスの例**

![](assets/image2015-1-15-17-3a36-3a5.png)

1. 「 **シーケンス**」をクリックします。
1. 「** RTP-Industry**」を選択します。
1. 業種 **名** ( 金融サービス、教育機関…)
1. 「 **適用**」をクリックします。
1. 「 **オーディエンス名**」を入力します。 「 **保存**」をクリックします。

![](assets/image2015-1-15-18-3a29-3a16.png)

## Google Adwordsでのリマーケティング広告キャンペーンの作成 {#create-a-remarketing-ad-campaign-in-google-adwords}

1. Google Adwords **にログインします**。 [ **キャンペーン**]をクリックし、[ネットワークのみ **を表示**]を選択します。

   ![](assets/image2015-1-15-18-3a31-3a58.png)

1. 「 **キャンペーン名**」を入力し、「 **タイプ」「リマーケティング」を選択します。**

   ![](assets/image2015-1-15-18-3a35-3a7.png)

1. 「 **広告グループ名」、** 「 **拡張CPC**」、「 **再マーケティングリスト**」の順に入力します。

   ![](assets/image2015-1-15-18-3a51-3a57.png)

1. 「保存」をクリックして続行します。
1. 画像またはテ追加キスト広告を作成し、リマーケティングキャンペーンを開始します。

   ![](assets/image2015-1-15-18-3a47-3a21.png)

>[!NOTE]
>
>**関連記事**
>
>* [Webパーソナライゼーションデータを使用した再ターゲティング](retargeting-with-web-personalization-data.md)
>* [Facebookでのパーソナライズされたリマーケティング](personalized-remarketing-in-facebook.md)

