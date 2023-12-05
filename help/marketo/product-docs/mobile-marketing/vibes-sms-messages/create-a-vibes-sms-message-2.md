---
description: Vibes SMS メッセージの作成 - Marketo ドキュメント - 製品ドキュメント
title: Vibes SMS メッセージの作成
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: cd09ad43c08855af63131aa385c4fd406c963926
workflow-type: tm+mt
source-wordcount: '441'
ht-degree: 66%

---

# Vibes SMS メッセージの作成 {#create-a-vibes-sms-message}

Vibes SMS メッセージの作成方法を以下に示します。

>[!AVAILABILITY]
>
>この機能は、Adobe Marketo Engage アカウントのアドオンとして使用できます。プロビジョニングを適切におこなうには、Adobeで購入する必要があります。 詳しくは、アドビアカウントチーム（担当のアカウントマネージャー）にお問い合わせください。

1. 「**マーケティングアクティビティ**」に移動します。

   ![](assets/mobile-right-click-hand.jpg)

1. プログラムを右クリックし、「 」を選択します。 **新規ローカルアセット**.

   ![](assets/mobile-right-click-hand.jpg)

1. 「**新規ローカルアセット**」をクリックします。

   ![](assets/new-local-asset-hand.jpg)

   >[!TIP]
   >
   >または、**新規作成**&#x200B;ドロップダウンをクリックできます。

1. 「**SMS メッセージ**」をクリックします。

   ![](assets/new-local-asset-selection-hand.jpg)

1. 新しい SMS メッセージの名前と説明（オプション）を入力し、「**作成**」をクリックします。

   ![](assets/new-sms-message-offer-ends-soon-hands.jpg)

1. **ドラフトの編集**&#x200B;をクリックします。

   ![](assets/edit-draft-hand.jpg)

1. メッセージエディターで、青い吹き出しの内側をクリックし、テキストの入力を開始します。

   ![](assets/message-text-pencil.jpg)

   >[!NOTE]
   >
   >SMS メッセージの文字制限は、標準の ASCII 文字セットを使用した 160 文字です。 160 文字を超える場合、メッセージは合計文字数に基づいて分割されます。

1. 挿入メニューの「**トークン**」をクリックして、メッセージにトークンを追加します。

   ![](assets/add-token-real-hand.jpg)

   >[!NOTE]
   >
   >トークンを追加すると、メッセージの上限を超える場合があります。その後、メッセージは分割され、結果として追加のメッセージが生成されます。

   >[!IMPORTANT]
   >
   >SMS コンプライアンス：すべての送信 SMS メッセージには、ブランド名またはプログラムの説明が含まれている必要があります。 定期的なメッセージプログラムの場合、購読者ごとに少なくとも月に 1 回、ヘルプと停止の手順を提供する必要があります。

   ??????Marketo URL 短縮サービスを使用すると、メッセージで X 文字が使用されます??????

1. 挿入メニューの「**リンク**」をクリックして、メッセージにリンクを追加します。

   ![](assets/full-message-link-hand.jpg)

1. リンクタイプを選択します。Marketo ランディングページがデフォルトです。これを使用する場合は、ドロップダウンからランディングページを選択し、「**挿入**」をクリックします。

   ![](assets/insert-link-real-hands.jpg)

   >[!NOTE]
   >
   >* デフォルトでは、2 つのトラッキングリンクが選択されています。
   >* Marketo URL 短縮サービスを使用すると、メッセージで X 文字が使用されます。??????????????????

1. 代わりに外部 URL を使用する場合は、「**外部 URL**」ボタンをクリックして、「URL」フィールドに URL を入力します。次に「**挿入**」をクリックします。

   ![](assets/insert-link-url-hands.jpg)

   >[!CAUTION]
   >
   >次の操作をお勧めします。 _not_ 通信事業者がメッセージにスパムのフラグを設定する場合があるので、短縮 URL（Bitly など）を使用します。

1. メッセージにリンクが表示されます。

   ![](assets/link-added.jpg)

   >[!NOTE]
   >
   >Marketo に、ブランド化されたトラッキングドメインのリンクプレビューが表示されます。mkt_tok リンクチェックボックスをオフにすると、リンクが変更されます。「リンクを追跡」チェックボックスもオフにすると、URL が基本的な長さに短縮されます（例：www.mygooglepage.com）。

   ![](assets/image2016-7-27-16-3a20-3a16.png)

   >[!NOTE]
   >
   >文字数には、最も低いメッセージに含まれる文字のみが反映されます。

米国の制限を超えて挿入すると、エディターはメッセージを複数のセクションに分割します。合計で 900 文字までという制限があります。上限に達すると、メッセージはオーディエンスに送信される際に自動的に切り捨てられます。

米国の上限????????
