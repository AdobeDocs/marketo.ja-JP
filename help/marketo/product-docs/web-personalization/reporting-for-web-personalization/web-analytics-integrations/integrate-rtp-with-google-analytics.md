---
unique-page-id: 2949158
description: RTP を Google Analytics に連携する — Marketo ドキュメント — 製品ドキュメント
title: RTP を Google Analytics に連携する
exl-id: a2bc0c17-dc23-435e-9480-857e97e6fd50
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '608'
ht-degree: 100%

---

# RTP を Google Analytics に連携する {#integrate-rtp-with-google-analytics}

>[!NOTE]
>
>ユニバーサルアナリティクスが操作の標準になり、Google のすべてのプロパティがユニバーサルアナリティクスにアップグレードされました。
>
>この記事では、古い Google スタンダードアナリティクスの使用方法について説明しますが、ユニバーサルアナリティクスに切り替えることをお勧めします。
>
>[analytics.js トラッキングコード](https://developers.google.com/analytics/devguides/collection/analyticsjs/)をまだ使用していない場合は、サイトを再タグ付けして使用することを強くお勧めします。Google では、次の機能が廃止されています。
>
>* ga.js
>* urchin.js
>* WAP／サーバーサイドスニペット
>* YT／MO
>* カスタム変数
>* ユーザー定義変数
>
>[Web パーソナライゼーションをユニバーサル分析と連携する方法](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)を参照してください。

## はじめに {#introduction}

Marketo Real-Time Personalization（RTP）から Google Analytics（GA）アカウントへの直接データフローを使用して、新しい角度から Web 分析をおこないます。組織、業種、RTP キャンペーンに従って、GA での Web 訪問を測定します。GA で業種や RTP セグメントのタイプなどの指標と効果を表示し、様々なトラフィックソース（ソーシャル、有料、オーガニック）に従ってリードを生成し、キャンペーンのクリックスルー率を分析し、パーソナリゼ―ションキャンペーンが Web サイトに与える影響を測定します。この機能を活用して、RTP アカウントから最大限のメリットを得ます。

**RTP Audience Analytics**

統合により、GA アカウントに新しいディメンションが追加されます。RTP は、次の機能を使用してダッシュボードを自動的に強化します。

1. 組織と業種
1. RTP でカスタマイズされたセグメント
1. アカウントベースのマーケティングリスト

主な B2B 見込み客に焦点を当てます。ターゲットとする業種およびセグメント別にチャネルを分析します。

## チャネルレポート {#channel-report}

![](assets/image2014-11-28-16-3a39-3a28.png)

RTP B2B ダッシュボードは、垂直および RTP セグメントに従った訪問者の分類を理解するのに役立ちます。訪問者のパフォーマンスは、金融業界や様々なマーケティングキャンペーン（有料、オーガニック、ソーシャル）に応じて確認できます。また、ダッシュボードには、RTP セグメントのパフォーマンスの概要と、サイトを訪問した上位の組織を表示するドリルダウンの概要も表示されます

## ビヘイビアーフロー {#behavioral-flow}

![](assets/image2014-11-28-16-3a40-3a43.png)

ビヘイビアーフローレポート（画像を参照）は、訪問者がページまたはイベント間を移動するパスを視覚化します。画像の例では、金融部門のすべての訪問者のパスを示しています。このレポートは、訪問者がサイトに関与し続ける理由となるコンテンツを見つけるのに役立ちます。

## RTP パフォーマンス {#rtp-performance}

RTP キャンペーンを測定し、サイト全体の平均値と関連付けます。これらのキャンペーンが Web サイトの指標に与える影響を知り、このデータを使用して、適切なターゲットにパーソナライゼーションの取り組みを集中させます。パーソナライゼーションキャンペーンのパフォーマンスをより深く理解できるように、カスタマイズされたレポートを生成します。

![](assets/image2014-11-28-16-3a47-3a0.png)

## RTP と Google Analytics の設定 {#setting-up-rtp-with-google-analytics}

1. GA アカウントにメール rtp.ga2@gmail.com を読み取りおよび分析ユーザーとして追加します。詳細は[こちら](https://support.google.com/analytics/answer/2884495?hl=ja)をご覧ください。

1. RTP アカウント内で次の手順を実行します。「**アカウント設定**」に移動します。

   ![](assets/image2014-11-28-16-3a54-3a40.png)

1. 「**アカウント設定**」、「**ドメイン**」、「**Analytics**」で、

1. 「**Google Analytics**」をクリックします。

1. 該当する「**カスタム変数**」と「**イベント**」をオンにして、このデータを RTP から Google Analytics に追加します。

1. **スロット**&#x200B;番号を入力して、カスタム変数データを送信します（デフォルトは 1,2）。

![](assets/image2014-11-28-17-3a0-3a17.png)

1. 「**保存**」をクリックします。

>[!NOTE]
>
>セグメントデータを GA に送信するには、RTP プラットフォームの[セグメント編集ページ](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md)で、「**セグメント一致で Google Analytics にイベントを送信する**」チェックボックスをオンにします。

## Google Analytics レポートと RTP データの設定 {#setting-up-google-analytics-reports-with-rtp-data}

Google Analytics では、ダッシュボード、GA セグメント化およびレポートを使用して、RTP データを表示できます。

* [](https://support.google.com/analytics/answer/1068216?hl=ja) ダッシュボードでは、Web サイトのパフォーマンスの概要を示します。
* GA セグメントは、GA インターフェイス内の訪問者をフィルターし、セグメントごとのトラフィックを表示することを目的としています。セグメントの作成方法については、[こちら](https://support.google.com/analytics/answer/3124493?hl=ja)を参照してください。
* [カスタマイズされたレポート](https://support.google.com/analytics/answer/1033013?hl=ja)を作成してスケジュールされたメールを表示／設定する「カスタマイズ／新しいカスタムレポート」の下を確認します。
