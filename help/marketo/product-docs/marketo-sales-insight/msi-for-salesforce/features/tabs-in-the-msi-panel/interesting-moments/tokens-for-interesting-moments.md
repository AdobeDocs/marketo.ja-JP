---
unique-page-id: 1146999
description: 興味深い瞬間のトークン — Marketto Docs — 製品ドキュメント
title: 興味深い瞬間のトークン
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 0%

---


# 興味深い瞬間のトークン {#tokens-for-interesting-moments}

>[!NOTE]
>
>**前提条件**
>
>* 注 [目の瞬間のフローステップの使用方法を学びます](../../../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md)。
>* トー [クンの詳細](http://docs.marketo.com/display/docs/tokens)。

>



## 使用可能なトークン {#available-tokens}

「 [トークンの概要](../../../../../../product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) 」をチェックして、興味深い瞬間に使えるすべてのトークンを確認します。

## トークンのトリガー {#trigger-tokens}

スマートキャンペーンで使用されるトリガーに基づいて、追加のトリガートークンが使用可能になります。

* `{{trigger.Trigger Name}}` これは常に実際のトリガです。 次に例を示します。電子メール内のリンクをクリックします。
* `{{trigger.Name}}` は、キャンペーンをトリガーしたアセットの名前です。 次に例を示します。「Webページ上のクリック数リンク」はURLであり、Salesforceトリガーなどの件名です。
* 制約に基づいて、追加のトリガーを使用できます。以下に示します。

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
  </tr> 
  <tr> 
   <td>電子メール内のリンクをクリック</td> 
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
  </tr> 
  <tr> 
   <td>電子メールのバウンス（ソフト）</td> 
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
  </tr> 
  <tr> 
   <td>電子メールを開く</td> 
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
  </tr> 
  <tr> 
   <td>電子メールから登録解除</td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>販売の電子メール内のクリック数リンク</td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>送信済みの販売メール</td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>販売の電子メールを開きます</td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>受信した販売の電子メール</td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
  </tr> 
  <tr> 
   <td colspan="1">販売の電子メールがバウンス</td> 
   <td colspan="1"><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td colspan="1"><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
  </tr> 
  <tr> 
   <td>Fills Out Form</td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td><br></td> 
   <td><p><br></p></td> 
  </tr> 
  <tr> 
   <td colspan="1">訪問回数ウェブページ*</td> 
   <td colspan="1"><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><img src="assets/check.svg" alt="（目盛り）"></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>チェック ![（ティック）がない場合](assets/check.svg) 、おもしろい瞬間に空の文字列（何もない）が返される。

*[ **訪問のトリガ]ウェブページには** 、次のトークンがいくつか追加されています。

* `{{trigger.Referrer}}`
* `{{trigger.Search Engine}}`
* `{{trigger.Search Query}}`

>[!TIP]
>
>興味深い瞬間を必ずテストして、思いどおりにレンダリングされることを確認してください。
>
>また、セールス担当者にとって、お客様だけでなく、おもしろいことを確認してください。 ![（ウィンク）](assets/wink.svg)>

