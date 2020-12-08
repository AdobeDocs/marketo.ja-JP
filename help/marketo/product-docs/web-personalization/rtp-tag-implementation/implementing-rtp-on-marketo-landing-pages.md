---
unique-page-id: 4720151
description: MarketorランディングページへのRTPの実装 — Marketto Docs — 製品ドキュメント
title: マーケティングランディングページへのRTPの実装
translation-type: tm+mt
source-git-commit: d88fb92a00e4c20509617e6ef8b2e51b66cc085b
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 0%

---


# マーケティングランディングページへのRTPの実装 {#implementing-rtp-on-marketo-landing-pages}

RTPタグを実装するには、次のインストール手順に従ってください。

1. Design **Studioに移動します。** 編集する項目を開きます。 「 **テンプレートのアクション**」を選択し、「ドラフト **の編集」を選択します。**

   ![](assets/image2015-4-26-18-3a27-3a4.png)

1. 「 **HTML Source** 」タブでテンプレートに変更を加えます。

   ![](assets/image2015-4-26-18-3a28-3a17.png)

1. RTPアカウントで、「**アカウント設定」に移動します。**

1. サポートからJavaScriptタグを既に受け取っている場合は、手順5に進みます。

   ![](assets/image2014-11-30-15-3a19-3a21-2.png)

1. 「Domain」で、関連するドメインを探し、「 **Generate Tag**」をクリックします。

   ![](assets/image2015-4-26-18-3a27-3a35.png)

   ![](assets/image2014-11-30-15-3a20-3a17-2.png)

1. RTP JavaScriptタグをコピーし、タグ間のすべてのランディングページテンプレートに貼り付け **`<head> </head>`** ます。
1. 「 **保存** 」をクリックし、ウィンドウ **を閉じます** 。
1. Design Studioに戻り、「 **Template Actions**」からランディングページを承認し **、「** Approve ****」をクリックします。\
   ![](assets/image2015-4-26-18-3a28-3a30.png)

1. 最後に、テンプレートの変更を有効にするには **、そのテンプレートを使用しているランディングページを** 再承認する必要があります。 メインランディングページセクションから一度にすべての承認を再度行うことができます。

   ![](assets/image2015-4-26-18-3a28-3a49.png)

1. すべての `pages including` ランディングページとサブドメインに表示されることを確認します。

   これは、 `website’s` ページを右クリックすると行えます。 「 **表示ページソース」に移動。** タグを見つけるには、 **RTP** を検索します。
