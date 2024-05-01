---
description: コールバック関数 – Marketoドキュメント – 製品ドキュメント
title: コールバック関数
feature: Dynamic Chat
exl-id: 5ae7f6cb-5c57-4257-8a1a-992c9602cfaa
source-git-commit: f355022fb7e6f733bb7485229e395b0fe1a9818f
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 7%

---

# コールバック関数 {#callback-functions}

Dynamic Chatウィジェットコールバック関数を使用して、任意のサードパーティプラットフォームにコンバージョンイベントを送信できます。

## はじめに {#getting-started}

このイベントは、Dynamic Chatウィジェットを使用する準備ができており、Dynamic Chatに関連するすべてのスクリプトが web ページに読み込まれると実行されることを示します。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    // code here will execute when chatbot scripts are loaded in a webpage 
}); 
```

## 会話イベント {#conversation-events}

これらのイベントは、特定の訪問者の特定のページをターゲットとした会話に関連しています。

### 会話がトリガー

Web サイトの訪問者を対象とした会話（ダイアログなど）が解決され、チャットボットが表示されます。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_TRIGGERED, (event) => { 
 // code here will execute when the chatbot is loaded for a visitor 
    }); 
});  
```

### 会話が開始されました {#conversation-engaged}

訪問者がチャットボットとエンゲージした（例えば、最初の応答を提供した）。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_ENGAGED, (event) => { 
 // code here will execute when a visitor engages with the chatbot 
     }); 
}); 
```

### 会話が完了しました {#conversation-completed}

訪問者は会話の最後に達しました。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_COMPLETED, (event) => { 
 // code here will execute when a conversation is completed 
     }); 
}); 
```

### 件の会話が終了

訪問者は、最後に達する前に会話を終了しました。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_CLOSED, (event) => { 
 // code here will execute when a conversation is closed 
    }); 
}); 
```

この `event` パラメーターは、会話に関連するメタデータを持つオブジェクトです。 にアクセスすることで、このメタデータにアクセスできます。 `event.data`.

アクセスできる主要なメタデータ値を次に示します。

<table>
<thead>
  <tr>
    <th style="width:75%">メタデータ</th>
    <th style="width:25%">属性</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>会話名</td>
    <td>payload.name</td>
  </tr>
  <tr>
    <td>会話 ID</td>
    <td>payload.id</td>
  </tr>
  <tr>
    <td>会話タイプ （ダイアログ/会話フロー）</td>
    <td>payload.type</td>
  </tr>
  <tr>
    <td>UI タイプ（ポップアップ/チャットボット/インライン）</td>
    <td>payload.uiType</td>
  </tr>
  <tr>
    <td>セッション ID</td>
    <td>payload.sid</td>
  </tr>
</tbody>
</table>

## 訪問者入力イベント

これらのイベントは、会話に参加している訪問者が連絡先情報（電話番号やメールアドレスなど）を提供したときにトリガーされます。 以下は、このカテゴリに該当するイベントです。

### 電話番号 {#phone-number}

このイベントは、訪問者が会話中に電話番号を指定したときにトリガーされます。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_INPUT_PHONE, (event) => { 
 // code here will execute when a visitor provides their phone number 
    }); 
});  
```

### メール ID {#email-id}

このイベントは、訪問者が会話中にメールアドレスを指定したときにトリガーされます。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_INPUT_EMAIL, (event) => { 
 // code here will execute when a visitor provides their email address 
    }); 
}); 
```

この `event` パラメーターは、会話に関連するメタデータを持つオブジェクトです。 にアクセスすることで、このメタデータにアクセスできます。 `event.data`.

アクセスできる主要なメタデータ値を次に示します。

<table>
<thead>
  <tr>
    <th style="width:75%">メタデータ</th>
    <th style="width:25%">属性</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>会話名</td>
    <td>payload.name</td>
  </tr>
  <tr>
    <td>会話 ID</td>
    <td>payload.id</td>
  </tr>
  <tr>
    <td>会話タイプ （ダイアログ/会話フロー）</td>
    <td>payload.type</td>
  </tr>
  <tr>
    <td>UI タイプ（ポップアップ/チャットボット/インライン）</td>
    <td>payload.uiType</td>
  </tr>
  <tr>
    <td>セッション ID</td>
    <td>payload.sid</td>
  </tr>
</tbody>
</table>

## 会議予約イベント {#meeting-booking-events}

これらのイベントは、訪問者がビジネス担当者とのミーティングを予約するとトリガーされます。

以下は、このカテゴリに該当するイベントです。

### ミーティング予約済み {#meeting-booked}

このイベントは、訪問者がエージェントのカレンダーで会議を予約するとトリガーされます。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_MEETING_BOOKED, (event) => { 
 // code here will execute when a meeting is booked 
    }); 
}); 
```

