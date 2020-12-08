---
unique-page-id: 2949158
description: RTPとGoogle Analyticsの統合 — Marketto Docs — 製品ドキュメント
title: RTPとGoogle Analyticsの統合
translation-type: tm+mt
source-git-commit: c8a77dc84c023e05fbb442f575269aac108ffb29
workflow-type: tm+mt
source-wordcount: '614'
ht-degree: 0%

---


# RTPとGoogle Analyticsの統合 {#integrate-rtp-with-google-analytics}

>[!NOTE]
>
>ユニバーサル分析がオペレーティング標準になり、Googleのすべてのプロパティがユニバーサル分析にアップグレードされました。
>
>この記事では、古いGoogle Standard Analyticsの使用方法を示しますが、ユニバーサル分析に切り替えることをお勧めします。
>
>analytics.jsトラッキングコードをまだ使用していない場合は [](https://developers.google.com/analytics/devguides/collection/analyticsjs/)、Googleでは、このコードを使用するようにサイトのタグを付け直すことを強くお勧めします。 以下は、Googleで廃止される予定です。
>
>* ga.js
>* urchin.js
>* WAP/サーバ側スニペット
>* YT/MO
>* カスタム変数
>* ユーザー定義変数

>
>
WebパーソナライゼーションとUniversal Analyticsの統合方法を参照して [ください。](integrate-rtp-with-google-universal-analytics.md)

## はじめに {#introduction}

Marketo Real-Time Personalization(RTP)からGoogle Analytics(GA)アカウントへの直接データフローを使用して、新しい角度からWeb解析を分析します。 組織、業界、RTPキャンペーンに従って、GAでのWeb訪問回数を測定します。 GAの業種やRTPセグメントのタイプ、様々なトラフィックソース（ソーシャル、有料、オーガニック）に従ったリードのパフォーマンスや生成方法、キャンペーンのクリックスルー率の分析、Webサイトに対するパーソナライズキャンペーンの影響の測定などの表示指標。 この機能を活用して、RTPアカウントから最大のメリットを得る

**RTPAudience Analytics**

統合を使用すると、GAアカウントに新しいディメンションが存在します。 RTPは、次の機能でダッシュボードを自動的に拡張します。

1. 組織と産業
1. RTPでのカスタマイズ済みセグメント
1. アカウントベースのマーケティングリスト

主なB2B見込み客に焦点を当てます。 対象とする業界やセグメント別にチャネルを分析する。

## チャネルレポート {#channel-report}

![](assets/image2014-11-28-16-3a39-3a28.png)

RTP B2Bダッシュボードは、垂直およびRTPセグメントに従った訪問者の分類を把握するのに役立ちます。 金融業界や様々なマーケティングキャンペーン（有料、オーガニック、ソーシャル）に応じて、訪問者のパフォーマンスを確認できます。 このダッシュボードでは、RTPセグメントのパフォーマンスの概要を詳細に説明し、ドリルダウンしてサイト訪問者の上位組織を表示します。

## 行動フロー {#behavioral-flow}

![](assets/image2014-11-28-16-3a40-3a43.png)

行動フローレポート（画像を参照）は、訪問者がページやイベント間を移動するパスを視覚化します。 この図の例は、金融セクターからのすべての訪問者のパスを示しています。 このレポートは、訪問者がサイトに関与し続けているコンテンツを特定するのに役立ちます。

## RTPパフォーマンス {#rtp-performance}

RTPキャンペーンを測定し、サイト全体の平均に関連付けます。 これらのキャンペーンがWebサイトの指標にどのような影響を与えているかを学び、このデータを使用して、適切なターゲットに対するパーソナライゼーションの取り組みに焦点を当てます。 カスタマイズしたレポートを生成して、パーソナライズキャンペーンのパフォーマンスをより深く理解します。

![](assets/image2014-11-28-16-3a47-3a0.png)

## Google AnalyticsでのRTPの設定 {#setting-up-rtp-with-google-analytics}

1. GAア追加カウントに対する読み取りと分析のユーザーとしての電子メール。 [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#0674727628616734466b67746d6372692865696b)詳しくは、 [ここを参照してください](https://support.google.com/analytics/answer/2884495?hl=en)。
1. RTPアカウント内。 「 **アカウント設定**」に移動します。

   ![](assets/image2014-11-28-16-3a54-3a40.png)

1. 「 **アカウント設定**」で、「 **ドメイン** 」および「 **Analytics」を選択します。**
1. 「**Google Analytics」をクリックします。**
1. 関連する **カスタム変数** / **** イベントをオンにして、RTPからのこのデータをGoogle Analyticsに追加します。
1. カスタム変数データを送信する **** スロット番号を入力します（デフォルトは1,2）。

![](assets/image2014-11-28-17-3a0-3a17.png)

「 **保存**」をクリックします。

>[!NOTE]
>
>セグメントデータをGAに送信するには、RTPプラットフォームの [Edit Segmentページ](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md) の下で、「Send **SendイベントtoGoogle Analyticson Segment Match**」チェックボックスを選択します。

## RTPデータを使用したGoogle Analyticsレポートの設定 {#setting-up-google-analytics-reports-with-rtp-data}

Google Analyticsでは、ダッシュボード、GAセグメント化、レポートを使用して、RTPデータを表示できます。

* [ダッシュボードは](https://support.google.com/analytics/answer/1068216?hl=en) 、Webサイトのパフォーマンスの概要を提供します。
* GAセグメントは、GAインターフェース内の訪問者をフィルタし、セグメントごとのトラフィックを表示することを目的としています。 セグメントの作成方法については、 [ここを参照してください](https://support.google.com/analytics/answer/3124493?hl=en)。
* 表示に [合わせた](https://support.google.com/analytics/answer/1033013?hl=en) カスタマイズレポートの作成、スケジュールされた電子メールの設定を行う。 「カスタマイズ」>「新しいカスタムレポート」の項を参照してください。
