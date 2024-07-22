---
description: コールバック関数 - Marketo ドキュメント - 製品ドキュメント
title: コールバック関数
feature: Dynamic Chat
exl-id: 5ae7f6cb-5c57-4257-8a1a-992c9602cfaa
source-git-commit: f355022fb7e6f733bb7485229e395b0fe1a9818f
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 100%

---

# コールバック関数 {#callback-functions}

Dynamic Chat ウィジェットコールバック関数を使用すると、対話イベントをサードパーティプラットフォームに送信できます。

## はじめに {#getting-started}

このイベントは、Dynamic Chat ウィジェットの使用準備が整っていることを示し、Dynamic Chat に関連するすべてのスクリプトが web ページに読み込まれると発生します。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    // code here will execute when chatbot scripts are loaded in a webpage 
}); 
```

## 対話イベント {#conversation-events}

このイベントは、特定の訪問者の特定のページでターゲットとされる対話に関連しています。

### 対話トリガー済み

Web サイトの訪問者をターゲットとした対話（ダイアログなど）が解決され、チャットボットが訪問者に表示されます。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_TRIGGERED, (event) => { 
 // code here will execute when the chatbot is loaded for a visitor 
    }); 
});  
```

### 対話エンゲージ済み {#conversation-engaged}

訪問者がチャットボットに関与しました（最初の応答を提供するなど）。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_ENGAGED, (event) => { 
 // code here will execute when a visitor engages with the chatbot 
     }); 
}); 
```

### 対話完了 {#conversation-completed}

訪問者が対話の終了に達しました。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_COMPLETED, (event) => { 
 // code here will execute when a conversation is completed 
     }); 
}); 
```

### 対話クローズ済み

訪問者が終了に達する前に対話をクローズしました。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_CLOSED, (event) => { 
 // code here will execute when a conversation is closed 
    }); 
}); 
```

`event` パラメーターは、対話に関連するメタデータを含むオブジェクトです。このメタデータには、`event.data` にアクセスすることでアクセスできます。

アクセスできるいくつかの主なメタデータ値を次に示します。

<table>
<thead>
  <tr>
    <th style="width:75%">メタデータ</th>
    <th style="width:25%">属性</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>対話名</td>
    <td>payload.name</td>
  </tr>
  <tr>
    <td>対話 ID</td>
    <td>payload.id</td>
  </tr>
  <tr>
    <td>対話タイプ（ダイアログ／対話フロー）</td>
    <td>payload.type</td>
  </tr>
  <tr>
    <td>UI タイプ（ポップアップ／チャットボット／インライン）</td>
    <td>payload.uiType</td>
  </tr>
  <tr>
    <td>セッション ID</td>
    <td>payload.sid</td>
  </tr>
</tbody>
</table>

## 訪問者入力イベント

このイベントは、対話に関与している訪問者が取引先責任者情報（電話番号やメールアドレスなど）を入力するとトリガーされます。このカテゴリに該当するイベントを次に示します。

### 電話番号 {#phone-number}

このイベントは、訪問者が対話中に電話番号を入力した際にトリガーされます。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_INPUT_PHONE, (event) => { 
 // code here will execute when a visitor provides their phone number 
    }); 
});  
```

### メール ID {#email-id}

