---
unique-page-id: 4720810
description: Google でのパーソナライズリマーケティング — Marketo ドキュメント - 製品ドキュメント
title: Google でのパーソナライズリマーケティング
exl-id: cc733f43-161d-41e4-afdf-8b5217700810
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 100%

---

# Google でのパーソナライズリマーケティング {#personalized-remarketing-in-google}

パーソナライズリマーケティングを使用すると、RTP データと  Google Analytics の力と Google ディスプレイネットワークのリーチを利用した利用して、ユーザーと再びエンゲージできます。

>[!PREREQUISITES]
>
>* [ [!DNL Web Personalization]  データを使用したリターゲティング](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)の設定の完了
>* [リマーケティングと Google Analytics のヘルプ](https://support.google.com/analytics/topic/2611283?hl=en&ref_topic=3413645)ドキュメントを確認してください。

## Google でのリマーケティングオーディエンスの作成 {#creating-a-remarketing-audience-in-google}

1. Google Analytics にログインします。**[!UICONTROL 管理者]**／**[!UICONTROL アカウント]**／**[!UICONTROL プロパティ]**&#x200B;をクリックします。**[!UICONTROL オーディエンス定義]**／**[!UICONTROL オーディエンス]**&#x200B;をクリックします。

   ![](assets/remarketing-ga-screenshots.jpg)

1. 「**[!UICONTROL +新規オーディエンス]**」をクリックします。

   ![](assets/image2015-1-15-17-3a26-3a40.png)

1. **[!UICONTROL リンク設定]**：[!DNL Google Adwords] アカウントにリンクします。**[!UICONTROL オーディエンスを定義]**：「**[!UICONTROL 新規作成]**」をクリックします。

   ![](assets/image2015-1-15-17-3a32-3a4.png)

1. Audience Builder で、「**[!UICONTROL シーケンス]**」をクリックして、「**[!UICONTROL RTP データを検索]**」を「[!UICONTROL カスタムディメンション]」、「[!UICONTROL [!]UICONTROL カスタム変数]」、「[!UICONTROL イベント]」の下でクリックします。

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

1. 「**[!UICONTROL シーケンス]」をクリックします。**
1. 「**[!UICONTROL イベントラベル]」を選択します。**
1. **[!UICONTROL セグメント化されたオーディエンス名]**&#x200B;を入力します（RTP で表示されるように）。
1. 「**[!UICONTROL 適用]**」をクリックします。

![](assets/image2015-2-10-14-3a51-3a43.png)

**RTP 業界データからのオーディエンスの例**

![](assets/image2015-1-15-17-3a36-3a5.png)

1. 「**[!UICONTROL シーケンス]**」をクリックします。
1. 「**[!UICONTROL RTP-Industry]**」を選択します。
1. **業界名**&#x200B;を入力します（例：[!UICONTROL 金融サービス]、[!UICONTROL 教育]…）。
1. 「**[!UICONTROL 適用]**」をクリックします。
1. **[!UICONTROL オーディエンス名]**&#x200B;を入力します。「**[!UICONTROL 保存]**」をクリックします。

![](assets/image2015-1-15-18-3a29-3a16.png)

## [!DNL Google Adwords] でのリマーケティング広告キャンペーンの作成 {#create-a-remarketing-ad-campaign-in-google-adwords}

1. **[!DNL Google Adwords]** にログインします。「**[!UICONTROL キャンペーン]**」をクリックして、「**[!UICONTROL ネットワークのみを表示]**」を選択します。

   ![](assets/image2015-1-15-18-3a31-3a58.png)

1. **[!UICONTROL キャンペーン名]**&#x200B;を入力して、「**[!UICONTROL タイプリマーケティング]」を選択します。**

   ![](assets/image2015-1-15-18-3a35-3a7.png)

1. **[!UICONTROL 広告グループ名]を入力し、****[!UICONTROL 拡張 CPC]** を入力して、「**[!UICONTROL リマーケティングリスト]**」を選択します。

   ![](assets/image2015-1-15-18-3a51-3a57.png)

1. 「**[!UICONTROL 保存]**」をクリックして続行します。
1. 画像またはテキスト広告を追加し、リマーケティングキャンペーンを開始します。

   ![](assets/image2015-1-15-18-3a47-3a21.png)

>[!MORELIKETHIS]
>
>* [ [!DNL Web Personalization]  データを使用したリターゲティング](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* [ [!DNL Facebook]](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md) でのパーソナライズリマーケティング
