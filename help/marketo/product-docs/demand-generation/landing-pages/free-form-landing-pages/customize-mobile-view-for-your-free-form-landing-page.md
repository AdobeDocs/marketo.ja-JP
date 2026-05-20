---
unique-page-id: 5472283
description: Marketoでフリーフォームのランディングページのモバイルビューをカスタマイズする方法について説明します。 モバイル訪問者のレイアウトとコンテンツを調整します。
title: フリーフォームランディングページのモバイル表示をカスタマイズする
exl-id: 8a5b3d81-34b1-47be-9575-d5ab61cdf9e4
feature: Landing Pages
TQID: https://experienceleague.adobe.com/RJiOHLIXxHZdZBJk2XtIqk6TtJ7UVjcExmkxyVFp3yQ
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b0bb9048-d951-48d8-8232-45cf248a7e27id: f82558ea-6af5-44eb-a424-5b3389abb0a3
source-git-commit: b2861922f7d2732a3286bab93243bdc0515a5995
workflow-type: tm+mt
source-wordcount: 378
ht-degree: 84%

---

# フリーフォームランディングページのモバイル表示をカスタマイズする {#customize-mobile-view-for-your-free-form-landing-page}

>[!PREREQUISITES]
>
>[フリーフォームランディングページのモバイル表示の追加](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/add-a-mobile-view-for-your-free-form-landing-page.md)

フリーフォームランディングページのモバイル表示は、ほとんど自動ですが、カスタマイズできます。

1. フリーフォームランディングページを選択します。

   ![](assets/selectlandingapge.jpg)

1. **[!UICONTROL ドラフトの編集]**&#x200B;をクリックします。

   ![](assets/image2015-1-22-18-3a33-3a12.png)

1. 「**[!UICONTROL モバイル]**」タブをクリックします。

   ![](assets/image2015-1-22-18-3a31-3a40.png)

## モバイル表示とデスクトップ表示+ {#mobile-vs-desktop-view}

ページ要素の下に、![](assets/image2015-1-22-18-3a39-3a53.png)（デスクトップ）アイコンと![](assets/image2015-1-22-18-3a40-3a31.png)（モバイル）アイコンがあります。 これにより、様々な要素の表示／非表示を動的に切り替えることができます。

![](assets/image2015-5-21-15-3a9-3a34.png)

デフォルトでは、デスクトップ表示のすべての項目がモバイル表示に表示されます。

>[!NOTE]
>
>長方形は、モバイルビューには表示されません。

![](assets/image2015-5-21-15-3a12-3a2.png)

## 留意事項 {#important-things-to-know}

* 画像はモバイルデバイスの幅に合わせて拡大されます。 画像を小さくしたい場合は、リッチテキスト要素を取り込み、そこから画像を追加します。
* Forms 2.0 フォームのみを使用してください。 これらはレスポンシブで、自動的に調整されます。
* 編集可能なテンプレート要素は 1 つだけです（BODY#bodyid (Mobile)）。 これを使用して、背景色を変更できます。

  ![](assets/image2015-5-21-15-3a15-3a47.png)

## モバイル表示から要素を非表示にする {#hide-an-element-from-the-mobile-view}

>[!TIP]
>
>携帯電話では少ないほうが効果的です。

1. 要素を非表示にするには、モバイル列の下にある、対応するチェックボックスをクリックします。

   ![](assets/image2015-5-21-15-3a28-3a17.png)

1. その要素は、モバイル表示には表示されなくなります。

   ![](assets/image2015-5-21-15-3a30-3a17.png)

## モバイル表示に要素を追加する {#add-an-element-to-the-mobile-view}

>[!TIP]
>
>モバイルビュー用に短いコンテンツを作成します。

1. 要素を追加するには、フリーフォームランディングページに要素をドラッグ&amp;ドロップします。

   ![](assets/image2015-5-21-15-3a32-3a22.png)

   要素がモバイル表示でのみ表示されるように設定されていることを確認します。

   ![](assets/image2015-5-21-15-3a35-3a29.png)

>[!TIP]
>
>モバイル表示でページ要素の配置を変更することもできます。 フリーフォームランディングページ上で移動するか、ドラッグ&amp;ドロップを使用して&#x200B;**[!UICONTROL ページ要素]**&#x200B;に表示されているオブジェクトを並べ替えます。

## モバイル表示をプレビュー {#preview-mobile-view}

1. 「**[!UICONTROL 下書きをプレビュー]**」をクリックします。

   ![](assets/image2015-5-21-15-3a36-3a35.png)

1. **[!UICONTROL Side By Side]**&#x200B;を選択すると、デスクトップ版とモバイル版を同時に比較できます。

   ![](assets/image2015-1-22-20-3a2-3a15.png)

1. ランディングページのデスクトップ版とモバイル版を同時に表示できるようになりました。

   ![](assets/image2015-1-22-20-3a3-3a22.png)

1. 「**[!UICONTROL 承認して閉じる]**」をクリックします。

   ![](assets/image2015-1-22-20-3a5-3a36.png)

   >[!NOTE]
   >
   >プレビューはインタラクティブではありません。 スマートフォンの表示は、それぞれ少し異なります。 ランディングページがどのように動作するかを正確に確認するには、いくつかのデバイスでランディングページをプレビューすることをお勧めします。


>[!MORELIKETHIS]
>
>[既存のフリーフォームランディングページテンプレートのモバイルとの互換性の確保](/help/marketo/product-docs/demand-generation/landing-pages/landing-page-templates/make-an-existing-free-form-landing-page-template-mobile-compatible.md)
