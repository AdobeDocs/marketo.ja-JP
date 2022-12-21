---
unique-page-id: 11378869
description: Vibes SMS メッセージの作成 - Marketo ドキュメント - 製品ドキュメント
title: Vibes SMS メッセージの作成
exl-id: 9ec0da97-7a80-4c40-be79-be08d7d1d9c1
source-git-commit: 35e86ac356e61e9d6b9a663e468ced1e9a947144
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 100%

---

# Vibes SMS メッセージの作成 {#create-a-vibes-sms-message}

Vibes SMS メッセージの作成方法を以下に示します。

>[!AVAILABILITY]
>
>この機能は、Adobe Marketo Engage アカウントのアドオンとして使用できます。プロビジョニングを適切におこなうには、アドビで購入する必要があります。詳しくは、アドビカスタマーサクセスマネージャーにお問い合わせください。

>[!NOTE]
>
>SMS テキストメッセージは、HIPAA に準拠していません。

1. **マーケティング活動**&#x200B;に移動して、プログラムに右クリックします。

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
   >米国とカナダの制限は異なり、それぞれ 160 文字と 130 文字です。これらの文字制限を超えると、メッセージは分割されます。カナダの制限を超えた場合は通知されますが、エディターは米国向けに最適化されており、米国の制限に基づいてメッセージが分割されます。

1. 挿入メニューの「**トークン**」をクリックして、メッセージにトークンを追加します。

   ![](assets/add-token-real-hand.jpg)

   >[!NOTE]
   >
   >トークンを追加すると、メッセージの上限を超える場合があります。メッセージが分割され、追加料金が発生する場合があります。

1. 挿入メニューの「**リンク**」をクリックして、メッセージにリンクを追加します。

   ![](assets/full-message-link-hand.jpg)

1. リンクタイプを選択します。Marketo ランディングページがデフォルトです。これを使用する場合は、ドロップダウンからランディングページを選択し、「**挿入**」をクリックします。

   ![](assets/insert-link-real-hands.jpg)

   >[!NOTE]
   >
   >デフォルトでは、2 つのトラッキングリンクが選択されています。

1. 代わりに外部 URL を使用する場合は、「**外部 URL**」ボタンをクリックして、「URL」フィールドに URL を入力します。次に「**挿入**」をクリックします。

   ![](assets/insert-link-url-hands.jpg)

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
