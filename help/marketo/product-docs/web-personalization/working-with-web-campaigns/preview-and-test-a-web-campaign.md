---
unique-page-id: 10092925
description: Web キャンペーンのプレビューとテスト - Marketo ドキュメント - 製品ドキュメント
title: Web キャンペーンのプレビューとテスト
exl-id: 6cc4ebd8-0d39-4a7d-bc3d-e8cd18157470
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 100%

---

# Web キャンペーンのプレビューとテスト {#preview-and-test-a-web-campaign}

この記事では、web キャンペーンの様々なプレビュー方法と、ウェブサイト上にあるサンドボックスセグメントを使用してキャンペーンをテストする方法について説明します。

>[!NOTE]
>
>プレビューは、選択したサイトでのキャンペーンの表示のみを示します。分析での誤ったクリック数や表示数を防ぐため、リンクとウィジェットは機能しなくなります。

## Web キャンペーンの作成ページでのプレビュー {#preview-a-web-campaign-on-the-creation-page}

1. 「**[!UICONTROL Web キャンペーン]**」に移動します。

   ![](assets/image2016-8-18-15-3a59-3a35.png)

1. 「**[!UICONTROL Web キャンペーンを新規作成]**」または既存のキャンペーンを編集するアイコンをクリックします。

   ![](assets/create-new-or-edit-web-campaign.png)

1. 「サイトでのプレビュー」で、ページの URL を追加し、「**[!UICONTROL プレビュー]**」をクリックします。新しいウィンドウまたはタブが開き、キャンペーンのプレビューが表示されます。

   ![](assets/three-1.png)

   >[!TIP]
   >
   >「**[!UICONTROL 共有]**」をクリックして、キャンペーンプレビューの固定 URL を持つメールを開きます。

   >[!NOTE]
   >
   >また、キャンペーンをプレビューする際のエクスペリエンスを最大限に高めるには、ブラウザープラグイン（[[!DNL Chrome]](https://chrome.google.com/webstore/detail/marketo-web-personalizati/ldiddonjplchallbngbccbfdfeldohkj) または [[!DNL Firefox]](https://rtp-static.marketo.com/rtp/libs/mwp-0.0.0.8.xpi)）をインストールすることもできます。以下の節を参照してください。

## ブラウザープラグインを使用した作成ページでの web キャンペーンのプレビュー {#preview-a-web-campaign-on-the-creation-page-using-the-browser-plug-in}

1. 上記の節の手順 1 および 2 に従います。

1. ブラウザープラグインへのリンクをクリックします（この場合は [!DNL Chrome] を使用）。

   ![](assets/4-1.png)

1. 新しいウィンドウ／タブが開きます。「**[!UICONTROL Chrome に追加]**」をクリックします。

   ![](assets/five.png)

1. 「**[!UICONTROL 拡張機能を追加]**」をクリックします。

   ![](assets/six.png)

1. Marketo に戻ります。ページ URL を追加し、「**[!UICONTROL プレビュー]**」をクリックします。

   ![](assets/seven.png)

1. 新しいウィンドウ／タブが開き、デスクトップ、スマートフォン、タブレットでのキャンペーンの表示をプレビューできます。

   ![](assets/campaign-preview.png)

## Web キャンペーンページでの web キャンペーンのプレビュー {#preview-a-web-campaign-on-the-web-campaigns-page}

1. Web キャンペーンのリストを見る場合は、キャンペーンを選択し、**[!UICONTROL プレビュー]**&#x200B;アイコンをクリックします。

   ![](assets/web-campaigns-1-preview-hand.png)

   簡単です。

## ウェブサイト上での web キャンペーンのプレビュー {#preview-a-web-campaign-on-your-website}

サンドボックスセグメントとキャンペーンを作成します。

1. 「**[!UICONTROL セグメント]**」に移動します。

   ![](assets/new-dropdown-segments-hand.jpg)

1. 「**[!UICONTROL 新規作成]**」をクリックします。

   ![](assets/image2015-9-10-10-3a42-3a39.png)

1. セグメントに名前を付けます。

1. 「[!UICONTROL 行動]」の下で、「[!UICONTROL ページを含める]」をキャンバスにドラッグします。値 &#42;sandbox=1&#42; を追加します。「**[!UICONTROL キャンペーンの保存と定義]**」をクリックします。

   ![](assets/segment.png)

1. Web キャンペーンを設定ページで、リストから選択して、ターゲットセグメントをサンドボックスセグメントに変更します。

   ![](assets/set-web-campaign-target-segment.jpg)

1. キャンペーンのクリエイティブを完了し、「**[!UICONTROL 起動]**」をクリックします。

   ![](assets/click-launch.jpg)

1. ウェブサイトに移動し、URL の末尾に URL パラメーター「?sandbox=1」を追加します。例: `www.marketo.com?sandbox=1`.

1. ウェブサイトでキャンペーンの反応を確認します。

>[!NOTE]
>
>キャンペーンの反応は、訪問者セッション中に 1 回だけ発生します。キャンペーンを再度表示するには、ブラウザーの Cookie を消去します。

>[!NOTE]
>
>リダイレクトキャンペーンをプレビューすることはできません。これらをテストする唯一の方法は、（特定のページでターゲットにする）サンドボックスセグメントを使用することです（&#42;sandbox=redirect&#42;）
