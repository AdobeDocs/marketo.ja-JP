---
unique-page-id: 2950555
description: Facebookのリッチ投稿設定の編集 — Marketto Docs — 製品ドキュメント
title: Facebookリッチ投稿設定の編集
translation-type: tm+mt
source-git-commit: 44ed91b485b52173922c709de63a4353e16c5072
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---


# Facebookリッチ投稿設定の編集 {#edit-facebook-rich-post-settings}

ユーザーがFacebookで [共有した場合に投稿をカスタマイズします](http://docs.marketo.com/display/docs/social) 。

>[!NOTE]
>
>**可用性**
>
>この機能を購入していないお客様もいます。 詳細については、セールス担当者にお問い合わせください。

Marketor [Socialアプリ](http://docs.marketo.com/display/docs/social) ：リードがFacebookやTwitterなどのソーシャルネットワーク上のランディングページとつながりを共有できます。 FacebookのOpenGraphタグ（OGタグ）を使用すると、ランディングページのどの情報をFacebookの投稿に含めるかを指定できます。

## リッチ投稿のオプションを選択 {#select-rich-post-options}

ランディングページからの共有によって生成されたFacebookリッチ投稿で使用するページ情報のタイプを指定できます。

1. YouTube **ビデオまたはソーシャルボタン用のエディターで** 、「 **Facebookメッセージ** 」を選択します。

   ![](assets/image2014-9-22-16-3a47-3a21.png)

1. Facebookメッセージに対して、次のオプションから選択します。

   * 静的追加コンテンツ：タイトル、キャプション、説明を手動で入力するには、このオプションを選択します。

      ![](assets/image2014-9-22-16-3a48-3a0.png)

   * 動的追加コンテンツ：Socialアプリでは、ランディングページの `<TITLE>`タグ、タグ `<CAPTION>``<DESCRIPTION>` 、タグを使用してリッチ投稿を入力できます。

      ![](assets/image2014-9-22-16-3a48-3a9.png)
   >[!NOTE]
   >
   >これらのタグはページソースに既に存在するはずですが、管理を強化するために、特定のFacebook OGタグをランディングページに [追加できます](edit-facebook-rich-post-settings.md)。

   * リッチコンテンツを追加しない：ランディングページからのFacebook投稿を、メインメッセージとリンクのみに制限します。

      ![](assets/image2014-9-22-16-3a48-3a18.png)



## ランディングページ追加へのFacebook OGタグ {#add-facebook-og-tags-to-a-landing-page}

ランディングページからFacebook共有に含めるページ要素を制御するには、ランディングページにタイトル、キャプション、説明のFacebook OG(Open Graph)タグを追加します。

1. YouTubeビデオ **** またはソーシャルボタンを含むランディングページを開きます。

   ![](assets/image2014-9-22-16-3a51-3a28.png)

   ランディングページ **デザイナが新しいウィンドウで開きます** 。

1. 「 **ランディングページアクション** / **ページメタタグを編集**」を選択します。*.*

   ![](assets/image2014-9-22-16-3a51-3a36.png)

1. 追加log:title、og:captionおよびog:descriptionを定義するHTMLです。 次の行をコピーして貼り付け、プレースホルダーテキストを置き換えます。

   `<meta property="og:title" content="My Post Title"/>`

   `<meta property="og:caption" content="My Post Caption"/>`

   `<meta property="og:description" content="This text appears in the post description"/>`

   ![](assets/image2014-9-22-16-3a52-3a8.png)

>[!NOTE]
>
>OGタグを追加する際は、適切なHTML構文を使用するように注意してください。
