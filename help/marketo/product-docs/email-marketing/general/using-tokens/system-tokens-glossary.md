---
unique-page-id: 1147344
description: システムトークンの用語集 — Marketo ドキュメント — 製品ドキュメント
title: システムトークンの用語集
exl-id: 8a7694af-4edb-4b32-b408-19d2e7bd596e
source-git-commit: 93032a016a67fe0edf7a8093633d6b06ec25c18d
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 55%

---

# システムトークンの用語集 {#system-tokens-glossary}

ユーザートークンに加えて、本当にクールなシステムトークンを使用できます。こちらです。

>[!NOTE]
>
>アカウントのタイムゾーン設定は、日時トークンが実行されるタイミングに影響します。

## system.date {#system-date}

`{{system.date}}` トークンは、実行時に現在の日付を **Aug 08, 2013** のようにレンダリングします。

**使用場所：**

* [データ値の変更](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target=&quot;_blank&quot;} フローステップ
* [注目のアクション](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target=&quot;_blank&quot;} フローステップ
* [タスクを作成](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target=&quot;_blank&quot;} フローステップ
* メールまたはテンプレートの本文

## system.time {#system-time}

`{{system.time}}` トークンは、実行時に現在時刻を **04:34 PM (GMT -0700)** のようにレンダリングします。

**使用場所：**

* [データ値の変更](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target=&quot;_blank&quot;} フローステップ
* [注目のアクション](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target=&quot;_blank&quot;} フローステップ
* [タスクを作成](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target=&quot;_blank&quot;} フローステップ
* メールまたはテンプレートの本文

## system.dateTime {#system-datetime}

`{{system.dateTime}}` トークンは、実行時に現在の日時を **2013-08-08 16:36:13** のようにレンダリングします。

**使用場所：**

* [データ値の変更](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target=&quot;_blank&quot;} フローステップ
* [注目のアクション](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target=&quot;_blank&quot;} フローステップ
* [タスクを作成](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target=&quot;_blank&quot;} フローステップ
* メールまたはテンプレートの本文

## system.forwardToFriendLink {#system-forwardtofriendlink}

この `{{system.forwardToFriendLink}}` トークンを使用すると、 [メール内の「友達リンクに転送」](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/forward-to-a-friend-link-in-emails.md){target=&quot;_blank&quot;}。

**使用場所：**

* [システムトークンをメール内のリンクとして追加する](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target=&quot;_blank&quot;} またはテンプレート

## system.unsubscribeLink {#system-unsubscribelink}

`{{system.unsubscribeLink}}` トークンを使用すると、メール内の登録解除リンクの配置を制御できます。

**使用場所：**

* [システムトークンをメール内のリンクとして追加する](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target=&quot;_blank&quot;} またはテンプレート

## system.viewAsWebpageLink {#system-viewaswebpagelink}

`{{system.viewAsWebpageLink}}` トークンを使用すると、メール内の「Web ページとして表示」リンクの配置を制御できます。

**使用場所：**

* [システムトークンをメール内のリンクとして追加する](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target=&quot;_blank&quot;} またはテンプレート
