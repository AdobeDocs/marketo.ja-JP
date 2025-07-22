---
unique-page-id: 4720796
description: ウェブパーソナライズデータによるリターゲティング — Marketo ドキュメント — 製品ドキュメント
title: ウェブパーソナライズデータによるリターゲティング
exl-id: b5af1f84-2061-4d0d-9d1f-2fff9191f028
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 71%

---

# [!DNL Web Personalization] データによるリターゲティング {#retargeting-with-web-personalization-data}

>[!AVAILABILITY]
>
>ウェブサイトのリターゲティングが、ウェブパーソナライズタイルの下に表示されるようになりました。リターゲティングのみを購入した場合、このタイルが表示され、[!DNL Web Personalization] のみ **リターゲティング機能が有効になっている** 製品にアクセスできます。 アカウント設定、リターゲティングページ、セグメント、追加のトラッキングページにアクセスできます。

「どんな人か」「何をしたか」に基づく広告表示を利用して、過去にサイトを訪問した見込み客を、リマーケティングのターゲットにします。パーソナライズされたレターゲティングでは、業界、特定顧客および認識済みリードのデータに基づき、関連性のある広告を出すことで特定のオーディエンスにターゲティングできます。

現在、ウェブパーソナライズは、次のリマーケティングプラットフォームにデータを追加します。

* [Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md)
* [Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)

[!DNL Web Personalization] は、オーディエンスを作成しリマーケティング広告キャンペーンを実行するために、次のデータをを通じてリマーケティングプラットフォームに送信します。

<table> 
 <tbody> 
  <tr> 
   <th colspan="1">[!DNL Web Personalization] データ</th> 
  </tr> 
  <tr> 
   <th><p>業界</p></th> 
  </tr> 
  <tr> 
   <th><p>グループ（エンタープライズ、中小企業）</p></th> 
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

1. 「**[!UICONTROL リターゲティング]**.」に移動します。

   ![](assets/one.png)

   >[!NOTE]
   >
   >リターゲティング設定は、ドメインごとまたはサブドメインごとにおこないます。これらのドメインからを通じてリターゲティングプラットフォームにデータを送信する場合は、他のドメインをアクティブ化します。

1. ドメインごとにGoogle Analyticsまたは [!DNL Google Universal Analytics] の設定をアクティベートします。

   >[!NOTE]
   >
   >ウェブサイトに Google リターゲティングタグを実装する必要があります。
   >
   >ウェブパーソナライズと Google Analytics との連携をすでに設定している場合は、「アカウント設定」の設定と同じなので、この部分を編集する必要はありません。

   ![](assets/two.png)

1. Facebook の設定をアクティブ化します。「[!DNL Facebook]」アコーディオンをクリックして展開し、「**[!UICONTROL オン]**」をクリックして、それぞれのイベントとデータを Facebook Audience Managerに送信します。 「**[!UICONTROL 保存]**」をクリックします。

   >[!NOTE]
   >
   >この機能を使用するには、[[!DNL Facebook]  カスタムオーディエンスピクセル ](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel) が Web サイトにインストールされている必要があります。

   ![](assets/three.png)

## セグメント化オーディエンスを作成する {#creating-segmented-audience}

セグメント化オーディエンスを使用すると、既存のセグメントをオーディエンスとして選択し、リターゲティングキャンペーンに使用できます。例えば、認識済みリードのセグメントを選択します。

>[!TIP]
>
>業界用や、ドメイン設定で既に送信されているその他のデータ用に、セグメント化オーディエンスを作成する必要はありません。セグメント化オーディエンスは、認識済みリードのデータに基づいたセグメントに対して使用するのが最適です。

1. 「**[!UICONTROL セグメント化オーディエンスを作成]**」をクリックします。

   ![](assets/image2015-1-15-16-3a36-3a38.png)

1. オーディエンス名を入力し、「チャネル」を選択し、既存のセグメントのリストから「セグメント」を選択します。

   ![](assets/image2015-1-15-16-3a40-3a17.png)

1. 「**[!UICONTROL 保存]**」をクリックします。

   これで、[!DNL Web Personalization] でリターゲティングの設定を完了し、リターゲティングプラットフォームにログインし、このデータに基づいてオーディエンスを作成し、リターゲティング広告キャンペーンを設定しました。
