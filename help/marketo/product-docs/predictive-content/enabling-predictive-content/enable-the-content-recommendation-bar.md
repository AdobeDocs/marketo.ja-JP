---
unique-page-id: 4720108
description: コンテンツレコメンデーションバー —Marketoドキュメント — 製品ドキュメントを有効にする
title: コンテンツレコメンデーションバーの有効化
exl-id: f2244db1-51a9-4e26-9bf7-b2c79df25552
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---

# コンテンツレコメンデーションバーを有効にする{#enable-the-content-recommendation-bar}

コンテンツの推奨エンジンでは、予測分析と機械学習アルゴリズムを使用して、関連するコンテンツを各Web訪問者に配信します。 レコメンデーションエンジンは、訪問者ごとにどのコンテンツが最も高いパフォーマンスを発揮するかを予測します。 エンジンのコンテンツはRecommendationsのページで監視および制御され、コンテンツのROIの最適化に役立ちます。

>[!PREREQUISITES]
>
>予測コンテンツを有効にする前に、次の操作を行う必要があります。
>
>* **予測コンテンツの準備**
   >
   >   
   * [電子メールの予測コンテンツの](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-emails.md) 編集
   >   * [リッチ](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-rich-media.md) メディアの予測コンテンツの編集
   >   * [レコメンデーションバーの予測コンテンツの編集](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-the-recommendation-bar.md)
>
>* [予測コンテンツのタイトルの承認](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md)


## コンテンツレコメンデーションバーの有効化とカスタマイズ{#enable-and-customize-the-content-recommendation-bar}

1. 「**コンテンツ設定**」に移動します。

   ![](assets/settings-dropdown-hand.png)

1. **棒グラフ**&#x200B;をクリックします。

   ![](assets/content-settings-bar-hand.png)

1. レコメンデーションバーでURLを表示するには、「**オン**」をクリックし、「**保存**」をクリックします。

   ![](assets/bar-enable.png)

1. URLをカスタマイズするには、色、スタイル、書式、レコメンデーションバーの矢印、およびバーを含める/除外するページを選択します。 Webサイトのブランディングに合わせてカスタマイズします。 「**保存**」をクリックします。

   ![](assets/bar-customize-details-hands.png)

   >[!NOTE]
   >
   >**表示URLを含む/除外**
   >
   >* 表示URLはドメインのパスである必要があります
   >* https://またはhttps://を含めない
   >* ワイルドカードには*を使用
   * セミコロンを区切り文字として使用する
   * 例：/contact_us*;*action=logout*
   * このフィールドでは大文字と小文字が区別されます


## レコメンデーションバーの考慮事項{#recommendation-bar-considerations}

* レコメンデーションエンジンを動作させるには、Recommendationsページで&#x200B;****&#x200B;に設定されたレコメンデーションバーに少なくとも1つのコンテンツが必要です。 有効なコンテンツがなく、バーが&#x200B;**On**&#x200B;に設定されている場合、矢印エフェクトはWebページの右下に表示されますが、推奨コンテンツは表示されません。

* レコメンデーションエンジンで実行するコンテンツが多いほど、アルゴリズムでテストし、どのコンテンツが最も効果が高いかを判断するのに適しています。 10 ～ 20個のコンテンツ要素を実行し、アクティブにして、新しい要素を追加し続けることをお勧めします。
* レコメンデーション用に有効にするコンテンツ部分には、RTP Javascriptタグを含める必要があります。 これは、アルゴリズムによる推奨コンテンツの追跡と最適化に役立ちます。

>[!MORELIKETHIS]
[Webリッチメディアの予測コンテンツを有効にする](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)
