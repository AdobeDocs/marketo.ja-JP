---
unique-page-id: 5472348
description: 既存のフリーフォームランディングページテンプレートのモバイルとの互換性の確保 - Marketo ドキュメント - 製品ドキュメント
title: 既存のフリーフォームランディングページテンプレートのモバイルとの互換性の確保
exl-id: 942456a5-3f3e-4a71-aecc-4cc6bf6237b3
feature: Landing Pages
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '251'
ht-degree: 87%

---

# 既存のフリーフォームのランディングページテンプレートを作成 [!UICONTROL &#x200B; モバイル互換 &#x200B;] {#make-an-existing-free-form-landing-page-template-mobile-compatible}

これは、テンプレートエディターとランディングページエディターの 2 か所でおこなえます。

## テンプレートエディターからのアップグレード {#upgrade-from-the-template-editor}

1. **[!UICONTROL Design Studio]** に移動します。

   ![](assets/designstudio-1.png)

1. 「**[!UICONTROL テンプレート]**」を選択します。

   ![](assets/image2015-1-22-20-3a20-3a2.png)

1. **[!UICONTROL モバイル互換]**&#x200B;が&#x200B;**[!UICONTROL いいえ]**&#x200B;のテンプレートを選択します。

   ![](assets/image2015-1-22-20-3a22-3a24.png)

1. **[!UICONTROL ドラフトの編集]**&#x200B;をクリックします。

   ![](assets/image2015-1-22-20-3a25-3a36.png)

1. 「**[!UICONTROL モバイルに対応させる]**」をクリックします。

   ![](assets/image2015-1-22-20-3a30-3a33.png)

1. 「**[!UICONTROL アップグレード]**」をクリックします。

   ![](assets/image2015-1-22-20-3a32-3a45.png)

   ランディングページテンプレートがモバイルに対応するようになりました。

   >[!NOTE]
   >
   >アップグレードは安全ですが、ページに食い違いがないかを確認してください。アップグレードすると、そのテンプレートを使用するすべてのランディングページのドラフトが作成されます。

   ![](assets/image2015-1-22-20-3a36-3a43.png)

## テンプレート [!UICONTROL &#x200B; モバイル互換 &#x200B;] の理由 {#what-makes-a-template-mobile-compatible}

いい質問です。テンプレートには次のタグが必要です。

`Must have <!DOCTYPE HTML> Must have a <HEAD> element Must have a <TITLE> in the <HEAD> element Must have <META CHARSET="UTF-8"> within the <HEAD> element Must have a <BODY> element that contains one (and only one) <DIV class="mktoContent"></DIV>`

問題がない場合は、次のメッセージが表示されます。

![](assets/image2015-1-22-20-3a41-3a31.png)

問題が発生した場合は、エラーメッセージが表示され、「修復」をクリックして問題を修正し、検証プロセスを繰り返します。

![](assets/image2015-1-22-20-3a43-3a20.png)

テンプレートに変更を加えた場合は、「[!UICONTROL &#x200B; テンプレートアクション &#x200B;]」をクリックし、「[!UICONTROL &#x200B; モバイル互換性を検証 &#x200B;]」を選択します。

## フリーフォームランディングページエディターからのテンプレートのアップグレード {#upgrading-a-template-from-the-free-form-landing-page-editor}

ランディングページを編集して「モバイル」タブをクリックすると、テンプレートがアップグレードされていないことに気付く場合があります。大丈夫です。すぐにアップグレードできます。

1. 「**[!UICONTROL モバイル]**」タブをクリックします。

   ![](assets/image2015-1-22-20-3a48-3a19.png)

1. チェックボックスをクリックして、「**[!UICONTROL 有効にする]**」をクリックします。

   ![](assets/image2015-1-22-20-3a49-3a34.png)

   >[!NOTE]
   >
   >モバイルバージョンのテンプレートをアクティベートすると、そのテンプレートを使用するランディングページのドラフトが作成されます。

これで完了です。このテンプレートを使用するすべてのランディングページの[モバイル表示をカスタマイズ](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/customize-mobile-view-for-your-free-form-landing-page.md)できます。
