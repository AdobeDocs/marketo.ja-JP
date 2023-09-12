---
description: Live Chat の概要 — Marketoドキュメント — 製品ドキュメント
title: ライブチャットの概要
hide: true
hidefromtoc: true
feature: Dynamic Chat
source-git-commit: a4fe70e1a95ff382499800049f161d1ad7dec7ab
workflow-type: tm+mt
source-wordcount: '239'
ht-degree: 3%

---

# ライブチャットの概要 {#live-chat-overview}

でライブチャットカードを使用します。 [ストリームデザイナー](/help/marketo/product-docs/demand-generation/dynamic-chat-two/automated-chat/stream-designer.md){target="_blank"} 訪問者がライブエージェントとチャットする場合。

## ライブチャットカードの使用 {#using-the-live-chat-card}

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
   <td>訪問者のルーティング先を検討する際には、すべてのカスタムルールがサイクルスルーされます。 訪問者がカスタムルールの対象でない場合、 <a href="/help/marketo/product-docs/demand-generation/dynamic-chat-two/setup-and-configuration/agent-management.md#live-chat-fallback" target="_blank">ライブチャットフォールバックメッセージ</a>.</td>
  </tr> 
  <tr> 
   <td><b>チーム</b></td>
   <td>チャットを受け取る特定のチームを選択します。 このオプションを選択すると、そのチーム内でラウンドロビンが割り当てられます。</td>
  </tr>
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[エージェントのインボックス](/help/marketo/product-docs/demand-generation/dynamic-chat-two/live-chat/agent-inbox.md){target="_blank"}
