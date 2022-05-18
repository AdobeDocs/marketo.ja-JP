---
unique-page-id: 4720810
description: Google でのパーソナライズリマーケティング — Marketo ドキュメント - 製品ドキュメント
title: Google でのパーソナライズリマーケティング
exl-id: cc733f43-161d-41e4-afdf-8b5217700810
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '298'
ht-degree: 100%

---

# Google でのパーソナライズリマーケティング {#personalized-remarketing-in-google}

パーソナライズリマーケティングを使用すると、RTP データと  Google Analytics の力と Google ディスプレイネットワークのリーチを利用した利用して、ユーザーと再びエンゲージできます。

>[!PREREQUISITES]
>
>* [ウェブパーソナライズデータによるリターゲティング](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)設定を完成します
>* [リマーケティングと Google Analytics のヘルプ](https://support.google.com/analytics/topic/2611283?hl=en&amp;ref_topic=3413645)ドキュメントを確認してください。


## Google でのリマーケティングオーディエンスの作成 {#creating-a-remarketing-audience-in-google}

1. Google Analytics にログインします。**管理者**／**アカウント**／**プロパティ**&#x200B;をクリックします。**オーディエンス定義**／**オーディエンス**&#x200B;をクリックします。

   ![](assets/remarketing-ga-screenshots.jpg)

1. 「**+新規オーディエンス**」をクリックします。

   ![](assets/image2015-1-15-17-3a26-3a40.png)

1. **リンク設定**：Google Adwords アカウントにリンクします。**オーディエンスを定義**：「**新規作成**」をクリックします。

   ![](assets/image2015-1-15-17-3a32-3a4.png)

1. Audience Builder で、「**シーケンス**」をクリックして、「カスタムディメンション」、「カスタム変数」、「イベント」の下で、「**RTP データを検索**」をクリックします。

>[!TIP]
>
>以下は、オーディエンスを構築するために Analytics で RTP データを見つける方法です。
>
>Google Analytics の場合：
>
>* カスタム変数：組織、業界
>* イベントカテゴリ：セグメント、Insightera-CTA、RTP-Remarketing
>* イベントラベル：セグメント名、キャンペーン名、セグメント化されたオーディエンス名

>
>Google Universal Analytics の場合：
>
>* カスタムディメンション：組織、業界、カテゴリ（Fortune 500、1000、グローバル 2000）、グループ（エンタープライズ、中小企業）、ABM リスト（アカウントリスト）
>* イベントカテゴリ：RTP-Segment、RTP-Campaign、RTP-Remarketing
>* イベントラベル：セグメント名、キャンペーン名、セグメント化されたオーディエンス名


**RTP セグメント化されたオーディエンスデータからのリマーケティングオーディエンスの例**

1. 「**シーケンス**」をクリックします。
1. **イベントラベル**&#x200B;を選択します。
1. **セグメント化されたオーディエンス名**&#x200B;を入力します（RTP で表示されるように）。
1. 「**適用**」をクリックします。

![](assets/image2015-2-10-14-3a51-3a43.png)

**RTP 業界データからのオーディエンスの例**

![](assets/image2015-1-15-17-3a36-3a5.png)

1. 「**シーケンス**」をクリックします。
1. 「**RTP-Industry**」を選択します。
1. **業界名**&#x200B;を入力します（例：金融サービス、教育…）。
1. 「**適用**」をクリックします。
1. **オーディエンス名**&#x200B;を入力します。「**保存**」をクリックします。

![](assets/image2015-1-15-18-3a29-3a16.png)

## Google Adwords でのリマーケティング広告キャンペーンの作成 {#create-a-remarketing-ad-campaign-in-google-adwords}

1. **Google Adwords**.にログインします。「**キャンペーン**」をクリックして、「**ネットワークのみを表示**」を選択します。

   ![](assets/image2015-1-15-18-3a31-3a58.png)

1. **キャンペーン名**&#x200B;を入力して、「**タイプリマーケティング**」を選択します。

   ![](assets/image2015-1-15-18-3a35-3a7.png)

1. **広告グループ名**&#x200B;を入力し、**拡張 CPC** を入力して、「**リマーケティングリスト**」を選択します。

   ![](assets/image2015-1-15-18-3a51-3a57.png)

1. 「保存」をクリックして続行します。
1. 画像またはテキスト広告を追加し、リマーケティングキャンペーンを開始します。

   ![](assets/image2015-1-15-18-3a47-3a21.png)

>[!MORELIKETHIS]
>
>* [ウェブパーソナライズデータによるリターゲティング](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* [Facebook でのパーソナライズリマーケティング](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)

