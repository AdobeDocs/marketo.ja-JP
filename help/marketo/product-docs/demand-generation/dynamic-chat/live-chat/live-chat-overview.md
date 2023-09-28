---
description: Live Chat の概要 — Marketoドキュメント — 製品ドキュメント
title: ライブチャットの概要
feature: Dynamic Chat
exl-id: f6563e73-4b6e-437d-bf8b-ec72a9b8bcb3
source-git-commit: 38274b4859ae38c018ee73d4f1715fdf6a78e815
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 2%

---

# ライブチャットの概要 {#live-chat-overview}

ライブチャットを使用すると、ウェブサイトの訪問者がセールスエージェントとリアルタイムでチャットできるようになります。

## ライブチャットエージェントの追加 {#add-live-chat-agents}

ライブチャットを開始するには、ライブチャットエージェントを [Adobe Admin Consoleのユーザー](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users.md#add-a-chat-user){target="_blank"} and give them the [Live Chat permission](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md){target="_blank"}. この処理が完了したら、 [ライブチャットカード](#using-the-live-chat-card) を新規または既存のダイアログに追加します。

訪問者がダイアログを通じてエージェントとのチャットを要求すると、エージェントは複数の [通知オプション](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#live-chat-notifications){target="_blank"}. When they click on the notification, they'll be taken to their [Agent Inbox](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md){target="_blank"} そこで訪問者と話し始める事が出来る

## ライブチャットカードの使用 {#using-the-live-chat-card}

でライブチャットカードを使用します。 [ストリームデザイナー](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md){target="_blank"} 訪問者がライブエージェントとチャットする場合。

![](assets/live-chat-overview-1.png)

>[!IMPORTANT]
>
>ライブチャットカードは、常にブランチの最後のカードである必要があります。 カードがブランチ内の任意のポイントに配置されている場合は、訪問者が突然エージェントに接続すると驚く可能性があります。

### ベストプラクティス {#best-practices}

* ライブチャットカードの前に質問カードを使用して、訪問者に接続を希望するかどうかを尋ねます。
* 訪問者がの接続に同意したら、情報キャプチャカードを使用して、氏名、E メールアドレス、職位など、情報の一部を収集します。 （少なくとも名と E メールアドレスをリクエストすることをお勧めします）。

## Live Chat カードのオプション {#live-chat-card-options}

ストリーム内のライブチャットカードをクリックすると、訪問者のルーティング方法を選択できます。 ラウンドロビン、エージェント、カスタムルール、チームから選択できます。

![](assets/live-chat-overview-2.png)

<table> 
 <tbody> 
  <tr> 
   <td><b>ラウンドロビン</b></td>
   <td>チャットは、エージェントに順番に割り当てられます。</td>
  </tr> 
  <tr> 
   <td><b>エージェント</b></td>
   <td>チャットを受信する特定のエージェントを選択します。</td>
  </tr>
    <tr> 
   <td><b>カスタムルール</b></td>
   <td>訪問者のルーティング先を検討する際には、すべてのカスタムルールがサイクルスルーされます。 訪問者がカスタムルールの対象でない場合、 <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-management.md#live-chat-fallback" target="_blank">ライブチャットフォールバックメッセージ</a>.</td>
  </tr> 
  <tr> 
   <td><b>チーム</b></td>
   <td>チャットを受け取る特定のチームを選択します。 このオプションを選択すると、そのチーム内でラウンドロビンが割り当てられます。</td>
  </tr>
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[エージェントのインボックス](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md){target="_blank"}
