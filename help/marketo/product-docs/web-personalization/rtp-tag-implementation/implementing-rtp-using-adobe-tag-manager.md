---
unique-page-id: 4720218
description: Adobe tagを使用したrtpの実装など、Marketo Engageのadobe tag managerを使用したrtpの実装について説明します。 このガイドを使用して、次のステップを完了してください。
title: Adobe Tag Manager を使用した RTP の実装
exl-id: 5a938d02-6b09-45d5-94b0-dbb50b5d62b6
feature: Web Personalization
TQID: https://experienceleague.adobe.com/aIrAA9GHOTh0EkaSgVYq4veUQH-0uNbIfUvWfV825fQ
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: e2290edd-b061-4880-9d79-dee306cf5aa9
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 230
ht-degree: 65%

---

# Adobe Tag Manager を使用した RTP の実装 {#implementing-rtp-using-adobe-tag-manager}

RTP タグを実装するには、次のインストール手順に従います。

1. RTP アカウントにログインします。

1. 「**[!UICONTROL アカウント設定]**」に移動します。

   a. サポートからJavaScript タグを既に受け取っている場合は、手順4に進みます。

   ![](assets/image2014-11-30-15-3a19-3a21-4.png)

1. 「[!UICONTROL ドメイン]」で、該当するドメインを選択し、「**[!UICONTROL タグを生成]**」をクリックします。

   ![](assets/image2014-11-30-15-3a20-3a17-4.png)

1. [!DNL Dynamic Tag Manager] アカウント（[https://dtm.adobe.com/sign_in](https://dtm.adobe.com/sign_in)）にログインします。

1. **[!UICONTROL ダッシュボード &#x200B;]に移動します。** 関連するweb プロパティをクリックします。

   ![](assets/image2014-12-3-17-3a58-3a17.png)

1. **[!UICONTROL ルール]**&#x200B;に移動して、「**[!UICONTROL ルールを新規作成]**」をクリックします。

1. 次の情報を入力します。

   1. [!UICONTROL 名前]：**Marketo RTP**
   1. [!UICONTROL 条件]（折りたたみ）：トリガールール：**[!UICONTROL ページの先頭]**
   1. [!UICONTROL JavaScript]（折りたたみ）：「**[!UICONTROL 新しいスクリプトを追加]**」をクリック

   ![](assets/image2014-12-3-17-3a59-3a40.png)

1. 新しいタグを **MarketoRTP タグ**&#x200B;と呼びます

1. [!UICONTROL RTP タグ]から次のコードを削除します

   * `<script type='text/javascript'>`
   * `</script>`

1. RTP JavaScript タグをペーストします。

   ![](assets/image2014-12-3-18-3a3-3a45.png)

   >[!CAUTION]
   >
   >すべてのタグを削除し、スクリプト自体のみを残します（`<script type='text/javascript'>`、`</script>` なし）

1. スクリプトエディターで、「**[!UICONTROL コードを保存]**」をクリックして、ルールエディターで「**[!UICONTROL ルールを保存]**」をクリックします。

1. ルールパネルで、Marketo RTP ページ読み込みルールを見つけ、**[!UICONTROL アクション]** ドロップダウン内で「**[!UICONTROL ルールをアクティブ化]**」を選択します。

   ![](assets/image2014-12-3-18-3a4-3a14.png)

1. ランディングページとサブドメインも含めて、すべてのページにタグがあることを&#x200B;**[!UICONTROL 確認]**&#x200B;します。

   これは、web サイトのページで右クリックすることで可能です。 **[!UICONTROL 要素を検査]**&#x200B;に移動して、「**[!UICONTROL ネットワーク]**」をクリックして **RTP** を検索します。
