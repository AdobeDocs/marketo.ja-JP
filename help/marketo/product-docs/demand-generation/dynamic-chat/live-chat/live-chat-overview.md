---
description: Live Chat の概要 — Marketoドキュメント — 製品ドキュメント
title: ライブチャットの概要
feature: Dynamic Chat
exl-id: 44e8b249-b534-4cec-a612-daa184acd266
source-git-commit: 492a43045bdf77243e4600eeb2223e750a35859b
workflow-type: tm+mt
source-wordcount: '618'
ht-degree: 1%

---

# ライブチャットの概要 {#live-chat-overview}

ライブチャットを使用すると、ウェブサイトの訪問者がセールスエージェントとリアルタイムでチャットできるようになります。

>[!NOTE]
>
>対話型フローとライブチャットは、Dynamic Chat選択パッケージ上のユーザーに対して 100 のエンゲージメントの総ライフタイム制限を持つトライアル機能です。 この制限に達すると、すべての公開済みの対話フローがトリガーされなくなり、ライブエージェントとのチャットを要求した訪問者がグローバルなフォールバックメッセージを受け取ります。 この制限を増やすには、アカウント担当者に連絡して、パッケージのアップグレードオプションについてお問い合わせください。

## ライブチャットエージェントの追加 {#add-live-chat-agents}

ライブチャットを開始するには、ライブチャットエージェントを [Adobe Admin Consoleのユーザー](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users.md#add-a-chat-user){target="_blank"} and give them the [Live Chat permission](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md){target="_blank"}. この処理が完了したら、 [ライブチャットカード](#using-the-live-chat-card) を新規または既存のダイアログに追加します。

訪問者がダイアログを通じてエージェントとのチャットを要求すると、エージェントは複数の [通知オプション](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#live-chat-notifications){target="_blank"}. When they click on the notification, they'll be taken to their [Agent Inbox](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md){target="_blank"} そこで訪問者と話し始める事が出来る

>[!NOTE]
>
>ライブエージェントのアバターは、エージェントのAdobeアカウントプロファイルのプロファイル画像を使用します。 画像を更新するには、以下に従ってください。 [以下の手順](https://helpx.adobe.com/manage-account/using/edit-adobe-account-personal-profile.html){target="_blank"}.

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

## ライブチャット通知 {#live-chat-notifications}

ライブチャットのブラウザ通知を受け取るには、すべてのライブチャットエージェントが、要求されたときにDynamic Chatのブラウザ通知を有効にする必要があります。

### 通知の有効化 {#enabling-notifications}

Live Chat エージェントは、ログイン時に画面の上部に「Please enable browser notifications to receive live chat notifications」と表示されます。 クリック **有効にする**.

![](assets/live-chat-overview-4.png)

その後、ライブチャットエージェントは、通知を表示するようにブラウザーから求められます。 「**許可**」をクリックします。

![](assets/live-chat-overview-5.png)

ブラウザーで許可した後でもエージェントがブラウザー通知を受け取らない場合は、OS 通知設定でブラウザーの通知を有効にする必要がある場合があります。

[Macの手順](https://support.apple.com/guide/mac-help/change-notifications-settings-mh40583/mac){target="_blank"}

[Windows の手順](https://support.microsoft.com/en-us/windows/change-notification-settings-in-windows-8942c744-6198-fe56-4639-34320cf9444e){target="_blank"}

### ライブチャットがエージェントにルーティングされたとき {#when-a-live-chat-is-routed-to-an-agent}

ライブチャットがエージェントにルーティングされると、画面の上部に青いバナーが表示され、受け入れを求められます。

![](assets/live-chat-overview-3.png)

>[!TIP]
>
>また、ブラウザー通知を設定するオプションもあります。ブラウザー通知は、Dynamic Chatにログインしていない場合に通知を受け取ります。
>
>* でのブラウザー通知の有効化 [Google Chrome](https://support.google.com/chrome/answer/3220216?hl=en&amp;co=GENIE.Platform%3DDesktop){target="_blank"}
>* でのブラウザー通知の有効化 [Mozilla Firefox](https://support.mozilla.org/en-US/kb/push-notifications-firefox){target="_blank"}

### 注意事項 {#things-to-note}

* エージェントは、「チャットを受け入れる」メッセージがタイムアウトするまでに、45 秒の応答時間があります
* 現時点では、エージェントごとに 10 のライブチャットの制限があります

>[!MORELIKETHIS]
>
>[エージェントインボックス](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md){target="_blank"}
