---
unique-page-id: 11385579
description: コンテンツパターンの作成 - Marketo ドキュメント - 製品ドキュメント
title: コンテンツパターンの作成
exl-id: 963529fb-1b30-486c-b97d-3ff697f91258
feature: Predictive Content
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 82%

---

# コンテンツパターンの作成 {#create-content-patterns}

コンテンツパターンを設定すると、web 訪問者がそのコンテンツパターンに関連する HTML web ページをクリックしたとき、コンテンツが自動検出されます。これは、コンテンツ分析ページにコンテンツとして HTML ページ（ブログ投稿、プレスリリース、ニュース記事など）を追加するために使用されます。コンテンツパターンに基づいて自動検出すると、web 訪問者が閲覧しているとき、またはページへのリンクをクリックするときに、定義された URL パターンに関連する HTML ページを検出し、トラックすることができます。このコンテンツ（URL、ページ名、画像 URL などのメタデータ、説明）は、予測コンテンツを作成する際、すべてのコンテンツページに追加されます。PDF や埋め込み動画など、その他のコンテンツの自動検出については、[コンテンツ検索を有効にする](/help/marketo/product-docs/predictive-content/getting-started/enable-content-discovery.md)必要があります。

1. 「**[!UICONTROL コンテンツ設定]**」に移動します。

   ![](assets/settings-dropdown-hand-2.png)

1. 「**[!UICONTROL URL パターン]**」をクリックします。

   ![](assets/click-url-patterns-hand.png)

1. 「**+**」をクリックして行を開き、情報を入力します。

   ![](assets/content-settings-create-patterns-hand.png)

1. Web ページが存在するドメインの URL 拡張子を追加します。カテゴリを選択します（例：[!UICONTROL &#x200B; ブログ &#x200B;]、[!UICONTROL &#x200B; 記事 &#x200B;]、[!UICONTROL &#x200B; データシート &#x200B;]、[!UICONTROL &#x200B; プレスリリース &#x200B;]）。

   ![](assets/content-settings-create-content-patterns-dm-hands.png)

   >[!NOTE]
   >
   >右側のドロップダウンリストの項目は、[作成したカテゴリ](/help/marketo/product-docs/predictive-content/getting-started/set-up-categories.md)に設定したカテゴリを反映しています。

1. 「**+**」をクリックして、別のパスを追加します。

   ![](assets/url-patterns-add2.png)

1. 追加パスの拡張子とカテゴリを追加し、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/url-patterns-save.png)

## コンテンツパターンのルール {#content-pattern-rules}

* ワイルドカードは、式内の任意の場所で使用できます（例：_domain.com/&#42;_, _domain.com/&#42;blog&#42;_）

* 式の最後に/&#42; を使用して、パターン検出を続行することをお勧めします（例：_domain.com/blog/&#42;_ は、ブログフォルダー内のすべての投稿を検出します）
* コンテンツパターンでは大文字と小文字が区別されません（例：_domain.com/Blog/&#42;_ は、_domain.com/Blog&rbrace; および_ 4&rbrace;domain.com/blog _上のすべての HTML ページを検出します）_

* URL パラメーターは検出しません（これにより、同じコンテンツ URL で異なるパラメーターを持つ複数の項目が検出されるのを回避します）

## 例 {#examples}

_domain.com_ の場合：

<table>
 <tbody>
  <tr>
   <th>URL パターン</th>
   <th>結果</th>
  </tr>
  <tr>
   <td>blog/*</td>
   <td><p>domain.com/blog/ というパターンに一致するすべてのコンテンツを検出します。</p><p>domain.com/blog/5-top-tricks</p><p>domain.com/blog/2017/new-year-solutions</p><p>domain.com/Blog/3-best-recipes</p></td>
  </tr>
  <tr>
   <td>article/2017/*</td>
   <td><p>domain.com/article/2017/ というパターンに一致するすべてのコンテンツを検出します。</p><p>domain.com/article/2017/5-top-tricks</p></td>
  </tr>
  <tr>
   <td><img alt="--" width="80" src="assets/image2017-3-24-10-3a38-3a46.png" data-linked-resource-id="12976559" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11385579" title="--"></td>
   <td><p>「datasheets」という単語を含む URL を検出します。</p><p>domain.com/datasheets/5-top-tricks</p><p>domain.com/blog/5-top-datasheets</p></td>
  </tr>
  <tr>
   <td>press-release</td>
   <td><p>完全に一致する HTML ページが 1 つだけ検出されます。</p><p>domain.com/press-release</p></td>
  </tr>
  <tr>
   <td colspan="1"> </td>
   <td colspan="1"><p>URL 式が空の場合、URL パターンはホームページのみを検出します。</p><p>domain.com</p></td>
  </tr>
 </tbody>
</table>
