---
unique-page-id: 2359798
description: 付加的なランディングページ CNAME の追加 - Marketo ドキュメント - 製品ドキュメント
title: 付加的なランディングページ CNAME の追加
exl-id: eb5a7f69-552e-49a2-91db-a784f4639cd0
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 100%

---

# 付加的なランディングページ CNAME の追加 {#add-additional-landing-page-cnames}

様々な URL で Marketo のランディングページを指すように、ランディングページの CNAME を追加することができます。次の手順に従うと、複数のドメインを管理するのに役立ちます。

>[!CAUTION]
>
>Cookie は、ドメイン間で共有できません。

>[!TIP]
>
>**同じトップレベルドメイン — 可能Cookie が共有されます**.<br/> **go**.mycompany.com > **info**.mycompany.com
>
>**異なるトップレベルドメイン — 不可能cookie は共有&#x200B;_されません。_**<br/> go.**mycompany**.com > go.**mynewcompany**.com

>[!NOTE]
>
>**管理者権限が必要**

## アカウント文字列を検索 {#find-your-account-string}

1. **管理者**&#x200B;セクションに移動して、「**ランディングページ**」をクリックします。

   ![](assets/image2014-9-16-15-3a19-3a54.png)

1. **アカウント文字列**&#x200B;を&#x200B;**設定**&#x200B;セクションからコピーします。

   ![](assets/image2014-9-16-15-3a20-3a2.png)

1. 次の手順でメモしておきます。

## IT にリクエストを送信する {#send-request-to-it}

1. 担当の IT 部門に、次の CNAME を設定するよう依頼します（[CNAME] を希望する CNAME で置き換え、[ACCOUNT STRING] を前の手順のテキストで置き換えます)。

   [CNAME].YourCompany.com > [ACCOUNT STRING].mktoweb.com

## 新しい CNAME を追加する {#add-a-new-cname}

1. IT 部門が CNAME を作成したら、**管理者**&#x200B;に移動して、「**ランディングページ**」をクリックします。

   ![](assets/image2014-9-16-15-3a20-3a20.png)

1. 「**新規**」をクリックして、「**新規ドメインエイリアス**」を選択します。

   ![](assets/image2014-9-16-15-3a20-3a28.png)

1. **ドメインエイリアス**&#x200B;を入力します。訪問者が URL を入力しない場合、**デフォルトのページ**&#x200B;が表示されます。その場合の移動先を入力します。

   >[!NOTE]
   >
   >デフォルトページの場合は、ランディングページまたは公開 Web サイトなどの外部 URL を選択できます。

   ![](assets/image2014-9-16-15-3a20-3a36.png)

1. **デフォルトページ**&#x200B;を入力して、「**作成**」をクリックします。

   ![](assets/image2014-9-16-15-3a20-3a43.png)

作業は以上です。これで、CNAME を追加したい場合の対処方法を理解できました。
