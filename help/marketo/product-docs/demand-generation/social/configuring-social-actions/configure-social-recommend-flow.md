---
unique-page-id: 2950549
description: ソーシャル推奨フローの設定 - Marketo ドキュメント - 製品ドキュメント
title: ソーシャル推奨フローの設定
exl-id: 01b54215-4a0c-4639-80d2-ec30603b3695
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '515'
ht-degree: 100%

---

# ソーシャル推奨フローの設定 {#configure-social-recommend-flow}

ソーシャルアプリを作成する際、ユーザーが新規登録すると表示されるソーシャルネットワークの選択肢とプロンプトを設定できます。

## 共有するネットワークの選択 {#select-networks-for-sharing}

>[!NOTE]
>
>これは、[ソーシャル新規登録／共有フローの設定](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/configure-social-sign-up-share-flow.md)に非常に似ていますが、ソーシャルアプリ&#x200B;_の_&#x200B;共有リンク用です。

1. **マーケティングアクティビティ**&#x200B;に移動します。

   ![](assets/login-marketing-activities-1.png)

1. アプリを選択し、「**ドラフトを編集**」をクリックします。

   ![](assets/image2014-9-22-11-3a51-3a6.png)

1. ソーシャルアプリエディターで、**フローを推奨**／**ソーシャルネットワーク**&#x200B;に移動します。

   ![](assets/recommendedflow.png)

1. ユーザーが共有できるネットワークを選択します。

   ![](assets/socialnetworkschoose.png)

## Facebook メッセージの設定 {#configure-the-facebook-message}

1. Facebook の投稿に表示するメッセージを設定します。

   ![](assets/image2014-9-22-11-3a53-3a21.png)

   >[!NOTE]
   >
   >ビデオ共有では、サムネールが自動的に生成されます。

   「**動的コンテンツを追加**」を選択すると、ページの OpenGraph タグ（og:title、og:caption、および og:description）の値とサムネールが Facebook の投稿に自動で追加されます。次の手順を参照してください。

   「**静的コンテンツを追加**」を選択した場合は、タイトル、キャプションおよび説明を入力し、画像をアップロードします。次の 2 つの手順を参照してください。

1. 表示と編集ウィンドウで、「**編集内容を表示**」をクリックし、Facebook の投稿に表示される共有プロンプトとメッセージをカスタマイズします。

   >[!TIP]
   >
   >詳しくは、[Facebook のリッチ投稿設定の編集](/help/marketo/product-docs/demand-generation/facebook/edit-facebook-rich-post-settings.md)を参照してください。

   ![](assets/image2014-9-22-11-3a54-3a36.png)

   >[!NOTE]
   >
   >[共有 URL](/help/marketo/product-docs/demand-generation/social/social-functions/choose-the-share-url-for-a-social-app.md) は、すべての共有メッセージに自動的に追加されます。

1. 上記の「**静的コンテンツを追加**」を選択した場合は、タイトル、キャプションおよび説明を編集し、カスタム画像を（Marketo の画像とファイルから）アップロードします。

   ![](assets/image2014-9-22-11-3a55-3a14.png)

   [Marketo への画像とファイルの追加](/help/marketo/product-docs/demand-generation/images-and-files/add-images-and-files-to-marketo.md)を参照してください。

   >[!NOTE]
   >
   >画像をアップロードすると、ソーシャルアプリエディターを閉じて再度開くまで、ここには表示されません。

1. 「**次へ**」をクリックします。

ページの OpenGraph タグ（og:title、og:caption および og:description）の値を選択すると、サムネールが Facebook の投稿に自動的に追加されます。次の手順を参照してください。

## Twitter メッセージの設定 {#configure-the-twitter-message}

1. クリックして、Twitter のツイートに表示される共有プロンプトとメッセージを編集します。

   ![](assets/image2014-9-22-12-3a2-3a40.png)

   >[!TIP]
   >
   >ツイートのテキストに {html_title} を使用すると、ページのタイトルが自動的に表示されます。

1. 「**次へ**」をクリックします。

## LinkedIn メッセージの設定 {#configure-the-linkedin-message}

1. LinkedIn の投稿に表示するメッセージを設定します。

   ![](assets/image2014-9-22-12-3a3-3a21.png)

   「**動的コンテンツを追加**」を選択すると、ページタグ（タイトルと説明）の値とサムネールが LinkedIn の投稿に自動で追加されます。次の手順を参照してください。

   「****&#x200B;静的コンテンツを追加」を選択した場合は、タイトル、キャプションおよび説明を入力し、画像をアップロードします。次の 2 つの手順を参照してください。

1. **表示と編集**&#x200B;ウィンドウで、「**編集内容を表示**」をクリックし、LinkedIn の投稿に表示される共有プロンプトとメッセージを編集します。

   ![](assets/image2014-9-22-12-3a3-3a38.png)

   >[!TIP]
   >
   >投稿のテキストで {html_title} を使用して、ページのタイトルを自動的に表示します。

1. 上記の「**静的コンテンツを追加**」を選択した場合はタイトルおよび説明を編集し、カスタム画像を（Marketo の画像とファイルから）アップロードします。

   ![](assets/image2014-9-22-12-3a4-3a43.png)

   [Marketo への画像とファイルの追加](/help/marketo/product-docs/demand-generation/images-and-files/add-images-and-files-to-marketo.md)を参照してください。

   >[!NOTE]
   >
   >画像をアップロードすると、ソーシャルアプリエディターを閉じて再度開くまで、ここには表示されません。

1. 「**次へ**」をクリックします。

## 確認メッセージの設定 {#configure-the-confirmation-message}

1. 共有を確認するテキストを編集します。

   ![](assets/image2014-9-22-12-3a5-3a30.png)

1. **完了** ／**承認**&#x200B;をクリックして、「**閉じる**」をクリックします。

   ![](assets/image2014-9-22-12-3a5-3a45.png)

>[!MORELIKETHIS]
>
>次に、ランディングページ、Facebook、独自の Web サイトに[動画共有](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-video-share-flow.md)または[投票](/help/marketo/product-docs/demand-generation/social/creating-a-poll/create-a-poll.md)を追加します。
