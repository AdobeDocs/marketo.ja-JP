---
unique-page-id: 2359746
description: CNAME を使用したランディングページ URL のカスタマイズ - Marketo ドキュメント - 製品ドキュメント
title: CNAME を使用したランディングページ URL のカスタマイズ
exl-id: 2cd87785-61e5-46cd-b1e0-6fbc145014d4
feature: Landing Pages
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: ht
source-wordcount: '237'
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

## Munchkin ID を検索する {#find-your-munchkin-id}

1. 「**管理者**」領域に移動します。

   ![](assets/customize-your-landing-page-urls-with-a-cname-1.png)

1. 「**マイアカウント**」をクリックします。

   ![](assets/customize-your-landing-page-urls-with-a-cname-2.png)

   >[!NOTE]
   >
   >**管理者権限が必要**

1. 「サポート情報」まで下にスクロールし、Munchkin ID をコピーします。

   ![](assets/customize-your-landing-page-urls-with-a-cname-3.png)

## IT にリクエストを送信する {#send-request-to-it}

次の CNAME を設定するよう IT スタッフに依頼します（[CNAME] および [Munchkin ID] を前の手順のテキストで置き換える）。

[CNAME].YourCompany.com／[Munchkin ID].mktoweb.com

## CNAME 設定を完了する {#complete-cname-setup}

1. IT 部門で CNAME が作成されたら、「**管理者**」領域に移動します。

   ![](assets/customize-your-landing-page-urls-with-a-cname-4.png)

1. 「**ランディングページ**」をクリックします。

   ![](assets/customize-your-landing-page-urls-with-a-cname-5.png)

1. 「**設定**」セクションで、「**編集**」をクリックします。

   ![](assets/customize-your-landing-page-urls-with-a-cname-6.png)

1. 「**[!UICONTROL ランディングページのドメイン名]**」に CNAME を入力します。**[!UICONTROL フォールバックページ]**&#x200B;と&#x200B;**[!UICONTROL ホームページ]**&#x200B;を入力して、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/customize-your-landing-page-urls-with-a-cname-7.png)

>[!NOTE]
>
>Marketo ランディングページを使用できない場合、フォールバックページにリダイレクトされます。

これで完了です。ランディングページが会社のドメインでブランディングされました。
