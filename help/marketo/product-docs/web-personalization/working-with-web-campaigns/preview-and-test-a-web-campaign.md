---
unique-page-id: 10092925
description: Webキャンペーンのプレビューとテスト — Marketto Docs — 製品ドキュメント
title: Webキャンペーンのプレビューとテスト
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 0%

---


# Webキャンペーンのプレビューとテスト {#preview-and-test-a-web-campaign}

この記事では、Webキャンペーンーをプレビューする様々な方法と、Webサイト上でライブなサンドボックスセグメントを使用してWebーをテストする方法について説明します。

## 作成ページでのWebキャンペーンのプレビュー {#preview-a-web-campaign-on-the-creation-page}

1. [ **Web** キャンペーンに移動 ****]。

   ![](assets/image2016-8-18-15-3a59-3a35.png)

1. 「**新規Webキャンペーンを作成**** **」をクリックするか、既存のキャンペーンを編集するアイコンをクリックします。

   ![](assets/create-new-or-edit-web-campaign.png)

1. 「サイトのプレビュー」で、ページのURLを追加し、「 **プレビュー**」をクリックします。 新しいウィンドウ/タブが開き、キャンペーンプレビューが表示されます。

   ![](assets/three-1.png)

   >[!TIP]
   >
   >「 **共有** 」をクリックして、キャンペーンプレビューの固定URLを含む電子メールを開きます。

   >[!NOTE]
   >
   >また、キャンペーンのプレビューを最適に行うために、ブラウザープラグイン( [Chrome](https://chrome.google.com/webstore/detail/marketo-web-personalizati/ldiddonjplchallbngbccbfdfeldohkj) または [Firefox](http://docs.marketo.com/display/docs/assets/mwp-0.0.0.8.xpi))をインストールすることもできます。 以下の節を参照してください。

## プレビュープラグインを使用した作成ページでのWebキャンペーンの作成 {#preview-a-web-campaign-on-the-creation-page-using-the-browser-plug-in}

1. の手順1と2に従い `section above`ます。
1. ブラウザープラグインへのリンクをクリックします（この場合はChromeを使用します）。

   ![](assets/4-1.png)

1. 新しいウィンドウ/タブが開きます。 Chrome **を追加クリックします**。

   ![](assets/five.png)

1. 「 **追加拡張機能**」をクリックします。

   ![](assets/six.png)

1. Marketoに戻ります。 追加ページのURLを指定し、「 **プレビュー**」をクリックします。

   ![](assets/seven.png)

1. 新しいウィンドウ/タブが開き、デスクトップ、スマートフォン、タブレットでのキャンペーンの見え方をプレビューできます。

   ![](assets/campaign-preview.png)

## WebキャンペーンページでのWebキャンペーンのプレビュー {#preview-a-web-campaign-on-the-web-campaigns-page}

1. Webキャンペーンーのリストを確認する際は、キャンペーンーを選択し、 **プレビュー** アイコンをクリックします。

   ![](assets/web-campaigns-1-preview-hand.png)

   簡単！

## WebキャンペーンのWebサイトへのプレビュー {#preview-a-web-campaign-on-your-website}

サンドボックスセグメントとキャンペーンを作成します。

1. 「 **セグメント**」に移動。

   ![](assets/new-dropdown-segments-hand.jpg)

1. 「新規 **作成**」をクリックします。

   ![](assets/image2015-9-10-10-3a42-3a39.png)

1. セグメントに名前を付けます。
1. 「行動」で、「ページを含める」をキャンバスにドラッグします。 値追加*sandbox=1*。 「キャンペーンの保存と定義」をクリックします。

   ![](assets/segment.png)

1. Webキャンペーンを設定ページで、リストからターゲットセグメントを選択して、サンドボックスセグメントに変更します。

   ![](assets/set-web-campaign-target-segment.jpg)

1. キャンペーンのクリエイティブを完成させ、「 **起動**」をクリックします。\
   ![](assets/click-launch.jpg)

1. Webサイトにアクセスし、URLの末尾にURLパラメータ「?sandbox=1」を追加します。 例： [www.marketo.com?sandbox=1](http://www.marketo.com/?sandbox=1)
1. Webサイトに対するキャンペーンの反応を確認する。

>[!NOTE]
>
>キャンペーンは、訪問者セッション中に1回だけ反応します。 キャンペーンを再度表示するには、ブラウザーのCookieをクリアします。

>[!NOTE]
>
>リダイレクトキャンペーンはプレビューできません。 これらをテストする唯一の方法は、サンドボックスセグメントを使用することです(特定のページによるターゲット- *sandbox=redirect*)。

