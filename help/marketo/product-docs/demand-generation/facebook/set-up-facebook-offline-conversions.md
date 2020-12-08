---
unique-page-id: 11383953
description: Facebookオフラインコンバージョンの設定 — Marketto Docs — 製品ドキュメント
title: Facebookオフラインコンバージョンの設定
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---


# Facebookオフラインコンバージョンの設定 {#set-up-facebook-offline-conversions}

リード広告を通じて作成された人のオフラインコンバージョンデータをFacebookに送り返すことで、広告チームは広告費用をこれまで以上に最適化できます。 設定方法を次に示します。

>[!NOTE]
>
>**前提条件**
>
>* Facebookのリード広告を [設定する必要があります](set-up-facebook-lead-ads.md)。
>* [売上高サイクルモデラーで承認済みのモデルが必要です](http://docs.marketo.com/display/docs/revenue+cycle+models)。

>



## 管理設定 {#admin-configuration}

1. 「マーケティング **管理者**」に移動します。

   ![](assets/image2016-11-29-13-3a8-3a45.png)

1. LaunchPointに移動し、 **重複クリックして** 、以前に作成したFacebookリード広告サービスを表示します。

   >[!NOTE]
   >
   >まだ設定していない場合は、「Facebookリード広告の [設定](set-up-facebook-lead-ads.md)」に進み、ここに戻ってください。

   ![](assets/image2016-11-29-13-3a10-3a43.png)

1. 必要に応じて、「 **表示名** 」を編集し、オフラインコンバージョンを含めます。 「 **次へ**」をクリックします。

   ![](assets/image2016-11-29-13-3a12-3a19.png)

1. 「オフラインコンバージョンを **有効にする** 」をオンにし、「 **次へ**」をクリックします。

   ![](assets/image2016-11-29-13-3a13-3a32.png)

1. 「 **次へ**」をクリックします。

   ![](assets/image2016-11-29-13-3a14-3a17.png)

1. 「 **保存**」をクリックします。

   ![](assets/image2016-11-29-13-3a14-3a52.png)

   甘い！ Facebookオフラインコンバージョンの有効化の途中です。 Revenue Cycle Modelerに移動して、ステージをマッピングします。

   ![](assets/image2016-11-29-13-3a16-3a55.png)

## 売上高サイクルモデラーの構成 {#revenue-cycle-modeler-configuration}

1. 「 **Analytics**」に移動します。

   ![](assets/image2016-11-29-13-3a29-3a23.png)

1. モデルを選択し、「ドラフトを **編集**」をクリックします。

   ![](assets/image2016-11-29-13-3a31-3a6.png)

   >[!NOTE]
   >
   >現在、売上高サイクルステージを次のようにマップできるFacebookイベントは10人です。
   >
   >    
   >    
   >    * 支払情報の追加
   >    * 買い物かごに追加
   >    * ウィッシュリストに追加
   >    * 登録完了
   >    * チェックアウト開始
   >    * 人
   >    * その他
   >    * 購入
   >    * 検索
   >    * コンテンツ表示


1. マッピングするステージを選択し、「 **Facebookコンバージョン** 」ドロップダウンから、マッピング先のFacebookイベントを選択します。 この手順を繰り返して、RCMのすべてのステージをFacebookのオフラインコンバージョンステージにマッピングします。

   ![](assets/1-1.png)

1. マッピングが完了したら、モデルを閉じます。

   ![](assets/2.png)

1. モデルを承認すると、完了です。

   ![](assets/image2016-11-29-15-3a6-3a30.png)

   現在は、リード広告のリードがマッピングしたステージに到達すると、レポートのためにFacebookにコンバージョンが送信されます。

   >[!CAUTION]
   >
   >Facebookアカウントを確認し、すべての [広告が「マーケティング先オフラインコンバージョン](https://www.facebook.com/business/url/?href=%2Fbusiness%2Fhelp%2Fwww%2F1776828022605281&amp;cmsid&amp;creative=link&amp;creative_detail=advertiser-help-center&amp;create_type&amp;destination_cms_id&amp;orig_http_referrer) 」イベントセットに関連付けられていることを確認します。 そうでない場合、広告のアトリビューションは機能しない可能性があります。

   >[!NOTE]
   >
   >オフラインコンバージョンデータは、MarketoからFacebookに1日に数回送信されます。

>[!NOTE]
>
>**関連記事**
>
>* [Facebookオフラインコンバージョンについて](understanding-facebook-offline-conversions.md)

>



