---
unique-page-id: 4719400
description: ゾーン内での新しいWebキャンペーンの作成 — Marketto Docs — 製品ドキュメント
title: ゾーン内の新しいWebキャンペーンの作成
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '694'
ht-degree: 0%

---


# ゾーン内の新しいWebキャンペーンの作成{#create-a-new-in-zone-web-campaign}

Webキャンペーンは、特定のセグメントに関連付けられたカスタマイズされた反応で、Webサイト上の[ダイアログボックス](create-a-new-dialog-web-campaign.md)、ゾーン内置き換え、[ウィジェット機能](create-a-new-widget-web-campaign.md)、電子メールアラートのいずれかになります。 ゾーン内Webキャンペーンは、ゾーンIDに基づくWebサイトの要素を、コンテンツまたはグラフィカルバナーで置き換えます。

## ゾーン内Webキャンペーンの作成{#create-an-in-zone-web-campaign}

1. **Webキャンペーン**&#x200B;に移動します。

   ![](assets/image2016-8-18-15-3a54-3a21.png)

1. 「**新しいWebキャンペーンーを作成」を選択します。**

   ![](assets/create-new-web-campaign-hand.png)

1. 「**ゾーン**&#x200B;内」キャンペーンタイプを選択します。 **ゾーンIDをカスタマイズして追加します。** キャンペーンを「ス **** ティッキー」に設定し、エディターでクリエイティブを追加します。プレビュー追加へのページのURLを指定し、「**プレビュー**」をクリックして、キャンペーンがサイト上でどのように反応するかを確認します。

   ![](assets/new-3-1.png)

   >[!NOTE]
   >
   >**定義**
   >
   >
   >**ゾーンIDとは**
   >
   >
   >ゾーンIDは、「ゾーン内」Webキャンペーンをオンサイトに配置する場所です。 「ゾーンID」を見つけるには、Webサイトにアクセスし、Webキャンペーンーで置き換える領域を選択して右クリックします。 Chromeでは「Inspect要素」を選択できますが、他のブラウザーでは異なる場合があります。
   >
   >
   >次に、Webサイトのこのセクションに関連付けられた「id」を探します。この「id」は、その要素を検査しているので強調表示されます。 例えば、Chromeで右クリックすると、強調表示されているテキストに`<div id="featured-slider">`と表示される場合は、「ゾーンID」セクションに「featured-slider」と入力する必要があります。 通常は&quot;div id&quot;が使用されますが、h1 id、p idなどの任意のIDも使用できます。

<table> 
 <thead> 
  <tr> 
   <th colspan="1" rowspan="1">名前</th> 
   <th colspan="1" rowspan="1">説明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="1" rowspan="1"><strong> ゾーンID </strong></td> 
   <td colspan="1" rowspan="1"><p>キャンペーンが置き換えるWebサイト要素のHTMLコードにあるIDの名前を入力します。</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong> 定着 </strong></p></td> 
   <td colspan="1" rowspan="1">「ゾーン内」キャンペーンではデフォルトで「固定」チェックボックスが選択されており、Webサイト上の訪問者のセッション全体で、ゾーン内キャンペーンがゾーンIDの位置を維持します。 常に「インゾーン」を「固定」に設定することをお勧めします。</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong> フェード</strong> </p></td> 
   <td colspan="1" rowspan="1">「効果を使用」チェックボックスと「フェード」を選択すると、WebサイトのゾーンID領域にフェード効果を適用できます。 「インゾーン」がグラフィカルバナーの場合、ページが最初に読み込まれ、次にキャンペーンがフェード効果でアクティブになります。</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong>スライド</strong></td> 
   <td colspan="1">「効果を使用」チェックボックスと「スライディング」オプションを選択すると、Webサイトの「ゾーンID」領域にスライディングが有効になります。 「インゾーン」がグラフィカルバナーの場合、ページが最初に読み込まれ、次にキャンペーンが左から右にスライドする効果でアクティブになります。</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong> リッチテキストエディタ  </strong></td> 
   <td colspan="1">リッチテキストエディターでは、テキストの書式設定、リンク、および画像の挿入が可能です。 <a href="using-the-web-personalization-rich-text-editor.md">詳しくはこちら</a> 。</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong> サイトでのプレビュー   </strong></td> 
   <td colspan="1">プレビューキャンペーンを起動する前に実行する必要があります。<br> 
    <ul> 
     <li> URL -キャンペーンが実行されるURLの例を入力し、キャンペーンがライブに見えるプレビューの例を確認します。</li> 
     <li>デバイス — デバイス別のキャンペーンの表示プレビュー:デスクトップ、モバイル向け縦置き、モバイル向け横置き、タブレット向け縦置き、縦置き</li> 
     <li> プレビュー- [<strong>プレビュー</strong>]をクリックすると、例のURLの新しいウィンドウが開き、キャンペーンがどのように反応するかが表示されます。</li> 
     <li> 共有 — [共有]ボタンを使用して、プロキシキャンペーンを表示するためのリンクを持つ同僚に電子メールを送信します。</li> 
    </ul></td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>組み込みのテンプレート](../../../product-docs/web-personalization/using-templates/using-templates-to-create-web-campaigns.md)を使用するか、既存のキャンペーン](../../../product-docs/web-personalization/using-templates/using-templates-to-create-web-campaigns.md)を再利用用のテンプレートとして保存することで、キャンペーンの作成プロセスを迅速化し、シンプル化します。[[

>[!NOTE]
>
>**WebキャンペーンーのA/Bテストを行う場合** 最適な結果を得るために、1つ以上のWebキャンペーンを [A/Bテストでき](ab-test-your-web-campaign.md)ます。自動調整機能を使用すると、プラットフォームは自動的にパフォーマンスの高いキャンペーンを認識し、コンバージョン率が最も高いキャンペーンを引き続き認識し、他のを一時停止します。

## Webキャンペーンの編集{#edit-a-web-campaign}

**Webキャンペーンー**&#x200B;ページから、キャンペーンーの&#x200B;**編集**&#x200B;をクリックします。

![](assets/in-zone-web-campaign-edit.png)

>[!NOTE]
>
>必要なキャンペーンを見つけやすくするには、[フィルター機能](filter-web-campaigns.md)を使用します。

## Webキャンペーンのプレビュー{#preview-a-web-campaign}

1. Webキャンペーンページで、表示するWebキャンペーンーの**プレビュー**をクリックします。

   ![](assets/in-zone-web-campaign-preview.png)

## Webキャンペーンのコピー{#clone-a-web-campaign}

[Webキャンペーンーのコピー](clone-a-web-campaign.md)を参照してください。

## Webキャンペーンの削除{#delete-a-web-campaign}

1. Webキャンペーンページで、削除するキャンペーンの「**削除**」をクリックします。

   ![](assets/in-zone-web-campaign-delete.png)

1. キャンペーンを削除するかどうかを確認するメッセージが表示されます。

>[!MORELIKETHIS]
>
>* [新しいウィジェットWebキャンペーンの作成](create-a-new-widget-web-campaign.md)
>* [新しいダイアログWebキャンペーンの作成](create-a-new-dialog-web-campaign.md)

