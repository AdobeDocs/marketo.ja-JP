---
description: ライブチャット 概要 - Marketo ドキュメント - 製品ドキュメント
title: ライブチャット概要
feature: Dynamic Chat
exl-id: 44e8b249-b534-4cec-a612-daa184acd266
source-git-commit: 56070990d8bcea61fbbf3b382e5abae786b2488e
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 1%

---

# ライブチャット概要 {#live-chat-overview}

ライブチャットを使用すると、Webサイトの訪問者は販売代理店とリアルタイムのチャット会話に参加できます。

>[!NOTE]
>
>会話フローとライブチャットは共有トライアル機能であり、Dynamic Chat Select パッケージのエンゲージメントの合計全期間制限は 100 です。 この制限に達すると、公開されたすべての会話フローのトリガーが停止し、ライブエージェントとのチャットリクエスト訪問者はグローバルフォールバックメッセージを受信します。 この制限を増やすには、アカウント担当者に連絡して、パッケージのアップグレードオプションについてお問い合わせください。

## ライブチャットエージェントの追加 {#add-live-chat-agents}

ライブチャットを開始するには、ライブチャットエージェントを [Adobe Admin Consoleのユーザー](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users.md#add-a-chat-user){target="_blank"} and give them the [Live Chat permission](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md){target="_blank"}. この処理が完了したら、 [ライブチャットカード](#using-the-live-chat-card) を新規または既存のダイアログに追加します。

訪問者がダイアログを通じてエージェントとのチャットを要求すると、エージェントは複数の [通知オプション](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#live-chat-notifications){target="_blank"}. When they click on the notification, they'll be taken to their [Agent Inbox](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md){target="_blank"} そこで訪問者と話し始める事が出来る

>[!NOTE]
>
>ライブエージェントのアバターは、エージェントのAdobeアカウントプロファイルのプロファイル画像を使用します。 画像を更新するには、以下に従ってください。 [以下の手順](https://helpx.adobe.com/manage-account/using/edit-adobe-account-personal-profile.html){target="_blank"}.

## ライブチャットカードの使用 {#using-the-live-chat-card}

ストリーム デザイナー](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md){target="_blank"}の[ライブ チャット カードは、訪問者にライブ エージェントとチャットさせる場合に使用します。

![](assets/live-chat-overview-1.png)

>[!IMPORTANT]
>
>ライブチャットカードは、常にブランチの最後のカードである必要があります。 カードがブランチ内の任意のポイントに配置されている場合は、訪問者が突然エージェントに接続すると驚く可能性があります。

### ベストプラクティス {#best-practices}

* ライブチャットカードの前に質問カードを使用して、訪問者に接続を希望するかどうかを尋ねます。
* 訪問者が接続に同意したら、情報キャプチャカードを使用して、姓名、電子メールアドレス、役職などの情報を収集します。 (少なくとも名とメールアドレスリクエストことをお勧めします)。

## ライブチャットカードオプション {#live-chat-card-options}

ストリーム内のライブチャットカードをクリックすると、訪問者のルーティング方法を選択できます。 ラウンドロビン、エージェント、カスタムルール、またはチームから選択します。

![](assets/live-chat-overview-2.png)

<table> 
 <tbody> 
  <tr> 
   <td><b>ラウンドロビン</b></td>
   <td>チャットは順番にエージェントに割り当てられます。</td>
  </tr> 
  <tr> 
   <td><b>エージェント</b></td>
   <td>チャットを受信する特定のエージェントを選択します。</td>
  </tr>
    <tr> 
   <td><b>特例文字 ルール</b></td>
   <td>すべてを選択カスタムルールは、訪問者のルーティング先を検討する際に循環します。 訪問者がカスタムルールの対象とならない場合は、 <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-management.md#live-chat-fallback" target="_blank">ライブチャットフォールバックメッセージが表示されます</a>。</td>
  </tr> 
  <tr> 
   <td><b>チーム</b></td>
   <td>チャットを受け取る特定のチームを選択します。 このオプションを選択すると、そのチーム内でラウンドロビンが割り当てられます。</td>
  </tr>
 </tbody> 
</table>

## ライブチャット通知 {#live-chat-notifications}

>[!IMPORTANT]
>
>ライブチャットのブラウザ通知を受け取るには、すべてのライブチャットエージェントが、要求されたときにDynamic Chatのブラウザ通知を有効にする必要があります。

### 通知の有効化 {#enabling-notifications}

ライブチャットエージェントは、ログイン時に画面の上部に「ライブチャット通知を受信するにはブラウザー通知を有効にしてください」というバナーが表示されます。 「Enable **」をクリックします**。

![](assets/live-chat-overview-4.png)

その後、ライブチャットエージェントは、通知を表示するようにブラウザーから求められます。 「**許可**」をクリックします。

![](assets/live-chat-overview-5.png)

ブラウザーで許可した後でもエージェントがブラウザー通知を受け取らない場合は、OS 通知設定でブラウザーの通知を有効にする必要がある場合があります。

[Macの手順](https://support.apple.com/guide/mac-help/change-notifications-settings-mh40583/mac){target="_blank"}

[Windows の手順](https://support.microsoft.com/en-us/windows/change-notification-settings-in-windows-8942c744-6198-fe56-4639-34320cf9444e){target="_blank"}

### ライブチャットがエージェントにルーティングされたとき {#when-a-live-chat-is-routed-to-an-agent}

ライブチャットがエージェントにルーティングされると、画面の上部に青いバナーが表示され、承諾を求められます。

![](assets/live-chat-overview-3.png)

>[!TIP]
>
>また、Dynamic Chatにログインしていない場合にアラートブラウザー通知を設定するオプションもあります。
>
>* Google クロム で [ブラウザー通知を有効にする](https://support.google.com/chrome/answer/3220216?hl=en&amp;co=GENIE.Platform%3DDesktop){target="_blank"}
>* Mozilla Firefox で [ブラウザー通知を有効にする](https://support.mozilla.org/en-US/kb/push-notifications-firefox){target="_blank"}

### 注意事項 {#things-to-note}

* エージェントは、「チャットを受け入れる」メッセージがタイムアウトするまでに、45 秒の応答時間があります。 その後、訪問者は [フォールバックメッセージ](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-management.md#live-chat-fallback){target="_blank"}. ルーティングオプションがに設定されているDynamic Chatプライム購読者の場合 **チーム**&#x200B;に設定されていない場合は、フォールバックメッセージが表示される前に、もう 1 つのエージェントが試行されます。
* 現時点では、エージェント 1 人につき 10 のライブチャットの制限があります。

>[!MORELIKETHIS]
>
>[エージェントインボックス](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md){target="_blank"}
