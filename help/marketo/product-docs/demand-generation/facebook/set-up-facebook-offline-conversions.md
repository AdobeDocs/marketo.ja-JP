---
unique-page-id: 11383953
description: facebookオフラインコンバージョンのセットアップ —Marketoドキュメント — 製品ドキュメント
title: facebookオフラインコンバージョンの設定
exl-id: e1974943-8fc8-41f6-be7e-1b594de13db6
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 5%

---

# facebookオフラインコンバージョンのセットアップ{#set-up-facebook-offline-conversions}

リード広告を通じて作成された人のためにオフラインコンバージョンデータをFacebookに送信することで、広告チームは広告費用をこれまで以上に最適化できます。 設定方法を次に示します。

>[!PREREQUISITES]
>
>* [Facebookリード広告](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)を設定する必要があります。
>* [売上高サイクルモデル](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/understanding-revenue-models.md)に承認済みのモデルが必要です。


## 管理構成{#admin-configuration}

1. Marketo **管理者**&#x200B;に移動します。

   ![](assets/image2016-11-29-13-3a8-3a45.png)

1. **LaunchPoint**&#x200B;に移動し、前に作成したFacebookリード広告サービスを重複クリックします。

   >[!NOTE]
   >
   >それをまだ行っていない場合は、[Facebookリード広告の設定](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)を行ってから、ここに戻って来てください。

   ![](assets/image2016-11-29-13-3a10-3a43.png)

1. 必要に応じて、**表示名**&#x200B;を編集し、オフラインコンバージョンを含めます。 「**次へ**」をクリックします。

   ![](assets/image2016-11-29-13-3a12-3a19.png)

1. 「**オフライン変換を有効にする**」をオンにし、「**次へ**」をクリックします。

   ![](assets/image2016-11-29-13-3a13-3a32.png)

1. 「**次へ**」をクリックします。

   ![](assets/image2016-11-29-13-3a14-3a17.png)

1. 「**保存**」をクリックします。

   ![](assets/image2016-11-29-13-3a14-3a52.png)

   甘い！ facebookオフラインコンバージョンの有効化の途中です。 Revenue Cycle Modelerに移動して、ステージをマッピングします。

   ![](assets/image2016-11-29-13-3a16-3a55.png)

## Revenue Cycle Modeler Configuration {#revenue-cycle-modeler-configuration}

1. **Analytics**&#x200B;に移動します。

   ![](assets/image2016-11-29-13-3a29-3a23.png)

1. モデルを選択し、**ドラフトを編集**&#x200B;をクリックします。

   ![](assets/image2016-11-29-13-3a31-3a6.png)

   >[!NOTE]
   >
   >現在、売上高サイクル段階を次のようにマップできるFacebookのイベントは10人です。
   >
   >* 支払情報の追加
   >* カートに追加
   >* ウィッシュリストに追加
   >* 登録が完了しました
   >* チェックアウトが開始されました
   >* 担当者
   >* その他
   >* 購入
   >* 検索
   >* コンテンツビュー


1. マッピングするステージを選択し、**Facebookコンバージョン**&#x200B;ドロップダウンから、マッピング先のFacebookイベントを選択します。 この手順を繰り返して、RCMのすべてのステージをFacebookのオフラインコンバージョンステージにマッピングします。

   ![](assets/1-1.png)

1. マッピングが完了したら、モデルを閉じます。

   ![](assets/2.png)

1. モデルを承認すると、完了です。

   ![](assets/image2016-11-29-15-3a6-3a30.png)

   次に、リード広告のリードがマッピングしたステージに到達すると、レポートのためにFacebookにコンバージョンが送信されます。

   >[!CAUTION]
   >
   >facebookアカウントを確認し、すべての[広告が](https://www.facebook.com/business/url/?href=%2Fbusiness%2Fhelp%2Fwww%2F1776828022605281&amp;cmsid&amp;creative=link&amp;creative_detail=advertiser-help-center&amp;create_type&amp;destination_cms_id&amp;orig_http_referrer)Marketoオフラインコンバージョンイベントセットに関連付けられていることを確認してください。 そうでない場合、広告のアトリビューションは機能しない可能性があります。

   >[!NOTE]
   >
   >オフラインコンバージョンデータは、MarketoからFacebookに1日に数回送信されます。

>[!MORELIKETHIS]
>
>[facebookオフラインコンバージョンについて](/help/marketo/product-docs/demand-generation/facebook/understanding-facebook-offline-conversions.md)