この `event` パラメーターは、会話に関連するメタデータを持つオブジェクトです。 にアクセスすることで、このメタデータにアクセスできます。 `event.data`.

アクセスできる主要なメタデータ値を次に示します。

<table>
<thead>
  <tr>
    <th style="width:75%">メタデータ</th>
    <th style="width:25%">属性</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>会話名</td>
    <td>payload.name</td>
  </tr>
  <tr>
    <td>会話 ID</td>
    <td>payload.id</td>
  </tr>
  <tr>
    <td>会話タイプ （ダイアログ/会話フロー）</td>
    <td>payload.type</td>
  </tr>
  <tr>
    <td>UI タイプ（ポップアップ/チャットボット/インライン）</td>
    <td>payload.uiType</td>
  </tr>
  <tr>
    <td>セッション ID</td>
    <td>payload.sid</td>
  </tr>
  <tr>
    <td>エージェント名</td>
    <td>payload.agentName</td>
  </tr>
  <tr>
    <td>エージェント ID</td>
    <td>payload.agentID</td>
  </tr>
  <tr>
    <td>ミーティング情報</td>
    <td>payload.meetingInfo</td>
  </tr>
</tbody>
</table>

## ライブチャットイベント {#live-chat-events}

これらのイベントは、訪問者がチャットボットとのエンゲージメント中にライブエージェントとつながったときにトリガーされます。

以下は、このカテゴリに該当するイベントです。

### ライブチャットがリクエストされました {#live-chat-requested}

このイベントは、訪問者がライブエージェントとチャットするオプションを選択し、使用可能なエージェントが解決される際にトリガーされます。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_LIVE_CHAT_REQUESTED, (event) => { 
 // code here will execute when a visitor requests a live chat 
    }); 
}); 
```

### ライブチャットが開始されました {#live-chat-initiated}

このイベントは、訪問者がライブエージェントとチャットするオプションを選択し、エージェントがチャットを受け入れるとトリガーされます。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_LIVE_CHAT_INITIATED, (event) => { 
 // code here will execute after a live agent accepts the chat 
    }); 
}); 
```

### ライブチャット終了 {#live-chat-ended}

このイベントは、訪問者とライブエージェントの間の会話が終了したときにトリガーされます。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_LIVE_CHAT_ENDED, (event) => { 
 // code here will execute when a live chat is ended 
    }); 
}); 
```

### ライブチャットタイムアウト {#live-chat-timeout}

このイベントは、訪問者が応答を停止したり、訪問者がドロップしたりしたためにライブチャットの会話がタイムアウトしたときにトリガーされます。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_LIVE_CHAT_REQUEST_TIMEOUT, (event) => { 
 // code here will execute when a visitor abandons a live chat 
    }); 
}); 
```

この `event` パラメーターは、会話に関連するメタデータを持つオブジェクトです。 にアクセスすることで、このメタデータにアクセスできます。 `event.data`.

アクセスできる主要なメタデータ値を次に示します。

<table>
<thead>
  <tr>
    <th style="width:75%">メタデータ</th>
    <th style="width:25%">属性</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>会話名</td>
    <td>payload.name</td>
  </tr>
  <tr>
    <td>会話 ID</td>
    <td>payload.id</td>
  </tr>
  <tr>
    <td>会話タイプ （ダイアログ/会話フロー）</td>
    <td>payload.type</td>
  </tr>
  <tr>
    <td>UI タイプ（ポップアップ/チャットボット/インライン）</td>
    <td>payload.uiType</td>
  </tr>
  <tr>
    <td>セッション ID</td>
    <td>payload.sid</td>
  </tr>
  <tr>
    <td>エージェント名</td>
    <td>payload.agentName</td>
  </tr>
  <tr>
    <td>エージェント ID</td>
    <td>payload.agentID</td>
  </tr>
</tbody>
</table>

これらのイベントをAdobe AnalyticsやGoogle Analyticsなどの Analytics プラットフォームに送信する場合は、これらのDynamic Chatイベント内にそれぞれのトラッキングコールを追加する必要があります。 次の例のようになります。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_TRIGGERED, (event) => { 
 // Enter Adobe Analytics or Google Analytics function here 
    ga('send', 'event', { 
      eventCategory: Dynamic Chat Conversations', 
      eventAction: 'Conversation Triggered', 
      eventLabel: event.data.payload.id, 
    }); 
    }); 
}); 
```
