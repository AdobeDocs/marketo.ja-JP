---
unique-page-id: 4720810
description: Googleのパーソナライズされたリマーケティングなど、Marketo EngageのGoogleのパーソナライズされたリマーケティングについて説明します。 このガイドを使用して、次のステップを完了してください。
title: Google でのパーソナライズされたリマーケティング
exl-id: cc733f43-161d-41e4-afdf-8b5217700810
feature: Web Personalization
TQID: 'https://experienceleague.adobe.com/qAvf6tO5v6j29k3wWf3irTqhwv6EDq0eHzijvOjGXls'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
    internal-label: Configuration
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
    internal-label: Personalization
  - id: 664d862c-1673-5ed4-a3d6-386ac83225e4
    internal-label: Web Personalization
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
    internal-label: Personalization
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 86%
---
# Google でのパーソナライズされたリマーケティング {#personalized-remarketing-in-google}

パーソナライズされたリマーケティングを使用すると、RTP データと Google Analytics の機能、そして Google ディスプレイネットワークのリーチを活用して、ユーザと再びエンゲージできます。

>[!PREREQUISITES]
>
>* [&#x200B; [!DNL Web Personalization]  データを使用したリターゲティング](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)の設定の完了
>* [リマーケティングと Google Analytics のヘルプ](https://support.google.com/analytics/topic/2611283?hl=en&ref_topic=3413645)ドキュメントを確認してください。

## Google でのリマーケティングオーディエンスの作成 {#creating-a-remarketing-audience-in-google}

1. Google Analytics にログインします。 **[!UICONTROL 管理者]**／**[!UICONTROL アカウント]**／**[!UICONTROL プロパティ]**&#x200B;をクリックします。 **[!UICONTROL オーディエンス定義]**／**[!UICONTROL オーディエンス]**&#x200B;をクリックします。

   ![](assets/remarketing-ga-screenshots.jpg)

1. 「**[!UICONTROL +新規オーディエンス]**」をクリックします。

   ![](assets/image2015-1-15-17-3a26-3a40.png)

1. **[!UICONTROL リンク設定]**：[!DNL Google Adwords] アカウントにリンクします。 **[!UICONTROL オーディエンスを定義]**：「**[!UICONTROL 新規作成]**」をクリックします。

   ![](assets/image2015-1-15-17-3a32-3a4.png)

1. オーディエンスビルダーで、[!UICONTROL &#x200B; カスタムディメンション &#x200B;]、[!UICONTROL UICONTROL [ !] カスタム変数]、[!UICONTROL &#x200B; イベント &#x200B;]の下の&#x200B;**[!UICONTROL シーケンス]**&#x200B;と&#x200B;**[!UICONTROL RTP データ]**&#x200B;をクリックします。

>[!TIP]
>
>Analytics で RTP データを見つけてオーディエンスを作成するにはどうすればよいですか。
>
>Google Analytics の場合：
>
>* カスタム変数：組織、業界
>* イベントカテゴリ：セグメント、Insightera-CTA、RTP-Remarketing
>* イベントラベル：セグメント名、キャンペーン名、セグメント化されたオーディエンス名
>
>Google Universal Analytics の場合：
>
>* カスタムディメンション：組織、業界、カテゴリ（Fortune 500、1000、グローバル 2000）、グループ（エンタープライズ、中小企業）、ABM リスト（重点アカウントリスト）
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
1. **業界名**&#x200B;を入力します（例： [!UICONTROL 金融サービス]、[!UICONTROL 教育]…）。
1. 「**[!UICONTROL 適用]**」をクリックします。
1. **[!UICONTROL オーディエンス名]**&#x200B;を入力します。 「**[!UICONTROL 保存]**」をクリックします。

![](assets/image2015-1-15-18-3a29-3a16.png)

## [!DNL Google Adwords] でのリマーケティング広告キャンペーンの作成 {#create-a-remarketing-ad-campaign-in-google-adwords}

1. **[!DNL Google Adwords]** にログインします。 「**[!UICONTROL キャンペーン]**」をクリックして、「**[!UICONTROL ネットワークのみを表示]**」を選択します。

   ![](assets/image2015-1-15-18-3a31-3a58.png)

1. **[!UICONTROL キャンペーン名]**&#x200B;を入力して、「**[!UICONTROL タイプリマーケティング]」を選択します。**

   ![](assets/image2015-1-15-18-3a35-3a7.png)

1. **[!UICONTROL 広告グループ名]を入力し、**&#x200B;**[!UICONTROL 拡張 CPC]** を入力して、「**[!UICONTROL リマーケティングリスト]**」を選択します。

   ![](assets/image2015-1-15-18-3a51-3a57.png)

1. 「**[!UICONTROL 保存]**」をクリックして続行します。
1. 画像またはテキスト広告を追加し、リマーケティングキャンペーンを開始します。

   ![](assets/image2015-1-15-18-3a47-3a21.png)

>[!MORELIKETHIS]
>
>* [&#x200B; [!DNL Web Personalization]  データを使用したリターゲティング](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* [&#x200B; [!DNL Facebook]](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md) でのパーソナライズリマーケティング
