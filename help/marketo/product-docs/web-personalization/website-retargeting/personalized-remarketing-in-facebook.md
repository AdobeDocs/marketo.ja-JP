---
unique-page-id: 4720917
description: Facebook でのパーソナライズリマーケティング - Marketo ドキュメント - 製品ドキュメント
title: Facebook でのパーソナライズリマーケティング
exl-id: 47636afa-49df-40ba-8948-4f2850467c2f
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 100%

---

# Facebook でのパーソナライズリマーケティング {#personalized-remarketing-in-facebook}

パーソナライズリマーケティングを使用すると、RTP データと Facebook リマーケティングの力を利用して、ユーザーと再びエンゲージできます。

>[!PREREQUISITES]
>
>* [ウェブパーソナライズデータによるリターゲティング](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)設定を完成します
>* [](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel) [カスタムオーディエンスとリマーケティングに関する Facebook ドキュメント](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel)を確認します。


## Facebook でのオーディエンスの作成 {#creating-an-audience-in-facebook}

1. Facebook の Ads Manager で、「[オーディエンス](https://www.facebook.com/ads/audience_manager)」タブに移動します。

1. 「**ツール**」をクリックして、「**オーディエンス**」を選択します。

   ![](assets/one-1.png)

1. 「**カスタムオーディエンスを作成**」をクリックします。

   ![](assets/two-1.png)

1. 「**ウェブサイトトラフィック**」を選択します。

   ![](assets/image2015-1-19-16-3a32-3a2.png)

1. ウェブサイトトラフィックリストで、「**カスタムの組み合わせ**」を選択します。

   ![](assets/image2015-1-19-16-3a33-3a21.png)

1. Include リストで、「**イベント**」を選択します。

   ![](assets/image2015-1-19-16-3a34-3a9.png)

1. イベントリストで、「**RTP リマーケティング**」を選択し、パラメーターを選択します。

   ![](assets/image2015-1-19-16-3a52-3a29.png)

1. この例では、「業界」に&#x200B;**教育**&#x200B;を含むように選択します。「**教育**」を入力し、「**過去の期間**」を編集して 180 日にします。オーディエンス名に「**教育業界**」と入力します。「**オーディエンスを作成**」をクリックします。

   ![](assets/image2015-1-19-16-3a56-3a15.png)

1. これで、Facebook で RTP データを使用して新しいカスタムオーディエンスを作成しました。

   ![](assets/image2015-1-19-16-3a59-3a2.png)

## Facebook の RTP データポイント {#rtp-data-points-in-facebook}

<table> 
 <tbody> 
  <tr> 
   <th>イベント名</th> 
   <th> </th> 
  </tr> 
  <tr> 
   <td>RTP リマーケティング</td> 
   <td> 
    <div> 
     <table> 
      <tbody> 
       <tr> 
        <th>パラメーター</th> 
        <th>値</th> 
       </tr> 
       <tr> 
        <td>ABM リスト</td> 
        <td>（顧客ベースのリスト）</td> 
       </tr> 
       <tr> 
        <td colspan="1">カテゴリ</td> 
        <td colspan="1"><p>Fortune 500</p><p>Fortune 1000</p><p>Global 2000</p></td> 
       </tr> 
       <tr> 
        <td colspan="1">グループ</td> 
        <td colspan="1"><p>エンタープライズ</p><p>中小企業</p></td> 
       </tr> 
       <tr> 
        <td>業界</td> 
        <td><p>防衛</p><p>教育</p><p>金融サービス</p><p>政府</p><p>医療、医薬品、バイオテクノロジー</p><p>ソフトウェア、インターネット</p><p>...（RTP 業界のオプションに従って）</p></td> 
       </tr> 
       <tr> 
        <td colspan="1">セグメント化されたオーディエンス</td> 
        <td colspan="1">（RTP で作成されたセグメント化されたオーディエンス名）</td> 
       </tr> 
      </tbody> 
     </table> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

## 広告によるオーディエンスのターゲティング {#target-your-audience-with-an-ad}

詳しくは、[Facebook ドキュメント](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#target-your-audience)を参照してください。

1. Ads Manager に移動し、「**広告を作成**」をクリックします。

   ![](assets/image2015-1-19-17-3a10-3a19.png)

1. キャンペーンの目的として「**ウェブサイトにリードを送信**」を選択します。

   ![](assets/image2015-1-19-17-3a11-3a20.png)

1. ウェブサイトの URL を入力します。

   ![](assets/image2015-1-19-17-3a12-3a39.png)

1. 広告セットを作成します。作成したオーディエンスのリストからカスタムオーディエンスを選択します（例：教育業界）。

   ![](assets/image2015-1-19-17-3a18-3a13.png)

1. その他すべての広告セットオプションを選択し、予算を設定して、広告クリエイティブを定義します。

   ![](assets/image2015-1-19-17-3a19-3a25.png)

1. これで、Facebook でパーソナライズされたリマーケティングキャンペーンの設定が完了しました。

>[!MORELIKETHIS]
>
>* [ウェブパーソナライズデータによるリターゲティング](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* [Google でのパーソナライズリマーケティング](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md)

