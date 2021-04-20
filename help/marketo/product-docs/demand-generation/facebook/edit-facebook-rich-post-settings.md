---
unique-page-id: 2950555
description: facebookリッチ投稿設定の編集 —Marketoドキュメント — 製品ドキュメント
title: facebookリッチ投稿の設定を編集
exl-id: f72bfb03-9bc7-46c4-bfb8-b377b2d23fc9
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 1%

---

# facebookリッチ投稿設定の編集{#edit-facebook-rich-post-settings}

ユーザーがFacebookで共有した投稿をカスタマイズします。

>[!AVAILABILITY]
>
>この機能を購入していないお客様もいます。  詳細は、営業取引先責任者にお問い合わせください。

Marketo[ソーシャルアプリ](/help/marketo/product-docs/demand-generation/social/social-functions/add-a-social-button-on-a-landing-page.md)では、リードがFacebookやTwitterなどのソーシャルネットワーク上のランディングページとのつながりを共有できます。 FacebookOpenGraphタグ（OGタグ）を使用すると、ランディングページのどの情報をFacebook投稿に含めるかを指定できます。

## リッチ投稿のオプションを選択{#select-rich-post-options}

ランディングページから共有によって生成されたFacebookリッチ投稿で使用するページ情報のタイプを指定できます。

1. **YouTube**&#x200B;ビデオまたはソーシャルボタン用のエディターで、**Facebookメッセージ**&#x200B;を選択します。

   ![](assets/image2014-9-22-16-3a47-3a21.png)

1. facebookメッセージに対して、次のオプションから選択します。

   * 静的追加コンテンツ：タイトル、キャプション、説明を手動で入力するには、このオプションを選択します。

   ![](assets/image2014-9-22-16-3a48-3a0.png)

   * 動的追加コンテンツ：ソーシャルアプリは、ランディングページの`<TITLE>`、`<CAPTION>`および`<DESCRIPTION>`タグを使用して、リッチ投稿を入力できます。

   ![](assets/image2014-9-22-16-3a48-3a9.png)

   >[!NOTE]
   >
   >これらは既にページソースに存在しているはずですが、管理を強化するために、特定のFacebookOGタグをランディングページに追加できます。

   * リッチコンテンツを追加しない：ランディングページからのFacebook投稿を、メインメッセージとリンクのみに制限します。

   ![](assets/image2014-9-22-16-3a48-3a18.png)

## 追加FacebookOGタグをランディングページに{#add-facebook-og-tags-to-a-landing-page}

ランディングページからFacebook共有に含まれるページ要素を制御するには、タイトル、キャプション、説明のFacebookOG(Open Graph)タグをランディングページに追加します。

1. **YouTubeビデオ**&#x200B;またはソーシャルボタンを含むランディングページを開きます。

   ![](assets/image2014-9-22-16-3a51-3a28.png)

   **ランディングページデザイナ**&#x200B;が新しいウィンドウで開きます。

1. **ランディングページアクション**/**ページのメタタグを編集**&#x200B;を選択します。

   ![](assets/image2014-9-22-16-3a51-3a36.png)

1. 追加log:title、og:captionおよびog:descriptionを定義するHTMLです。 次の行をコピーして貼り付け、プレースホルダーテキストを置き換えます。

   `<meta property="og:title" content="My Post Title"/>`

   `<meta property="og:caption" content="My Post Caption"/>`

   `<meta property="og:description" content="This text appears in the post description"/>`

   ![](assets/image2014-9-22-16-3a52-3a8.png)

>[!NOTE]
>
>OGタグを追加する際は、適切なHTML構文を使用するように注意してください。
