---
unique-page-id: 1146999
description: 興味深い瞬間のトリガートークン —Marketoドキュメント — 製品ドキュメント
title: 興味深い瞬間のトリガートークン
exl-id: 666a6eed-c432-4088-b4f1-54c996eca64c
translation-type: tm+mt
source-git-commit: 20a3bee9973340d7b772532d1be31fe745e5ffd7
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 29%

---

# 興味深い瞬間のトリガートークン{#trigger-tokens-for-interesting-moments}

>[!PREREQUISITES]
>
>[注目のモーメントフローステップ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md)の使用を学びます。

## 使用可能なトークン{#available-tokens}

[Tokens Overview](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md)を調べて、おもしろい瞬間に使えるすべてのトークンを確認します。

## トリガートークン{#trigger-tokens}

スマートキャンペーンで使用されるトリガーに基づいて、追加のトリガートークンが使用可能になります。

* `{{trigger.Trigger Name}}` それは常に実際のトリガーそのものです次に例を示します。電子メール内のリンクをクリックします。
* `{{trigger.Name}}` は、キャンペーンをトリガーしたアセットの名前です。次に例を示します。「Webページ上のクリック数リンク」はURLであり、Salesforceトリガーなどの件名です。
* 制約に基づいて追加のトリガーを使用できます。以下に示します。

**電子メールトリガー**

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col>
  <col>
  <col>
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th><br></th> 
   <th><code>{{trigger.Trigger Name}}</code></th> 
   <th><code>{{trigger.Name}}</code></th> 
   <th><code>{{trigger.Link}}</code></th> 
   <th><code>{{trigger.Subject}}</code></th> 
   <th><code>{{trigger.Category}}</code></th> 
   <th><code>{{trigger.Details}}</code></th> 
   <th><code>{{trigger.Web Page}}</code></th> 
   <th><code>{{trigger.Client IP Address}}</code></th> 
   <th><code>{{trigger.Sent By}}</code></th> 
   <th><code>{{trigger.Received By}}</code></th> 
   <th><code>{{trigger.Referrer}}</code></th>
   <th><code>{{trigger.Search Engine}}</code></th>
   <th><code>{{trigger.Search Query}}</code></th>
   <th><code>{{trigger.Browser}}</code></th>
  </tr> 
  <tr> 
   <td>メール内リンクをクリック</td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>電子メールのバウンス（ハード）</td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>ソフトバウンスメール</td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>電子メールが配信される</td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>メールを開く</td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
    <tr> 
   <td>友達への転送メール受信</td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
    <tr> 
   <td>友達への転送メール送信</td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td>
  </tr> 
  <tr> 
   <td>メール配信停止</td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
 </tbody> 
</table>

**Salesforceトリガー**

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col>
  <col>
  <col>
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th><br></th> 
   <th><code>{{trigger.Trigger Name}}</code></th> 
   <th><code>{{trigger.Name}}</code></th> 
   <th><code>{{trigger.Link}}</code></th> 
   <th><code>{{trigger.Subject}}</code></th> 
   <th><code>{{trigger.Category}}</code></th> 
   <th><code>{{trigger.Details}}</code></th> 
   <th><code>{{trigger.Web Page}}</code></th> 
   <th><code>{{trigger.Client IP Address}}</code></th> 
   <th><code>{{trigger.Sent By}}</code></th> 
   <th><code>{{trigger.Received By}}</code></th> 
   <th><code>{{trigger.Referrer}}</code></th>
   <th><code>{{trigger.Search Engine}}</code></th>
   <th><code>{{trigger.Search Query}}</code></th>
   <th><code>{{trigger.Browser}}</code></th>
  </tr> 
  <tr> 
   <td>セールスメール内のリンクをクリック</td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>セールスメール送信</td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>セールスメールを開く</td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>セールスメールのバウンス</td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>セールスメールを受信</td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
    <tr> 
   <td>商談更新</td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
    <tr> 
   <td>所有者の変更</td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>顧客を変換</td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>担当者を SFDC から削除します</td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>担当者を SFDC に同期します</td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>商談から削除</td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>SFDC キャンペーンから削除</td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>活動の記録</td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>活動の更新</td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>商談に追加</td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>SFDC キャンペーンに追加</td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>SFDC キャンペーンでのステータス変更</td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
 </tbody> 
</table>

**Sales Connectトリガー**

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col>
  <col>
  <col>
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th><br></th> 
   <th><code>{{trigger.Trigger Name}}</code></th> 
   <th><code>{{trigger.Name}}</code></th> 
   <th><code>{{trigger.Link}}</code></th> 
   <th><code>{{trigger.Subject}}</code></th> 
   <th><code>{{trigger.Category}}</code></th> 
   <th><code>{{trigger.Details}}</code></th> 
   <th><code>{{trigger.Web Page}}</code></th> 
   <th><code>{{trigger.Client IP Address}}</code></th> 
   <th><code>{{trigger.Sent By}}</code></th> 
   <th><code>{{trigger.Received By}}</code></th> 
   <th><code>{{trigger.Referrer}}</code></th>
   <th><code>{{trigger.Search Engine}}</code></th>
   <th><code>{{trigger.Search Query}}</code></th>
   <th><code>{{trigger.Browser}}</code></th>
  </tr> 
  <tr> 
   <td>セールスメール内のリンクをクリック</td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>セールスメール送信</td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>セールスメールを開く</td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>セールスメールのバウンス</td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>セールスメールを受信</td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>セールスキャンペーンに追加しました</td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr>
   <td>所有者の変更</td> 
   <td>セールスキャンペーンから削除しました</td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>セールス電話を受信しました</td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
 </tbody> 
</table>

**その他**

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col>
  <col>
  <col>
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th><br></th> 
   <th><code>{{trigger.Trigger Name}}</code></th> 
   <th><code>{{trigger.Name}}</code></th> 
   <th><code>{{trigger.Link}}</code></th> 
   <th><code>{{trigger.Subject}}</code></th> 
   <th><code>{{trigger.Category}}</code></th> 
   <th><code>{{trigger.Details}}</code></th> 
   <th><code>{{trigger.Web Page}}</code></th> 
   <th><code>{{trigger.Client IP Address}}</code></th> 
   <th><code>{{trigger.Sent By}}</code></th> 
   <th><code>{{trigger.Received By}}</code></th> 
   <th><code>{{trigger.Referrer}}</code></th>
   <th><code>{{trigger.Search Engine}}</code></th>
   <th><code>{{trigger.Search Query}}</code></th>
   <th><code>{{trigger.Browser}}</code></th>
  </tr> 
  <tr> 
   <td>フォームの入力</td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>ウェブページにアクセス</td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>ウェブページのリンクをクリック</td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>チェック![(tick)](assets/check.svg)がない場合は、おもしろい瞬間に空の文字列（何もない）が返されます。

*トリガー&#x200B;**訪問ウェブページ**&#x200B;には、次のトークンがいくつか追加されています。

* `{{trigger.Referrer}}`
* `{{trigger.Search Engine}}`
* `{{trigger.Search Query}}`

>[!TIP]
>
>興味深い瞬間を必ずテストして、思いどおりにレンダリングされることを確認してください。
>
>また、セールス担当者にとって、お客様だけでなく、おもしろいことを確認してください。 ![（ウィンク）](assets/wink.svg)>
