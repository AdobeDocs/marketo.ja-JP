---
unique-page-id: 4720218
description: Adobe Tag Manager を使用した RTP の実装 - Marketo ドキュメント - 製品ドキュメント
title: Adobe Tag Manager を使用した RTP の実装
exl-id: 5a938d02-6b09-45d5-94b0-dbb50b5d62b6
feature: Web Personalization
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '208'
ht-degree: 79%

---

# Adobe Tag Manager を使用した RTP の実装 {#implementing-rtp-using-adobe-tag-manager}

RTP タグを実装するには、次のインストール手順に従います。

1. RTP アカウントにログインします。

1. 「**[!UICONTROL アカウント設定]**」に移動します。

   a サポートから既に JavaScript タグを受け取っている場合は、手順 4 に進みます。

   ![](assets/image2014-11-30-15-3a19-3a21-4.png)

1. [!UICONTROL &#x200B; ドメイン &#x200B;] の下で関連するドメインを見つけて、「**[!UICONTROL タグを生成]**」をクリックします。

   ![](assets/image2014-11-30-15-3a20-3a17-4.png)

1. [!DNL Dynamic Tag Manager] アカウント （[https://dtm.adobe.com/sign_in](https://dtm.adobe.com/sign_in)）にログインします。

1. **[!UICONTROL ダッシュボード &#x200B;] に移動します。**&#x200B;関連する web プロパティをクリックします。

   ![](assets/image2014-12-3-17-3a58-3a17.png)

1. **[!UICONTROL ルール]**&#x200B;に移動して、「**[!UICONTROL ルールを新規作成]**」をクリックします。

1. 次の情報を入力します。

   1. [!UICONTROL &#x200B; 名前 &#x200B;]: **Marketo RTP**
   1. [!UICONTROL &#x200B; 条件 &#x200B;] （折りたたみ） :トリガールール **[!UICONTROL 場所 – ページの上部]**
   1. [!UICONTROL JavaScript] （折りたたみ）:「**[!UICONTROL 新規スクリプトを追加]**」をクリックします

   ![](assets/image2014-12-3-17-3a59-3a40.png)

1. 新しいタグを **MarketoRTP タグ**&#x200B;と呼びます

1. [!UICONTROL RTP タグ &#x200B;] から次のコードを削除します。

   * `<script type='text/javascript'>`
   * `</script>`

1. RTP JavaScript タグをペーストします。

   ![](assets/image2014-12-3-18-3a3-3a45.png)

   >[!CAUTION]
   >
   >すべてのタグを削除し、スクリプト自体のみを残します（`<script type='text/javascript'>`、`</script>` なし）

1. スクリプトエディターで、「**[!UICONTROL コードを保存]**」をクリックして、ルールエディターで「**[!UICONTROL ルールを保存]**」をクリックします。

1. ルールパネルで、Marketo RTP ページ読み込みルールを探し、**[!UICONTROL アクション]**&#x200B;ドロップダウンで「**[!UICONTROL ルールをアクティブ化]**」を選択します。

   ![](assets/image2014-12-3-18-3a4-3a14.png)

1. ランディングページとサブドメインも含めて、すべてのページにタグがあることを&#x200B;**[!UICONTROL 確認]**&#x200B;します。

   これは、web サイトのページを右クリックすると実行できます。**[!UICONTROL 要素を検査]**&#x200B;に移動して、「**[!UICONTROL ネットワーク]**」をクリックして **RTP** を検索します。
