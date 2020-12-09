---
unique-page-id: 4720917
description: Facebookでのパーソナライズされたリマーケティング — Marketto Docs — 製品ドキュメント
title: Facebookでのパーソナライズされたリマーケティング
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '311'
ht-degree: 0%

---


# Facebookでのパーソナライズされたリマーケティング {#personalized-remarketing-in-facebook}

パーソナライズされたリマーケティングを使用すると、RTPデータとFacebookリマーケティングの機能を利用して、ユーザーと再び関わりを持つことができます。

>[!PREREQUISITES]
>
>* Webパーソナライゼーションデータの [再ターゲティング](retargeting-with-web-personalization-data.md) 設定の完了
>* カスタムオーディエンスとリマーケティングに関する [](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel) Facebookのドキュメントを確認し [](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel)ます。

>



## Facebookでのオーディエンスの作成 {#creating-an-audience-in-facebook}

1. Facebookで、広告マネージャーの [オーディエンスタブ](https://www.facebook.com/ads/audience_manager) 。
1. 「 **ツール** 」をクリックし、「 **オーディエンス**」を選択します。

   ![](assets/one-1.png)

1. 「カスタムオーディエンスを **作成**」をクリックします。

   ![](assets/two-1.png)

1. 「 **Webサイトトラフィック**」を選択します。

   ![](assets/image2015-1-19-16-3a32-3a2.png)

1. Webサイトトラフィックリストで、「**カスタムの組み合わせ**」を選択します。

   ![](assets/image2015-1-19-16-3a33-3a21.png)

1. 「含める」リストで、「 **イベント**」を選択します。

   ![](assets/image2015-1-19-16-3a34-3a9.png)

1. イベントリストで、「**RTP Remarketing **」を選択し、パラメータを選択します。

   ![](assets/image2015-1-19-16-3a52-3a29.png)

1. この例では、「 **Education**」を含める業種を選択します。 「 **Education**」と入力し、「In **The Last** 」を180日に編集します。 オーディエンス名を入力： **教育業界**。 「 **オーディエンスを作成**」をクリックします。

   ![](assets/image2015-1-19-16-3a56-3a15.png)

1. これで、FacebookのRTPデータを使用して新しいカスタムオーディエンスが作成されました。

   ![](assets/image2015-1-19-16-3a59-3a2.png)

## FacebookのRTPデータポイント {#rtp-data-points-in-facebook}

<table> 
 <tbody> 
  <tr> 
   <th>イベント名</th> 
   <th> </th> 
  </tr> 
  <tr> 
   <td>RTP再マーケティング</td> 
   <td> 
    <div> 
     <table> 
      <tbody> 
       <tr> 
        <th>パラメータ</th> 
        <th>値</th> 
       </tr> 
       <tr> 
        <td>ABMリスト</td> 
        <td>(口座開設リストの名称)</td> 
       </tr> 
       <tr> 
        <td colspan="1">カテゴリ</td> 
        <td colspan="1"><p>フォーチュン500</p><p>Fortune 1000</p><p>グローバル2000</p></td> 
       </tr> 
       <tr> 
        <td colspan="1">グループ</td> 
        <td colspan="1"><p>Enterprise</p><p>SMB</p></td> 
       </tr> 
       <tr> 
        <td>業界</td> 
        <td><p>防衛</p><p>教育</p><p>金融サービス</p><p>政府機関</p><p>医療、製薬、バイオテク</p><p>ソフトウェアとインターネット</p><p>など（RTP Industryオプションに基づく）</p></td> 
       </tr> 
       <tr> 
        <td colspan="1">セグメント化されたオーディエンス</td> 
        <td colspan="1">(RTPで作成されたセグメント化オーディエンスの名前)</td> 
       </tr> 
      </tbody> 
     </table> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

## 広告でのオーディエンスのターゲット {#target-your-audience-with-an-ad}

詳しくは、 [Facebookのドキュメントを参照してください](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#target-your-audience)。

1. 広告マネージャーに移動し、「広告を **作成**」をクリックします。

   ![](assets/image2015-1-19-17-3a10-3a19.png)

1. キャンペーンの目的として **「Webサイトにユーザーを送信** 」を選択します。

   ![](assets/image2015-1-19-17-3a11-3a20.png)

1. WebサイトのURLを入力します。

   ![](assets/image2015-1-19-17-3a12-3a39.png)

1. 広告セットを作成します。 作成したオーディエンスのリストからカスタムオーディエンスを選択します（例：Education Industry）。

   ![](assets/image2015-1-19-17-3a18-3a13.png)

1. その他すべての広告セットオプションを選択し、予算を設定して広告クリエイティブを定義します。

   ![](assets/image2015-1-19-17-3a19-3a25.png)

1. これで、Facebookでパーソナライズされたリマーケティングキャンペーンが設定されました。

>[!NOTE]
>
>**関連記事**
>
>* [Webパーソナライゼーションデータを使用した再ターゲティング](retargeting-with-web-personalization-data.md)
>* [Googleでのパーソナライズされたリマーケティング](personalized-remarketing-in-google.md)

>



