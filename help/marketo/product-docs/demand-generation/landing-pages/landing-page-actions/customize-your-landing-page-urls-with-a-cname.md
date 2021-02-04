---
unique-page-id: 2359746
description: CNAMEを使用したランディングページURLのカスタマイズ — Marketto Docs — 製品ドキュメント
title: CNAMEを使用したランディングページURLのカスタマイズ
translation-type: tm+mt
source-git-commit: 2969e6f94f5fd781e2167ae2aa8680bb8d134754
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 0%

---


# CNAME {#customize-your-landing-page-urls-with-a-cname}でランディングページURLをカスタマイズする

Marketoがランディングページをホストしている場合でも、URLは完全にカスタマイズできます。 CNAMEを使用しない場合の外観：

`http://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html`

表示方法：

`http://go.YourCompany.com/UnsubscribePage.html`

## CNAMEを選択{#choose-a-cname}

ランディングページのURLの先頭に移動する単語を選択します。 単語は1つで、比較的短くする必要があります。 例：

* go.YourCompany.com/NameOfPage.html
* info.YourCompany.com/NameOfPage.html
* pages.YourCompany.com/NameOfPage.html

「(plus YourCompany.com)」という単語は「CNAME」と呼ばれます。 後で必要になるので、メモしておいてください。

## アカウント文字列{#find-your-account-string}を探します。

1. **管理者**&#x200B;領域に移動し、**ランディングページ**&#x200B;をクリックします。

   ![](assets/image2014-9-18-16-3a2-3a45.png)

   >[!NOTE]
   >
   >**必要な管理者権限**

1. 「**ランディング****ページ**」タブの下で、**アカウント** **文字列**&#x200B;を&#x200B;**設定**&#x200B;セクションからコピーします。

   ![](assets/image2014-9-18-16-3a44-3a12.png)

1. あとで必要になるので、メモしておいてください。

## リクエストをITに送信{#send-request-to-it}

ITスタッフに次のCNAMEを設定するよう依頼します。（「[CNAME]」と「[ACCOUNT STRING]」という語を前の手順のテキストに置き換えます）。

[CNAME].YourCompany.com >  [ACCOUNT STRING].mktoweb.com

## CNAMEの設定{#complete-cname-setup}の完了

1. IT部門がCNAMEを作成したら、**管理者**&#x200B;に移動し、**ランディングページ**&#x200B;をクリックします。

   ![](assets/image2014-9-18-17-3a15-3a11.png)

1. 「**設定**」セクションで、「**編集**」をクリックします。

   ![](assets/image2014-9-18-17-3a15-3a18.png)

1. **ランディングページのドメイン名**&#x200B;にCNAMEを入力し、**フォールバックページ**&#x200B;を入力します。**ホームページ**&#x200B;を入力して、**保存**&#x200B;をクリックします。

   ![](assets/image2014-9-18-17-3a15-3a25.png)

>[!NOTE]
>
>フォールバックページは、Marketorランディングページが利用できない場合、ページのリードがリダイレクトされます。

いい仕事！ これで、ランディングページに会社ドメインのブランドが付けられました。
