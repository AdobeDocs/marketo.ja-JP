---
unique-page-id: 5472348
description: 既存の自由形式ランディングページテンプレートをモバイル対応にする方法について説明します。 テンプレートエディターまたはランディングページエディターからアップグレードします。
title: 既存のフリーフォームランディングページテンプレートのモバイルとの互換性の確保
exl-id: 942456a5-3f3e-4a71-aecc-4cc6bf6237b3
feature: Landing Pages
TQID: https://experienceleague.adobe.com/-EJdlRrUIvCn6r4P6LGvZbyAyBy1K3HJms38fW2VKnE
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: d65b4a73-87a3-4d56-b638-74e74d9939ce
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
source-git-commit: b2861922f7d2732a3286bab93243bdc0515a5995
workflow-type: tm+mt
source-wordcount: 259
ht-degree: 74%

---

# 既存のフリーフォームランディングページテンプレートのモバイルとの互換性の確保 {#make-an-existing-free-form-landing-page-template-mobile-compatible}

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
   >アップグレードは安全ですが、ページに食い違いがないかを確認してください。 アップグレードすると、そのテンプレートを使用するすべてのランディングページのドラフトが作成されます。

   ![](assets/image2015-1-22-20-3a36-3a43.png)

## テンプレートを[!UICONTROL モバイルに対応]させる理由は何ですか？ {#what-makes-a-template-mobile-compatible}

テンプレートには次のタグが必要です。

```
Must have <!DOCTYPE HTML> 
Must have a <HEAD> element 
Must have a <TITLE> in the <HEAD> element 
Must have <META CHARSET="UTF-8"> within the <HEAD> element 
Must have a <BODY> element that contains one (and only one) <DIV class="mktoContent"></DIV>
```

問題がない場合は、次のメッセージが表示されます。

![](assets/image2015-1-22-20-3a41-3a31.png)

問題が発生した場合は、エラーメッセージが表示され、「修復」をクリックして問題を修正し、検証プロセスを繰り返します。

![](assets/image2015-1-22-20-3a43-3a20.png)

テンプレートに変更を加える場合は、**[!UICONTROL テンプレートアクション]**&#x200B;をクリックし、**[!UICONTROL モバイル互換性の検証]**&#x200B;を選択します。

## フリーフォームランディングページエディターからのテンプレートのアップグレード {#upgrading-a-template-from-the-free-form-landing-page-editor}

ランディングページを編集する際に「モバイル」タブをクリックすると、テンプレートがアップグレードされていないことがあります。 大丈夫です。 すぐにアップグレードできます。

1. 「**[!UICONTROL モバイル]**」タブをクリックします。

   ![](assets/image2015-1-22-20-3a48-3a19.png)

1. チェックボックスをクリックして、「**[!UICONTROL 有効にする]**」をクリックします。

   ![](assets/image2015-1-22-20-3a49-3a34.png)

   >[!NOTE]
   >
   >モバイルバージョンのテンプレートをアクティベートすると、そのテンプレートを使用するランディングページのドラフトが作成されます。

このテンプレートを使用するすべてのランディングページの[モバイル表示をカスタマイズ](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/customize-mobile-view-for-your-free-form-landing-page.md)できます。
