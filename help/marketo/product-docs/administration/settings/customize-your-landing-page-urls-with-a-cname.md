---
unique-page-id: 2360189
description: CNAME を使用したランディングページ URL のカスタマイズ（管理） - Marketo ドキュメント - 製品ドキュメント
title: CNAME を使用したランディングページ URL のカスタマイズ（管理）
exl-id: a5aa1c76-15f7-4e8c-a736-77c79f65c368
source-git-commit: 07899e541b3624e99e0ead59d898ced2ab4e57af
workflow-type: ht
source-wordcount: '249'
ht-degree: 100%

---

# CNAME を使用したランディングページ URL のカスタマイズ  {#customize-your-landing-page-urls-with-a-cname}

Marketo がランディングページをホストしている場合でも、URL は会社向けにカスタマイズする必要があります。

>[!NOTE]
>
>CNAME なし：
>
>https://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html
>
>ブランディング CNAME：
>
>https://go.**YourCompany**.com/UnsuscribePage.html

>[!NOTE]
>
>**管理者権限が必要**

設定してみましょう。

1. CNAME を選択します。

   URL の前の部分です。例:

   * **go**.YourCompany.com/NameOfPage.html
   * **info**.YourCompany.com/NameOfPage.html
   * **pages**.YourCompany.com/NameOfPage.html

   1 つの単語（プラス YourCompany.com）が CNAME と呼ばれます。後で必要になるので、メモしておきます。

1. アカウント文字列を検索します。

1. 「**管理者**」領域に移動します。

   ![](assets/customize-your-landing-page-urls-with-a-cname-1.png)

1. 「**ランディングページ**」をクリックします。

   ![](assets/customize-your-landing-page-urls-with-a-cname-2.png)

1. 「**ランディングページ**」タブで、「設定」セクションから「アカウント文字列」をコピーします。

   ![](assets/customize-your-landing-page-urls-with-a-cname-3.png)

1. これも後で必要になるので、メモしておきます。

1. IT 部門にリクエストを送信します。

1. 次の CNAME を設定するよう IT スタッフに依頼します（[CNAME] および[アカウント文字列]を、前の手順のテキストで置き換えます）：

   [CNAME].YourCompany.com ＞ [アカウント文字列].mktoweb.com

1. CNAME 設定を完了します。

1. IT 部門で CNAME が作成されたら、「**管理者**」領域に戻ります。

   ![](assets/customize-your-landing-page-urls-with-a-cname-4.png)

1. 「**ランディングページ**」をクリックします。

   ![](assets/customize-your-landing-page-urls-with-a-cname-5.png)

1. 「**設定**」セクションで、「**編集**」をクリックします。

   ![](assets/customize-your-landing-page-urls-with-a-cname-6.png)

1. 「**ランディングページのドメイン名**」に CNAME を入力し、「**フォールバックページ**」と「**ホームページ**」を入力し、「**保存**」をクリックします。

   ![](assets/customize-your-landing-page-urls-with-a-cname-7.png)

フォールバックページは、Marketo のランディングページを使用できない場合に、ユーザがリダイレクトされるページです。

これで完了です。ランディングページが会社のドメインでブランディングされました。
