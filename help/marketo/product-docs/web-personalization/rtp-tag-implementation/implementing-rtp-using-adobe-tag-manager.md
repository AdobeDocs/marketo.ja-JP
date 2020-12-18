---
unique-page-id: 4720218
description: Adobe Tag Managerを使用したRTPの実装 — Marketto Docs — 製品ドキュメント
title: Adobe Tag Managerを使用したRTPの実装
translation-type: tm+mt
source-git-commit: d88fb92a00e4c20509617e6ef8b2e51b66cc085b
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---


# Adobe Tag Manager{#implementing-rtp-using-adobe-tag-manager}を使用したRTPの実装

RTPタグを実装するには、次のインストール手順に従ってください。

1. RTPアカウントにログインします。
1. **アカウント設定に移動します。**

   サポートからJavaScriptタグを既に受け取っている場合は、手順4に進みます。

   ![](assets/image2014-11-30-15-3a19-3a21-4.png)

1. 「Domain」で、関連するドメインを探し、「**Generate Tag**」をクリックします。

   ![](assets/image2014-11-30-15-3a20-3a17-4.png)

1. Dynamic Tag Managerアカウント([https://dtm.adobe.com/sign_in](https://dtm.adobe.com/sign_in))にログインします。
1. **ダッシュボードに移動します。** 関連するWebプロパティをクリックします。

   ![](assets/image2014-12-3-17-3a58-3a17.png)

1. [**ルール**]に移動し、[**新しいルールの作成]をクリックします。**

1. 次の情報を入力します。

   1. 名前：**Marketo RTP**
   1. 条件（折りたたみ）:- **ページの先頭**&#x200B;のトリガールール
   1. JavaScript（折りたたみ）:**追加新しいスクリプト**&#x200B;をクリックします

   ![](assets/image2014-12-3-17-3a59-3a40.png)

1. 新しいタグを呼び出します。**Marketo RTPタグ**
1. RTPタグから次のコードを削除します。

   * `<script type='text/javascript'>`
   * `</script>`

1. RTP JavaScriptタグを貼り付けます。

   ![](assets/image2014-12-3-18-3a3-3a45.png)

   >[!CAUTION]
   >
   >すべてのタグを削除し、スクリプト自体は残しておく必要があります（`<script type='text/javascript'>`、`</script>`は除く）

1. スクリプトエディターで「**コードを保存**」をクリックし、ルールエディターで「**ルールを保存**」をクリックします。

1. ルールパネルで、Marketo RTPページ型ルールを見つけ、**アクション**&#x200B;ドロップダウンで&#x200B;**ルールをアクティブ化**&#x200B;を選択します。

   ![](assets/image2014-12-3-18-3a4-3a14.png)

1. **ランディングページとサブドメインを含むすべてのページに表示されることを** 確認します。

   Webサイトのページを右クリックすると、その操作を実行できます。 **Inspect要素**&#x200B;に移動し、「**ネットワーク， **検索：**RTP**。
