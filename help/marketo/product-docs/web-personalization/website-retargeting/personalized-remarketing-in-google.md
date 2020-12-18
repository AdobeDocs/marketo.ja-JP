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


# Googleでのパーソナライズされたリマーケティング{#personalized-remarketing-in-google}

Personalized Remarketingを使用すると、RTPデータを使用し、Google Display Networkの到達に応じてGoogle Analyticsの能力を活用して、ユーザーと再び関わりを持つことができます。

>[!PREREQUISITES]
>
>* [Webパーソナライゼーションデータ](retargeting-with-web-personalization-data.md)の構成を実行します。
>* [Google Analyticsとのリマーケティングのヘルプ](https://support.google.com/analytics/topic/2611283?hl=en&amp;ref_topic=3413645)ドキュメントを確認

>



## Googleでのリマーケティングオーディエンスの作成{#creating-a-remarketing-audience-in-google}

1. Google Analyticsにログインします。 **管理者**、**アカウント**、**プロパティ**&#x200B;の順にクリックします。 **オーディエンス定義**&#x200B;と&#x200B;**オーディエンス**&#x200B;をクリックします。

   ![](assets/remarketing-ga-screenshots.jpg)

1. 「**+新規オーディエンス**」をクリックします。

   ![](assets/image2015-1-15-17-3a26-3a40.png)

1. **リンクの設定**:Google Adwordsアカウントへのリンク
1. **オーディエンスの定義**:「新規 **作成**」をクリックします。

   ![](assets/image2015-1-15-17-3a32-3a4.png)

1. オーディエンスビルダーで、「カスタムDimension、カスタム変数、イベント」の下の「**シーケンス**」と「**RTPデータ**&#x200B;を検索します」をクリックします。

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

1. **シーケンス**&#x200B;をクリックします。
1. 「**イベントのラベル」を選択します。**
1. **セグメント化されたオーディエンスの名前**&#x200B;を入力します（RTPに表示される）。
1. 「**適用**」をクリックします。

![](assets/image2015-2-10-14-3a51-3a43.png)

**RTP Industry Dataからのオーディエンスの例**

![](assets/image2015-1-15-17-3a36-3a5.png)

1. 「**シーケンス**」をクリックします。
1. 「** RTP-Industry**」を選択します。
1. **業界名**&#x200B;を入力します(例： 金融サービス、教育機関…)
1. 「**適用**」をクリックします。
1. **オーディエンス名**&#x200B;を入力します。 「**保存**」をクリックします。

![](assets/image2015-1-15-18-3a29-3a16.png)

## Google Adwordsでのリマーケティング広告キャンペーンの作成{#create-a-remarketing-ad-campaign-in-google-adwords}

1. **Google Adwords**&#x200B;にログインします。 「**キャンペーン**」をクリックし、「**ネットワークのみを表示**」を選択します。

   ![](assets/image2015-1-15-18-3a31-3a58.png)

1. **キャンペーン名**&#x200B;を入力し、**再マーケティングを入力します。**

   ![](assets/image2015-1-15-18-3a35-3a7.png)

1. 「**広告グループ名を入力**」に&#x200B;**強化CPC**&#x200B;を入力&#x200B;**再マーケティングリスト**&#x200B;を選択します。

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

