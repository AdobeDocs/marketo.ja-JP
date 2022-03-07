---
unique-page-id: 11383953
description: Facebook オフラインコンバージョンの設定 - Marketo ドキュメント - 製品ドキュメント
title: Facebook オフラインコンバージョンの設定
exl-id: e1974943-8fc8-41f6-be7e-1b594de13db6
source-git-commit: 41d8762203786bac9aea03ac978daa0549ac8e93
workflow-type: ht
source-wordcount: '331'
ht-degree: 100%

---

# Facebook オフラインコンバージョンの設定 {#set-up-facebook-offline-conversions}

リード広告を通じて作成されたユーザーのオフラインコンバージョンデータを Facebook に送り返すことで、広告チームは広告費用をこれまで以上に最適化できます。その設定方法を説明しましょう。

>[!PREREQUISITES]
>
>* [Facebook リード広告の統合を設定](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)する必要があります。
>* [収益サイクルモデラー](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/understanding-revenue-models.md)で承認済みのモデルが必要です。


## 管理設定 {#admin-configuration}

1. Marketo の「**管理**」に移動します。

   ![](assets/image2016-11-29-13-3a8-3a45.png)

1. **LaunchPoint** に移動して、前に作成した Facebook リード広告サービスをダブルクリックします。

   >[!NOTE]
   >
   >まだおこなっていない場合は、[続行する前に Facebook リード広告を設定](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)してください。

   ![](assets/image2016-11-29-13-3a10-3a43.png)

1. 必要に応じて、**表示名**&#x200B;を編集してオフラインコンバージョンを含めます。「**次へ**」をクリックします。

   ![](assets/image2016-11-29-13-3a12-3a19.png)

1. 「**オフラインコンバージョンを有効にする**」のチェックをオンにして、「**次へ**」をクリックします。

   ![](assets/image2016-11-29-13-3a13-3a32.png)

1. 「**次へ**」をクリックします。

   ![](assets/image2016-11-29-13-3a14-3a17.png)

1. 「**保存**」をクリックします。

   ![](assets/image2016-11-29-13-3a14-3a52.png)

   できましたね。Facebook オフラインコンバージョンの有効化が半分ほど完了しました。収益サイクルモデラーに移動して、ステージをマッピングします。

   ![](assets/image2016-11-29-13-3a16-3a55.png)

## 収益サイクルモデラーの設定 {#revenue-cycle-modeler-configuration}

1. **分析**&#x200B;に移動します。

   ![](assets/image2016-11-29-13-3a29-3a23.png)

1. モデルを選択して、「**ドラフトを編集**」をクリックします。

   ![](assets/image2016-11-29-13-3a31-3a6.png)

   >[!NOTE]
   >
   >現在、収益サイクルステージをマッピングできる Facebook イベントは 10 件あります。
   >
   >* 支払情報の追加
   >* カートに追加
   >* ウィッシュリストに追加
   >* 登録が完了しました
   >* チェックアウトが開始されました
   >* 顧客
   >* その他
   >* 購入
   >* 検索
   >* コンテンツビュー


1. マッピングするステージを選択し、**Facebook コンバージョン**&#x200B;ドロップダウンで、マッピング先の Facebook イベントを選択します。この手順を繰り返して、RCM のすべてのステージを Facebook のオフラインコンバージョンステージにマッピングします。

   ![](assets/1-1.png)

1. マッピングが完了したら、モデルを閉じます。

   ![](assets/2.png)

1. モデルを承認すれば完了です。

   ![](assets/image2016-11-29-15-3a6-3a30.png)

   これで、リード広告のリードがマッピングしたステージに到達すると、コンバージョンがレポート用に Facebook に送信されます。

   >[!CAUTION]
   >
   >Facebook アカウントで、Marketo オフラインコンバージョンイベントセットにすべての[広告が関連付けられている](https://www.facebook.com/business/url/?href=%2Fbusiness%2Fhelp%2Fwww%2F1776828022605281&amp;cmsid&amp;creative=link&amp;creative_detail=advertiser-help-center&amp;create_type&amp;destination_cms_id&amp;orig_http_referrer)ことを確認してください。そうでない場合、広告アトリビューションは機能しない可能性があります。

   >[!NOTE]
   >
   >オフラインコンバージョンデータは、Marketo から Facebook に 1 日に数回送信されます。

>[!MORELIKETHIS]
>
>[Facebook オフラインコンバージョンについて](/help/marketo/product-docs/demand-generation/facebook/understanding-facebook-offline-conversions.md)
