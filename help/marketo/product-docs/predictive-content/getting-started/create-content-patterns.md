---
unique-page-id: 11385579
description: コンテンツパターンの作成 — Marketto Docs — 製品ドキュメント
title: コンテンツパターンの作成
translation-type: tm+mt
source-git-commit: 06e0f5489e6375a97e2fe77834bf45fa41f23ea6
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 0%

---


# コンテンツパターンを作成{#create-content-patterns}

コンテンツパターンを設定すると、Web訪問者がコンテンツパターンに関連するHTML Webページをクリックしたときに、コンテンツが自動検出されます。 HTMLページ（ブログ投稿、プレスリリース、ニュース記事）をコンテンツ要素として「すべてのコンテンツ」ページに追加するために使用します。 コンテンツパターンに基づいた自動検出では、Web訪問者ーがページへのリンクを表示またはクリックしたときに、定義済みのURLパターンに関連するHTMLページを検出して追跡します。 このコンテンツ部分（URL、ページ名、画像URLや説明を含むメタデータ）をすべてのコンテンツページに追加して、予測コンテンツを準備します。 PDFや埋め込みビデオなど、他のコンテンツを自動検出するには、[コンテンツ検出を有効にする](/help/marketo/product-docs/predictive-content/getting-started/enable-content-discovery.md)必要があります。

1. 「**コンテンツ設定**」に移動します。

   ![](assets/settings-dropdown-hand-2.png)

1. 「**URLパターン**」をクリックします。

   ![](assets/click-url-patterns-hand.png)

1. **+**&#x200B;をクリックすると、情報を入力できる行が開きます。

   ![](assets/content-settings-create-patterns-hand.png)

1. webページが追加存在するドメインのURL拡張子。 カテゴリ（ブログ、記事、データシート、プレスリリースなど）を選択します。

   ![](assets/content-settings-create-content-patterns-dm-hands.png)

   >[!NOTE]
   >
   >右側のドロップダウンリストの項目は、[カテゴリ](/help/marketo/product-docs/predictive-content/getting-started/set-up-categories.md)を作成したときに設定したカテゴリを反映しています。

1. **+**&#x200B;をクリックして、別のパスを追加します。

   ![](assets/url-patterns-add2.png)

1. 追加追加パスの拡張子とカテゴリを指定し、「**保存**」をクリックします。

   ![](assets/url-patterns-save.png)

## コンテンツパターンルール{#content-pattern-rules}

* 式内の任意の場所にワイルドカードを使用できます(例：_domain.com/*_, _domain.com/*blog*_)

* パターン検出を続行するには、式の最後に/*を使用することをお勧めします(例：_domain.com/blog/*_&#x200B;は、ブログフォルダー内のすべての投稿を検出します)。
* コンテンツパターンでは大文字と小文字が区別されません(例：_domain.com/Blog/*_&#x200B;は、_domain.com/Blog_&#x200B;と&#x200B;_domain.com/blog_)にあるすべてのhtmlページを検出します

* URLパラメーターが見つからない（これにより、同じコンテンツURLで異なるパラメーターを持つ複数の項目を見つけることができます）

## 例{#examples}

_domain.com_&#x200B;の場合：

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
   <td><img alt="—" width="80" src="assets/image2017-3-24-10-3a38-3a46.png" data-linked-resource-id="12976559" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11385579" title="—"></td> 
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
