---
unique-page-id: 11383953
description: Facebook オフラインコンバージョンの設定 - Marketo ドキュメント - 製品ドキュメント
title: Facebook オフラインコンバージョンの設定
exl-id: e1974943-8fc8-41f6-be7e-1b594de13db6
feature: Integrations
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 50%

---

# [!DNL Facebook] オフラインコンバージョンの設定 {#set-up-facebook-offline-conversions}

リード広告を通じて作成された人物のオフラインコンバージョンデータを [!DNL Facebook] に送り返すことで、広告チームは広告費用をこれまで以上に最適化できます。 その設定方法を説明しましょう。

>[!PREREQUISITES]
>
>* [Facebook リード広告の統合を設定](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)する必要があります。
>* [収益サイクルモデラー](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/understanding-revenue-models.md)で承認済みのモデルが必要です。

## 管理設定 {#admin-configuration}

1. Marketo の「**[!UICONTROL 管理]**」に移動します。

   ![](assets/image2016-11-29-13-3a8-3a45.png)

1. **[!UICONTROL LaunchPoint]** に移動して、前に作成した Facebook リード広告サービスをダブルクリックします。

   >[!NOTE]
   >
   >まだ行っていない場合は、[Facebook リード広告の設定 [!UICONTROL  を行い、ここに戻っ ]](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md) ください。

   ![](assets/image2016-11-29-13-3a10-3a43.png)

1. 必要に応じて、**[!UICONTROL 表示名]**&#x200B;を編集してオフラインコンバージョンを含めます。「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/image2016-11-29-13-3a12-3a19.png)

1. 「**[!UICONTROL オフラインコンバージョンを有効にする]**」のチェックをオンにして、「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/image2016-11-29-13-3a13-3a32.png)

1. 「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/image2016-11-29-13-3a14-3a17.png)

1. 「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2016-11-29-13-3a14-3a52.png)

   できましたね。[!DNL Facebook] オフラインコンバージョンの有効化が半分完了しました。 収益サイクルモデラーに移動して、ステージをマッピングします。

   ![](assets/image2016-11-29-13-3a16-3a55.png)

## 収益サイクルモデラーの設定 {#revenue-cycle-modeler-configuration}

1. **[!UICONTROL 分析]**&#x200B;に移動します。

   ![](assets/image2016-11-29-13-3a29-3a23.png)

1. モデルを選択して、「**[!UICONTROL ドラフトを編集]**」をクリックします。

   ![](assets/image2016-11-29-13-3a31-3a6.png)

   >[!NOTE]
   >
   >現在、収益サイクルステージをマッピングできる [!DNL Facebook] イベントは 10 個あります。
   >
   >* 支払情報の追加
   >* 買い物かごに追加
   >* ウィッシュリストに追加
   >* 登録が完了しました
   >* チェックアウトが開始されました
   >* 顧客
   >* その他
   >* 購入
   >* 検索
   >* コンテンツビュー

1. マッピングするステージを選択し、「**[!UICONTROL Facebook コンバージョン]**」ドロップダウンからマッピングする [!DNL Facebook] イベントを選択します。 この手順を繰り返して、RCM のすべてのステージを [!DNL Facebook] のオフラインコンバージョンステージにマッピングします。

   ![](assets/1-1.png)

1. マッピングが完了したら、モデルを閉じます。

   ![](assets/2.png)

1. モデルを承認すれば完了です。

   ![](assets/image2016-11-29-15-3a6-3a30.png)

   リード広告リードがマッピングしたステージに到達すると、コンバージョンはレポート用に [!DNL Facebook] に送信されるようになりました。

   >[!CAUTION]
   >
   >[!DNL Facebook] アカウントを確認し、すべての [ 広告が関連付けられている ](https://www.facebook.com/business/url/?href=%2Fbusiness%2Fhelp%2Fwww%2F1776828022605281&cmsid&creative=link&creative_detail=advertiser-help-center&create_type&destination_cms_id&orig_http_referrer)Marketo オフラインコンバージョンイベントセットであることを確認します。 そうでない場合、広告アトリビューションは機能しない可能性があります。

   >[!NOTE]
   >
   >オフラインコンバージョンデータは、Marketoから [!DNL Facebook] に 1 日に数回送信されます。

>[!MORELIKETHIS]
>
>[ オフラインコンバージョン  [!DNL Facebook]  ついて ](/help/marketo/product-docs/demand-generation/facebook/understanding-facebook-offline-conversions.md)
