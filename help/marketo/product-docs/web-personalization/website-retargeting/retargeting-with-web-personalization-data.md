---
unique-page-id: 4720796
description: Webパーソナライゼーションデータを使用したリターゲティング — Marketto Docs — 製品ドキュメント
title: Webパーソナライゼーションデータを使用した再ターゲティング
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---


# Webパーソナライゼーションデータを使用した再ターゲティング{#retargeting-with-web-personalization-data}

>[!NOTE]
>
>**可用性**
>
>Webサイトの再ターゲティングが、Webパーソナライゼーションタイルの下に表示されるようになりました。 リターゲティングのみを購入した場合は、このタイルが表示され、**のみ**&#x200B;のリターゲティング機能が有効なWebパーソナライゼーション製品にアクセスできます。 これにより、アカウント設定、再ターゲティングページ、セグメントおよび追加のトラッキングページにアクセスできます。

過去にサイトを訪問したことのあるターゲット見込み客の再マーケティング（訪問者の人名と行動内容に基づくディスプレイ広告を含む）。 業界、指名されたアカウント、既知の人物データに基づき、関連する広告を含む、ターゲット固有のパーソナライズされたリターゲティングオーディエンス。

現在、Webパーソナライゼーションは、次のリマーケティングプラットフォームにデータを追加します。

* [Google](personalized-remarketing-in-google.md)
* [Facebook](personalized-remarketing-in-facebook.md)

Webパーソナライゼーションは、リマーケティングプラットフォームに以下のデータを送信して、オーディエンスを作成し、リマーケティング広告キャンペーンを実行します。

<table> 
 <tbody> 
  <tr> 
   <th colspan="1">Webパーソナライゼーションデータ</th> 
  </tr> 
  <tr> 
   <th><p>業界</p></th> 
  </tr> 
  <tr> 
   <th><p>グループ（エンタープライズ、SMB）</p></th> 
  </tr> 
  <tr> 
   <th><p>カテゴリ(Fortune 500/1000、Global 2000)</p></th> 
  </tr> 
  <tr> 
   <th><p>ABMリスト(固有のアカウントリスト)</p></th> 
  </tr> 
  <tr> 
   <th><p>セグメント化されたオーディエンス（セグメントに基づく）</p></th> 
  </tr> 
  <tr> 
   <th><p>クリックされたWebキャンペーン</p></th> 
  </tr> 
 </tbody> 
</table>

## リマーケティングの設定{#remarketing-configuration}

1. **リターゲティング**&#x200B;に移動します。

   ![](assets/one.png)

   >[!NOTE]
   >
   >再ターゲット設定は、ドメインまたはサブドメインごとに行われます。 これらのドメインから再ターゲティングプラットフォームにデータを送信する場合は、他のドメインをアクティブ化します。

1. ドメインごとにGoogle AnalyticsまたはGoogle Universal Analyticsの設定をアクティブにします。

   >[!NOTE]
   >
   >WebサイトにGoogle Retargetingタグを導入する必要があります。
   >
   >
   >既にWebパーソナライゼーションおよびGoogle Analyticsとの統合を設定している場合、このパーツは「アカウントの設定」の同じ設定なので、編集する必要はありません。

   ![](assets/two.png)

1. Facebookの設定をアクティブ化します。 Facebookアコーディオンをクリックして展開し、「**オン**」をクリックして、それぞれのイベントとデータをFacebookAudience Managerに送信します。 「**保存**」をクリックします。

   >[!NOTE]
   >
   >この機能を動作させるには、[Facebookカスタムオーディエンスピクセル](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel)をインストールする必要があります。

   ![](assets/three.png)

## セグメント化されたオーディエンスの作成{#creating-segmented-audience}

セグメント化オーディエンスを使用すると、既存のセグメントをキャンペーンの再ターゲティングに使用するオーディエンスとして選択できます。 例えば、既知の人のセグメントを選択します。

>[!TIP]
>
>ドメイン設定で既に送信されている業界や他のデータ用にセグメント化オーディエンスを作成する必要はありません。 既知の人物データに基づくセグメント化オーディエンスは、セグメント化されたユーザーに使用するのが最適です。

1. 「**セグメント化されたオーディエンスを作成**」をクリックします。

   ![](assets/image2015-1-15-16-3a36-3a38.png)

1. オーディエンス名を入力し、チャネルを選択して、既存のセグメントのリストから「セグメント」を選択します。

   ![](assets/image2015-1-15-16-3a40-3a17.png)

1. 「**保存**」をクリックします。

   これで、Webパーソナライゼーションのリターゲティング設定が完了し、リターゲティングプラットフォームにログインして、このデータに基づいてオーディエンスを作成し、リターゲティング広告キャンペーンを設定しました。

>[!MORELIKETHIS]
>
>* [Googleでのパーソナライズされたリマーケティング](personalized-remarketing-in-google.md)
>* [Facebookでのパーソナライズされたリマーケティング](personalized-remarketing-in-facebook.md)

