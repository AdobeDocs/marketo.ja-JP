---
unique-page-id: 4720151
description: MarketoランディングページでのRTPの実装 —Marketoドキュメント — 製品ドキュメント
title: MarketoランディングページでのRTPの実装
exl-id: fd19c3ad-d3f6-44a3-9f7a-d518e2d3f02a
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%

---

# MarketoランディングページでのRTPの実装{#implementing-rtp-on-marketo-landing-pages}

RTPタグを実装するには、次のインストール手順に従ってください。

1. **Design Studioに移動します。** 編集する項目を開きます。「**テンプレートアクション**」を選択し、「**ドラフトを編集**」を選択します。

   ![](assets/image2015-4-26-18-3a27-3a4.png)

1. 「**HTML Source**」タブでテンプレートに変更を加えます。

   ![](assets/image2015-4-26-18-3a28-3a17.png)

1. RTPアカウントで、**「アカウント設定**」に移動します。

   a.サポートからJavaScriptタグを既に受け取っている場合は、手順5に進みます。

   ![](assets/image2014-11-30-15-3a19-3a21-2.png)

1. 「Domain」で、関連するドメインを探し、「**Generate Tag**」をクリックします。

   ![](assets/image2015-4-26-18-3a27-3a35.png)

   ![](assets/image2014-11-30-15-3a20-3a17-2.png)

1. RTP JavaScriptタグをコピーし、**`<head> </head>`**&#x200B;タグ間のすべてのランディングページテンプレートに貼り付けます。

1. 「**保存**」をクリックし、「**閉じる**」をクリックします。

1. **Design Studio**&#x200B;に戻り、**テンプレートアクション**&#x200B;からランディングページを承認し、**承認**&#x200B;をクリックします。

   ![](assets/image2015-4-26-18-3a28-3a30.png)

1. 最後に、テンプレートの変更を有効にするには、そのテンプレートを使用しているすべてのランディングページを&#x200B;**再承認**&#x200B;する必要があります。 メインランディングページセクションから一度にすべての承認を再度行うことができます。

   ![](assets/image2015-4-26-18-3a28-3a49.png)

1. ランディングページとサブドメインを含むすべてのページに表示されることを確認します。

   これは、ウェブサイトのページを右クリックすると行えます。 **表示ページソースに移動します。** RTPを検索して、タグを探し **** ます。
