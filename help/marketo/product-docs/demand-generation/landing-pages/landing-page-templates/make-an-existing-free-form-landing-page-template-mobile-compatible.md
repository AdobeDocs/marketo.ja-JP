---
unique-page-id: 5472348
description: 既存のフリーフォームランディングページテンプレートとモバイルとの互換性の確保 —Marketoドキュメント — 製品ドキュメント
title: 既存のフリーフォームランディングページテンプレートとモバイルとの互換性の設定
exl-id: 942456a5-3f3e-4a71-aecc-4cc6bf6237b3
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '251'
ht-degree: 0%

---

# 既存のフリーフォームランディングページテンプレートとモバイルとの互換性の設定{#make-an-existing-free-form-landing-page-template-mobile-compatible}

これは、ランディングページエディターとテンプレートエディターの2か所で行うことができます。

## テンプレートエディターからのアップグレード{#upgrade-from-the-template-editor}

1. **Design Studio**&#x200B;に移動します。

   ![](assets/designstudio-1.png)

1. 「**テンプレート**」を選択します。

   ![](assets/image2015-1-22-20-3a20-3a2.png)

1. **モバイル互換**&#x200B;が&#x200B;**なし**&#x200B;であるテンプレートを選択します。

   ![](assets/image2015-1-22-20-3a22-3a24.png)

1. 「**ドラフトを編集**」をクリックします。

   ![](assets/image2015-1-22-20-3a25-3a36.png)

1. 「**モバイルと互換性を持たせる**」をクリックします。

   ![](assets/image2015-1-22-20-3a30-3a33.png)

1. 「**アップグレード**」をクリックします。

   ![](assets/image2015-1-22-20-3a32-3a45.png)

   ランディングページテンプレートはモバイルとの互換性が確保されました。

   >[!NOTE]
   >
   >アップグレードは安全ですが、ページに食い違いがないかどうかを確認してください。 アップグレードすると、そのテンプレートを使用するランディングページのドラフトが作成されます。

   ![](assets/image2015-1-22-20-3a36-3a43.png)

## テンプレートモバイルとの互換性{#what-makes-a-template-mobile-compatible}

素晴らしい質問です！ テンプレートには次のタグが必要です。

`<pre data-theme="Confluence">Must have <!DOCTYPE HTML> Must have a <HEAD> element Must have a <TITLE> in the <HEAD> element Must have <META CHARSET="UTF-8"> within the <HEAD> element Must have a <BODY> element that contains one (and only one) <DIV class="mktoContent"></DIV></pre>`

問題がない場合は、次のメッセージが表示されます。

![](assets/image2015-1-22-20-3a41-3a31.png)

問題が発生した場合は、エラーメッセージが表示されます。「修復」をクリックして問題を修正し、検証プロセスを繰り返します。

![](assets/image2015-1-22-20-3a43-3a20.png)

テンプレートに変更を加えた場合は、「テンプレートのアクション」をクリックし、「モバイルの互換性を検証」を選択します。

## フリーフォームランディングページエディタからのテンプレートのアップグレード{#upgrading-a-template-from-the-free-form-landing-page-editor}

ランディングページを編集中に「モバイル」タブをクリックすると、テンプレートがアップグレードされていないことに気付く場合があります。 恐れない！ アップグレードは、すぐに行えます。

1. 「**モバイル**」タブをクリックします。

   ![](assets/image2015-1-22-20-3a48-3a19.png)

1. チェックボックスをクリックし、「**アクティブ化**」をクリックします。

   ![](assets/image2015-1-22-20-3a49-3a34.png)

   >[!NOTE]
   >
   >モバイルバージョンのテンプレートをアクティブ化すると、それを使用するランディングページのドラフトが作成されます。

やりましたね！これで、このテンプレートを使用するすべてのランディングページのモバイル表示](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/customize-mobile-view-for-your-free-form-landing-page.md)を[カスタマイズできます。