このイベントは、訪問者が対話中にメールアドレスを入力した際にトリガーされます。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_INPUT_EMAIL, (event) => { 
 // code here will execute when a visitor provides their email address 
    }); 
}); 
```

`event` パラメーターは、対話に関連するメタデータを含むオブジェクトです。このメタデータには、`event.data` にアクセスすることでアクセスできます。

アクセスできるいくつかの主なメタデータ値を次に示します。

<table>
<thead>
  <tr>
    <th style="width:75%">メタデータ</th>
    <th style="width:25%">属性</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>対話名</td>
    <td>payload.name</td>
  </tr>
  <tr>
    <td>対話 ID</td>
    <td>payload.id</td>
  </tr>
  <tr>
    <td>対話タイプ（ダイアログ／対話フロー）</td>
    <td>payload.type</td>
  </tr>
  <tr>
    <td>UI タイプ（ポップアップ／チャットボット／インライン）</td>
    <td>payload.uiType</td>
  </tr>
  <tr>
    <td>セッション ID</td>
    <td>payload.sid</td>
  </tr>
</tbody>
</table>

## ミーティング予約イベント {#meeting-booking-events}

このイベントは、訪問者がビジネス担当者とのミーティングを予約するとトリガーされます。

このカテゴリに該当するイベントを次に示します。

### ミーティング予約済み {#meeting-booked}

このイベントは、訪問者がエージェントのカレンダーでミーティングを予約するとトリガーされます。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_MEETING_BOOKED, (event) => { 
 // code here will execute when a meeting is booked 
    }); 
}); 
```

`event` パラメーターは、対話に関連するメタデータを含むオブジェクトです。このメタデータには、`event.data` にアクセスすることでアクセスできます。

アクセスできるいくつかの主なメタデータ値を次に示します。

<table>
<thead>
  <tr>
    <th style="width:75%">メタデータ</th>
    <th style="width:25%">属性</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>対話名</td>
    <td>payload.name</td>
  </tr>
  <tr>
    <td>対話 ID</td>
    <td>payload.id</td>
  </tr>
  <tr>
    <td>対話タイプ（ダイアログ／対話フロー）</td>
    <td>payload.type</td>
  </tr>
  <tr>
    <td>UI タイプ（ポップアップ／チャットボット／インライン）</td>
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

このイベントは、訪問者がチャットボットとのエンゲージメント中にライブエージェントに接続するとトリガーされます。

このカテゴリに該当するイベントを次に示します。

### ライブチャットリクエスト済み {#live-chat-requested}

このイベントは、訪問者がライブエージェントとチャットするオプションを選択し、対応可能なエージェントが解決されるとトリガーされます。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_LIVE_CHAT_REQUESTED, (event) => { 
 // code here will execute when a visitor requests a live chat 
    }); 
}); 
```

### ライブチャット開始済み {#live-chat-initiated}

このイベントは、訪問者がライブエージェントとチャットするオプションを選択し、エージェントがチャットを受け入れるとトリガーされます。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_LIVE_CHAT_INITIATED, (event) => { 
 // code here will execute after a live agent accepts the chat 
    }); 
}); 
```

### ライブチャット終了済み {#live-chat-ended}

このイベントは、訪問者とライブエージェント間の対話が終了するとトリガーされます。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_LIVE_CHAT_ENDED, (event) => { 
 // code here will execute when a live chat is ended 
    }); 
}); 
```

### ライブチャットタイムアウト {#live-chat-timeout}

このイベントは、訪問者が応答の停止やドロップを行ったので、ライブチャットの対話がタイムアウトするとトリガーされます。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_LIVE_CHAT_REQUEST_TIMEOUT, (event) => { 
 // code here will execute when a visitor abandons a live chat 
    }); 
}); 
```

`event` パラメーターは、対話に関連するメタデータを含むオブジェクトです。このメタデータには、`event.data` にアクセスすることでアクセスできます。

アクセスできるいくつかの主なメタデータ値を次に示します。

<table>
<thead>
  <tr>
    <th style="width:75%">メタデータ</th>
    <th style="width:25%">属性</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>対話名</td>
    <td>payload.name</td>
  </tr>
  <tr>
    <td>対話 ID</td>
    <td>payload.id</td>
  </tr>
  <tr>
    <td>対話タイプ（ダイアログ／対話フロー）</td>
    <td>payload.type</td>
  </tr>
  <tr>
    <td>UI タイプ（ポップアップ／チャットボット／インライン）</td>
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

これらのイベントのいずれかを Adobe Analytics や Google Analytics などの分析プラットフォームに送信する場合は、これらの Dynamic Chat イベント内にそれぞれのトラッキング呼び出しを追加する必要があります。次の例のようになります。

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
