---
description: Dynamic Chatの概要 — Marketoドキュメント — 製品ドキュメント
title: ダイナミックチャットの概要
hide: true
hidefromtoc: true
source-git-commit: c6713c972603ab9528a66e908e47e4c187b86c0c
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---

# ダイナミックチャットの概要 {#dynamic-chat-overview}

導入テキスト

>[!NOTE]
>
>Dynamic Chatは展開中で、すべての購読はDATEでアクセスできます。

## ダイナミックチャットの設定 {#access-dynamic-chat}

初期設定の手順は次のとおりです。

1. マイMarketoで、**ダイナミックチャット**&#x200B;タイルをクリックします。

   PICC

   >[!NOTE]
   >
   >見えなければ…Marketoの管理者に問い合わせてください)。

1. 以前にAdobe IDでアプリにアクセスしたことがある場合は、Dynamic Chatに直接アクセスできます。 そうでない場合は、[Adobe ID](https://helpx.adobe.com/manage-account/using/create-update-adobe-id.html)を設定します。

   PICC

1. Marketoインスタンスに接続するには、「**統合**」を選択します。

   PICC

1. ?INSERT TEXT HERE？をクリックします。

   PICC

   >[!NOTE]
   >
   >データベースのサイズに応じて、同期が完了するまでに5分から8時間かかる場合があります。 平均同期時間は60分です。

## 統合 {#integrations}

統合は、Dynamic Chatにアクセスする際に最初にアクセスするタブです。 Marketoサブスクリプションを同期する場所で、Marketoデータベースのデータを利用してサイト/チャットの訪問者を識別できます（[上記の手順3](#access-dynamic-chat)を参照）。

## ダイアログ {#dialogues}

ダイアログは、設定する個々のチャットの会話です。 既知の訪問者や匿名の訪問者に対して、誰に何を表示するかを指定できます。 [ダイアログの詳細](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues.md)を参照してください。

## 構成 {#configuration}

「設定」タブで、様々なダイアログのルックアンドフィールをカスタマイズします。 フォント、色、応答時間などを変更します。 [設定の詳細](/help/marketo/product-docs/demand-generation/dynamic-chat/configuration.md)を説明します。

## カレンダー {#calendar}

[カレンダー]タブで、（OutlookまたはGmail）カレンダーをDynamic Chatに接続して、サイト訪問者がエージェントとの予定をスケジュールできるようにします。

## 会議 {#meetings}

[会議]タブでは、Dynamic Chatを介してエージェントがスケジュールしたすべての会議のステータスや、その他の関連する詳細を確認できます。

PICC?

## Routing {#routing}

ルーティングには、エージェントがミーティングを割り当てられる順序と、（エージェントごとの）今日までの総ミーティングが表示されます。 会議はラウンドロビン方式で行われるので、エージェントが5人、エージェントが3人、最後の会議を取った場合、エージェント4が次の1人、次に5人、次にエージェント1に戻ります。
