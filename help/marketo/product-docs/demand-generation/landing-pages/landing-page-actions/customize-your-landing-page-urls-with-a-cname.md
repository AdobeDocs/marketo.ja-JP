---
unique-page-id: 2359746
description: CNAMEを使用したランディングページURLのカスタマイズ — Marketto Docs — 製品ドキュメント
title: CNAMEを使用したランディングページURLのカスタマイズ
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---


# CNAMEを使用したランディングページURLのカスタマイズ {#customize-your-landing-page-urls-with-a-cname}

Marketoがランディングページをホストしている場合でも、URLは完全にカスタマイズできます。 CNAMEを使用しない場合の外観：`<pre data-theme="Confluence">http://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html</pre>` 表示方法：
`<pre data-theme="Confluence"> http://go.YourCompany.com/UnsubscribePage.html</pre>`

## CNAMEの選択 {#choose-a-cname}

ランディングページのURLの先頭に移動する単語を選択します。 単語は1つで、比較的短くする必要があります。 例：

* 行け。 [YourCompany.com/NameOfPage.html](http://YourCompany.com/NameOfPage.html)
* 情報 [YourCompany.com/NameOfPage.html](http://YourCompany.com/NameOfPage.html)
* ページ、 [YourCompany.com/NameOfPage.html](http://YourCompany.com/NameOfPage.html)

1つ目の単語(plus [YourCompany.com](http://YourCompany.com))はCNAMEと呼ばれます。 後で必要になるので、メモしてください。

## アカウント文字列の検索 {#find-your-account-string}

1. 「 **管理者** 」領域に移動し、「 **ランディングページ」をクリックします。**

   ![](assets/image2014-9-18-16-3a2-3a45.png)

   >[!NOTE]
   >
   >**必要な管理者権限**

1. 「 **Landing** Pages **(ランディング** ページ **)」タブの下で、「Account String（アカウント文字列）」を「Settings（設定）」セクション********** からコピーします。

   ![](assets/image2014-9-18-16-3a44-3a12.png)

1. あとで必要になるので、メモしておいてください。

## リクエストをITに送信 {#send-request-to-it}

ITスタッフに次のCNAMEを設定するよう依頼します。(「 [CNAME] 」と「 [ACCOUNT STRING] 」という語を前の手順のテキストに置き換えます)。

[CNAME]。 [YourCompany.com](http://yourcompany.com/) / [ACCOUNT STRING]。 [mktoweb.com](http://mktoweb.com/)

## CNAMEの設定の完了 {#complete-cname-setup}

1. IT部門がCNAMEを作成したら、「 **管理者** 」に移動し、「 **ランディング** ページ ****」をクリックします。

   ![](assets/image2014-9-18-17-3a15-3a11.png)

1. 「 **設定** 」セクションで、「 **編集**」をクリックします。

   ![](assets/image2014-9-18-17-3a15-3a18.png)

1. CNAMEを **ドメイン名** 名 **** 名 **に** 入力し **ます。** CNAMEの ********************&#x200B;名前名前に入力します。

   ![](assets/image2014-9-18-17-3a15-3a25.png)

>[!NOTE]
>
>フォールバックページは、Marketorランディングページが利用できない場合、ページのリードがリダイレクトされます。

いい仕事！ これで、ランディングページに会社ドメインのブランドが付けられました。