---
unique-page-id: 11385579
description: コンテンツパターンの作成 — Marketto Docs — 製品ドキュメント
title: コンテンツパターンの作成
translation-type: tm+mt
source-git-commit: f28ff1acb0090892bdb92b75ef90d489db7abf20
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 0%

---


# コンテンツパターンの作成 {#create-content-patterns}

>[!NOTE]
>
>購入日に応じて、マーケティング担当購読に「予測コンテンツ」または「コンテンツ`<sup>AI</sup>`」が含まれる場合があります。 予測コンテンツを使用するユーザーの場合、Marketing Cloudでは、2018年4月31日までコンテンツ`<sup>AI</sup>` 分析機能を有効にしています。 これらの機能をこの日以降に引き続きご利用いただくには、マーケティング担当者カスタマーサクセスマネージャーにお問い合わせの上、マーケティングコンテンツにアップグレードしてください`<sup>AI</sup>`。

コンテンツパターンを設定すると、Web訪問者がコンテンツパターンに関連するHTML Webページをクリックしたときに、コンテンツが自動検出されます。 HTMLページ（ブログ投稿、プレスリリース、ニュース記事）をコンテンツ要素として「すべてのコンテンツ」ページに追加するために使用します。 コンテンツパターンに基づいた自動検出では、Web訪問者ーがページへのリンクを表示またはクリックしたときに、定義済みのURLパターンに関連するHTMLページを検出して追跡します。 このコンテンツ部分（URL、ページ名、画像URLや説明を含むメタデータ）をすべてのコンテンツページに追加して、予測コンテンツを準備します。 PDFや埋め込みビデオなど、他のコンテンツの自動検出を行うには、コンテンツの検出を [有効にする必要があります](enable-content-discovery.md)。

1. 「 **コンテンツ設定**」に移動します。

   ![](assets/settings-dropdown-hand-2.png)

1. 「 **URLパターン**」をクリックします。

   ![](assets/click-url-patterns-hand.png)

1. **+ **をクリックすると、行が開き、情報を入力できます。

   ![](assets/content-settings-create-patterns-hand.png)

1. webページが追加存在するドメインのURL拡張子。 カテゴリ（ブログ、記事、データシート、プレスリリースなど）を選択します。

   ![](assets/content-settings-create-content-patterns-dm-hands.png)

   >[!NOTE]
   >
   >右側のドロップダウンリストの項目は、カテゴリを [作成したときに設定したカテゴリを反映しています](set-up-categories.md)。

1. **+ **をクリックして、別のパスを追加します。

   ![](assets/url-patterns-add2.png)

1. 追加追加パスの拡張子とカテゴリを指定し、「 **保存**」をクリックします。

   ![](assets/url-patterns-save.png)

## コンテンツパターンのルール {#content-pattern-rules}

* 式内の任意の場所にワイルドカードを使用できます(例： *domain.com/**、 *domain.com/*blog**)

* パターン検出を続行するには、式の最後に/*を使用することをお勧めします(例： *domain.com/blog/** discover all posts in the Blog folder)
* コンテンツパターンでは大文字と小文字が区別されません(例： *domain.com/Blog/** は、domain.com/Blogおよびdomain.com/blogにあるすべてのhtmlページを *検出します***)。

* URLパラメーターが見つからない（これにより、同じコンテンツURLで異なるパラメーターを持つ複数の項目を見つけることができます）

## 例 {#examples}

*domain.comの場合*:

<table> 
 <tbody> 
  <tr> 
   <th>URLパターン</th> 
   <th>結果</th> 
  </tr> 
  <tr> 
   <td>blog/*</td> 
   <td><p>次のパターンに一致するすべてのコンテンツを見つけます：domain.com/blog/</p><p>domain.com/blog/5-top-tricks</p><p>domain.com/blog/2017/new-year-solutions</p><p>domain.com/Blog/3-best-recipes</p></td> 
  </tr> 
  <tr> 
   <td>article/2017/*</td> 
   <td><p>次のパターンに一致するすべてのコンテンツを見つけます：domain.com/article/2017/</p><p>domain.com/article/2017/5-top-tricks</p></td> 
  </tr> 
  <tr> 
   <td><img alt="--" width="80" src="assets/image2017-3-24-10-3a38-3a46.png" data-linked-resource-id="12976559" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11385579" title="--"></td> 
   <td><p>「datasheets:」という語を含むURLを検出します。</p><p>domain.com/datasheets/5-top-tricks</p><p>domain.com/blog/5-top-datasheets</p></td> 
  </tr> 
  <tr> 
   <td>プレスリリース</td> 
   <td><p>検出されたHTMLページは、次のうち1つだけです。</p><p>domain.com/press-release</p></td> 
  </tr> 
  <tr> 
   <td colspan="1"> </td> 
   <td colspan="1"><p>URL式ーが空の場合、URLパターンは次のホームページのみを検出します。</p><p>domain.com</p></td> 
  </tr> 
 </tbody> 
</table>

