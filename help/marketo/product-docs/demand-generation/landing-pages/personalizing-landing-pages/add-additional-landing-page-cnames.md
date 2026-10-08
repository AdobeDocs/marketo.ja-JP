---
unique-page-id: 2359798
description: Marketoでランディングページ CNAMEを追加する方法について説明します。 ランディングページには、複数のカスタムドメインを使用できます。
title: 追加のランディングページ CNAME の追加
exl-id: eb5a7f69-552e-49a2-91db-a784f4639cd0
feature: Landing Pages
TQID: 'https://experienceleague.adobe.com/IhpbLwq0syIQpnKsRApy6YtEKhe56dbDciW8lSYJ9tI'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: c2dbad80-0f5c-4d96-a798-2a65f93b8721
    internal-label: Assets
subfeature_v2:
  - id: edda586e-0147-48f2-b791-992622a00783
    internal-label: Landing pages
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '232'
ht-degree: 78%
---
# 追加のランディングページ CNAME の追加 {#add-additional-landing-page-cnames}

様々な URL で Marketo のランディングページを指すように、ランディングページの CNAME を追加することができます。 次の手順に従うと、複数のドメインを管理するのに役立ちます。

>[!CAUTION]
>
>Cookie は、ドメイン間で共有できません。

>[!TIP]
>
>**同じトップレベルドメイン — 可能 Cookie が共有されます**.<br/> **go**.mycompany.com > **info**.mycompany.com
>
>**異なるトップレベルドメイン — 不可能 Cookieは&#x200B;_共有されていません_**.<br/> go.**mycompany**.com > go.**mynewcompany**.com

>[!NOTE]
>
>**管理者権限が必要**

1. 「**管理者**」領域に移動します。

   ![](assets/add-additional-landing-page-cnames-1.png)

1. 「**マイアカウント**」をクリックします。

   ![](assets/add-additional-landing-page-cnames-2.png)

1. 「サポート情報」まで下にスクロールし、Munchkin ID をコピーします。

   ![](assets/add-additional-landing-page-cnames-3.png)

## IT にリクエストを送信する {#send-request-to-it}

1. 担当の IT 部門に、次の CNAME を設定するよう依頼します（[CNAME] を希望する CNAME で置き換え、[Munchkin ID] を前の手順のテキストで置き換えます)。

   [CNAME].YourCompany.com／[Munchkin ID].mktoweb.com

## 新しい CNAME を追加する {#add-a-new-cname}

1. IT 部門で CNAME が作成されたら、「**管理者**」領域に移動します。

   ![](assets/add-additional-landing-page-cnames-4.png)

1. 「**ランディングページ**」をクリックします。

   ![](assets/add-additional-landing-page-cnames-5.png)

1. 「**[!UICONTROL 新規]**」をクリックして、「**[!UICONTROL 新規ドメインエイリアス]**」を選択します。

   ![](assets/add-additional-landing-page-cnames-6.png)

1. **[!UICONTROL ドメインエイリアス]**&#x200B;を入力します。 訪問者がURLを入力しない場合、**[!UICONTROL デフォルトページ]**&#x200B;が表示されます。 その場合の移動先を入力します。

   >[!NOTE]
   >
   >[!UICONTROL デフォルトページ]の場合は、ランディングページまたは公開 web サイトなどの外部 URL を選択できます。

   ![](assets/add-additional-landing-page-cnames-7.png)

1. **[!UICONTROL デフォルトページ]**&#x200B;を入力して、「**[!UICONTROL 作成]**」をクリックします。

   ![](assets/add-additional-landing-page-cnames-8.png)

これで、ランディングページにCNAMEを追加する方法が分かりました。
