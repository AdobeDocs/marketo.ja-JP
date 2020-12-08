---
unique-page-id: 2360189
description: CNAMEを使用したランディングページURLのカスタマイズ（管理） - Marketto Docs — 製品ドキュメント
title: CNAMEを使用したランディングページURLのカスタマイズ（管理）
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---


# CNAMEを使用したランディングページURLのカスタマイズ（管理） {#customize-your-landing-page-urls-with-a-cname-administration}

Marketoがランディングページをホストしている場合でも、URLは会社に合わせてカスタマイズする必要があります。

>[!NOTE]
>
>**例**
>
>No CNAME:
>
>http://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html
>
>ブランドCNAME:
>
>http://go **YourCompany**.com/UnsuscribePage.html

>[!NOTE]
>
>**必要な管理者権限**

お前の準備を！

1. CNAMEの選択

   URLの前の部分です。 例：

   * **go**.YourCompany.com/NameOfPage.html
   * **info**.YourCompany.com/NameOfPage.html
   * **pages**.YourCompany.com/NameOfPage.html

   「(plus YourCompany.com)」という単語は「CNAME」と呼ばれます。 後で必要になるので、メモしてください。

1. アカウント文字列の検索
1. 「 **管理者** 」領域に移動し、「 **ランディングページ」をクリックします**。

   ![](assets/image2014-9-16-13-3a9-3a44.png)

1. 「**ランディングページ**」タブで、「設定」セクションから「アカウント文字列」をコピーします。

   ![](assets/image2014-9-16-13-3a9-3a57.png)

1. 後で必要になる場合もありますので、メモしてください。
1. リクエストをITに送信
1. ITスタッフに次のCNAMEを設定するように依頼します(「 [CNAME] 」と「 [ACCOUNT STRING] 」という単語を前の手順のテキストに置き換えます)。

   [CNAME].YourCompany.com > [ACCOUNT STRING].mktoweb.com

1. CNAMEの設定の完了
1. IT部門がCNAMEを作成したら、「 **管理者** 」に移動し、「 **ランディングページ**」をクリックします。

   ![](assets/image2014-9-16-13-3a10-3a14.png)

1. 「 **設定** 」セクションで、「 **編集**」をクリックします。

   ![](assets/image2014-9-16-13-3a10-3a31.png)

1. ランディングページの **ドメイン名にCNAMEを入力し、**&#x200B;フォールバックページを入力し **、ホームページを入力して、「**&#x200B;保存 **」をクリックし******&#x200B;ます。

   ![](assets/image2014-9-16-13-3a10-3a45.png)

   フォールバックページとは、Marketoランディングページが利用できない場合にユーザーがリダイレクトされるページです。
いい仕事！ これで、ランディングページに会社ドメインのブランドが付けられました。

