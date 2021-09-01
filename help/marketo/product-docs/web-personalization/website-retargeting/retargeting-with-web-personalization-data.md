---
unique-page-id: 4720796
description: Web パーソナライゼーションデータによるリターゲティング — Marketo ドキュメント — 製品ドキュメント
title: Web パーソナライゼーションデータによるリターゲティング
exl-id: b5af1f84-2061-4d0d-9d1f-2fff9191f028
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '406'
ht-degree: 100%

---

# Web パーソナライゼーションデータによるリターゲティング {#retargeting-with-web-personalization-data}

>[!AVAILABILITY]
>
>Web サイトのリターゲティングが、 Web パーソナライゼーションタイルの下に表示されるようになりました。リターゲティングのみを購入した場合は、このタイルが表示され、リターゲティング機能&#x200B;**のみ**&#x200B;が有効になっているパーソナライゼーション製品にアクセスできます。アカウント設定、リターゲティングページ、セグメント、追加のトラッキングページにアクセスできます。

「どんな人か」「何をしたか」に基づく広告表示を利用して、過去にサイトを訪問した見込み客を、リマーケティングのターゲットにします。パーソナライズされたレターゲティングでは、業界、特定顧客および認識済みリードのデータに基づき、関連性のある広告を出すことで特定のオーディエンスにターゲティングできます。

現在、Web パーソナライゼーションは、次のリマーケティングプラットフォームにデータを追加します。

* [Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md)
* [Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)

Web パーソナライゼーションは、次のデータをリマーケティングプラットフォームに送信して、オーディエンスを作成し、リマーケティング広告キャンペーンを実行します。

<table> 
 <tbody> 
  <tr> 
   <th colspan="1">Web パーソナライゼーションデータ</th> 
  </tr> 
  <tr> 
   <th><p>業界</p></th> 
  </tr> 
  <tr> 
   <th><p>グループ（エンタープライズ、SMB）</p></th> 
  </tr> 
  <tr> 
   <th><p>カテゴリー（Fortune 500/1000、Global 2000）</p></th> 
  </tr> 
  <tr> 
   <th><p>ABM リスト（名前付きアカウントリスト）</p></th> 
  </tr> 
  <tr> 
   <th><p>セグメント化オーディエンス（セグメントに基づく）</p></th> 
  </tr> 
  <tr> 
   <th><p>クリックされた Web キャンペーン</p></th> 
  </tr> 
 </tbody> 
</table>

## リマーケティング設定 {#remarketing-configuration}

1. 「**リターゲティング**.」に移動します。

   ![](assets/one.png)

   >[!NOTE]
   >
   >リターゲティング設定は、ドメインごとまたはサブドメインごとにおこないます。これらのドメインからを通じてリターゲティングプラットフォームにデータを送信する場合は、他のドメインをアクティブ化します。

1. ドメインごとに、Google Analytics または Google ユニバーサルアナリティクスの設定をアクティブ化します。

   >[!NOTE]
   >
   >Web サイトに Google リターゲティングタグを実装する必要があります。
   >
   >Web パーソナライゼーションと Google Analytics との連携をすでに設定している場合は、「アカウント設定」の設定と同じなので、この部分を編集する必要はありません。

   ![](assets/two.png)

1. Facebook の設定をアクティブ化します。「Facebook」アコーディオンをクリックして展開し、「**オン**」をクリックして、それぞれのイベントとデータを Facebook Audience Manager に送信します。「**保存**」をクリックします。

   >[!NOTE]
   >
   >この機能を動作させるには、[Facebook Custom Audience Pixel](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel) を Web サイトにインストールする必要があります。

   ![](assets/three.png)

## セグメント化オーディエンスを作成する {#creating-segmented-audience}

セグメント化オーディエンスを使用すると、既存のセグメントをオーディエンスとして選択し、リターゲティングキャンペーンに使用できます。例えば、認識済みリードのセグメントを選択します。

>[!TIP]
>
>業界用や、ドメイン設定で既に送信されているその他のデータ用に、セグメント化オーディエンスを作成する必要はありません。セグメント化オーディエンスは、認識済みリードのデータに基づいたセグメントに対して使用するのが最適です。

1. 「**セグメント化オーディエンスを作成**」をクリックします。

   ![](assets/image2015-1-15-16-3a36-3a38.png)

1. オーディエンス名を入力し、「チャネル」を選択し、既存のセグメントのリストから「セグメント」を選択します。

   ![](assets/image2015-1-15-16-3a40-3a17.png)

1. 「**保存**」をクリックします。

   これで、Web パーソナライゼーションのリターゲティングの設定が完了し、リターゲティングプラットフォームにログインして、このデータに基づいてオーディエンスを作成し、リターゲティング広告キャンペーンを設定しました。
