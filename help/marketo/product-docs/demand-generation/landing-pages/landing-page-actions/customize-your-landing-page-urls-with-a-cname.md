---
unique-page-id: 2359746
description: CNAME を使用したランディングページ URL のカスタマイズ - Marketo ドキュメント - 製品ドキュメント
title: CNAME を使用したランディングページ URL のカスタマイズ
exl-id: 2cd87785-61e5-46cd-b1e0-6fbc145014d4
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '254'
ht-degree: 100%

---

# CNAME を使用したランディングページ URL のカスタマイズ {#customize-your-landing-page-urls-with-a-cname}

Marketo がランディングページをホストしている場合でも、URL は完全にカスタマイズできます。CNAME がない場合の外観は次のとおりです。

`https://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html`

表示方法：

`https://go.YourCompany.com/UnsubscribePage.html`

## CNAME を選択する {#choose-a-cname}

ランディングページの URL の先頭に移動する単語を選択します。単語は 1 つだけで、比較的短くする必要があります。例:

* go.YourCompany.com/NameOfPage.html
* info.YourCompany.com/NameOfPage.html
* pages.YourCompany.com/NameOfPage.html

1 つの単語（plus YourCompany.com）が CNAME と呼ばれます。後で必要になるので、覚えておいてください。

## アカウント文字列を検索する {#find-your-account-string}

1. **管理**&#x200B;領域に移動して、「**ランディングページ**」をクリックします。

   ![](assets/image2014-9-18-16-3a2-3a45.png)

   >[!NOTE]
   >
   >**管理者権限が必要**

1. 「**ランディング****ページ**」タブで、**アカウント****文字列**&#x200B;を&#x200B;**設定**&#x200B;セクションからコピーします。

   ![](assets/image2014-9-18-16-3a44-3a12.png)

1. 後でも必要になるので、覚えておいてください。

## IT にリクエストを送信する {#send-request-to-it}

次の CNAME を設定するよう IT スタッフに依頼します（[CNAME] および [ACCOUNT STRING] を前の手順のテキストで置き換える）。

[CNAME].YourCompany.com > [ACCOUNT STRING].mktoweb.com

## CNAME 設定を完了する {#complete-cname-setup}

1. IT で CNAME が作成されたら、**管理者**&#x200B;に移動して、「**ランディングページ**」をクリックします。

   ![](assets/image2014-9-18-17-3a15-3a11.png)

1. **設定**&#x200B;セクションで、「**編集**」をクリックします。

   ![](assets/image2014-9-18-17-3a15-3a18.png)

1. 「**ランディングページのドメイン名**」に CNAME を入力します。**フォールバックページ**&#x200B;と&#x200B;**ホームページ**&#x200B;を入力して、「**保存**」をクリックします。

   ![](assets/image2014-9-18-17-3a15-3a25.png)

>[!NOTE]
>
>Marketo ランディングページを使用できない場合、フォールバックページにリダイレクトされます。

これで完了です。ランディングページが会社のドメインでブランディングされました。
