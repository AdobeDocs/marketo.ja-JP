---
unique-page-id: 2950555
description: Facebook リッチ投稿設定の編集 - Marketo ドキュメント - 製品ドキュメント
title: Facebook リッチ投稿設定の編集
exl-id: f72bfb03-9bc7-46c4-bfb8-b377b2d23fc9
hide: true
hidefromtoc: true
feature: Integrations
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 50%

---

# リッチ投稿設定 [!DNL Facebook] 編集 {#edit-facebook-rich-post-settings}

[!DNL Facebook] で他のユーザーがあなたを共有するときに投稿をカスタマイズします。

>[!AVAILABILITY]
>
>すべての Marketo Engage ユーザがこの機能を購入しているわけではありません。詳しくは、アドビのアカウントチーム（担当のアカウントマネージャー）にお問い合わせください。

Marketo の&#x200B;_ソーシャルアプリ_&#x200B;を使用すると、リードが Facebook や Twitter などのソーシャルネットワーク上のつながりを利用して、ランディングページを共有できるようになります。Facebook の OpenGraph タグ（OG タグ）を指定すると、ランディングページのどの情報を Facebook の投稿に含めるかを指定できます。

## リッチ投稿オプションの選択 {#select-rich-post-options}

ランディングページの共有で生成される [!DNL Facebook] しいリッチ投稿で使用するページ情報のタイプを指定できます。

1. ***[!UICONTROL ビデオまたはソーシャルボタンのエディターで]** Facebook メッセージ *[!DNL YouTube*]*」を選択します。

   ![](assets/image2014-9-22-16-3a47-3a21.png)

1. [!DNL Facebook] メッセージに対して次のオプションから選択します。

   * 静的コンテンツの追加：タイトル、キャプション、説明を手動で入力するには、このオプションを選択します。

   ![](assets/image2014-9-22-16-3a48-3a0.png)

   * 動的コンテンツの追加：ソーシャルアプリでは、ランディングページの `<TITLE>`、`<CAPTION>` および `<DESCRIPTION>` タグを使用して、リッチ投稿を生成できます。

   ![](assets/image2014-9-22-16-3a48-3a9.png)

   >[!NOTE]
   >
   >これらは既にページソースに存在しているはずですが、より詳細に制御するには、ランディングページに特定の [!DNL Facebook] OG タグを追加します。

   * リッチコンテンツを追加しない：ランディングページからの [!DNL Facebook] 投稿をメインメッセージとリンクのみに制限します。

   ![](assets/image2014-9-22-16-3a48-3a18.png)

## ランディングページへの [!DNL Facebook] OG タグの追加 {#add-facebook-og-tags-to-a-landing-page}

ランディングページから [!DNL Facebook] 共有に含めるページ要素を制御するには、タイトル、キャプション、説明の OG （グラフを開く）タグ [!DNL Facebook] ランディングページに追加します。

1. **[!DNL YouTube]ビデオ** またはソーシャルボタンを含むランディングページを開きます。

   ![](assets/image2014-9-22-16-3a51-3a28.png)

   **[!UICONTROL ランディングページデザイナー]**&#x200B;が新しいウィンドウで開きます。

1. **[!UICONTROL ランディングページのアクション]**／**[!UICONTROL ページメタタグを編集]**&#x200B;を選択します。

   ![](assets/image2014-9-22-16-3a51-3a36.png)

1. og:title、og:caption、og:description を定義するHTMLを追加します。 次の行をコピー＆ペーストして、プレースホルダーテキストを置き換えます。

   `<meta property="og:title" content="My Post Title"/>`

   `<meta property="og:caption" content="My Post Caption"/>`

   `<meta property="og:description" content="This text appears in the post description"/>`

   ![](assets/image2014-9-22-16-3a52-3a8.png)

>[!NOTE]
>
>OG タグを追加する際は、適切な HTML 構文を使用するように注意してください。
