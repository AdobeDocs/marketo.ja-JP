---
unique-page-id: 1147344
description: Marketoのメールで使用できるシステムトークンについて説明します。 用語集を使用して、パーソナライゼーションに適したトークンを見つけます。
title: システムトークンの用語集
exl-id: 8a7694af-4edb-4b32-b408-19d2e7bd596e
feature: Tokens
source-git-commit: 7eb2f49718ea02be4a394a142c3a0ff05eeff796
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 85%

---

# システムトークンの用語集 {#system-tokens-glossary}

ユーザトークンに加えて、本当にクールなシステムトークンを使用できます。こちらです。

>[!NOTE]
>
>アカウントのタイムゾーン設定は、日時トークンが実行されるタイミングに影響します。

## system.date {#system-date}

`{{system.date}}` トークンは、実行時に現在の日付を **Aug 08, 2013** のようにレンダリングします。

**使用場所：**

* [データ値の変更](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"}フローステップ
* [注目のアクション](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"}フローステップ
* [タスクの作成](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"}フローステップ
* メールまたはテンプレートの本文

## system.time {#system-time}

`{{system.time}}` トークンは、実行時に **04:34PM （GMT -0700）のように現在の時刻をレンダリングします**

**使用場所：**

* [データ値の変更](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"}フローステップ
* [注目のアクション](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"}フローステップ
* [タスクの作成](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"}フローステップ
* メールまたはテンプレートの本文

## system.dateTime {#system-datetime}

`{{system.dateTime}}` トークンは、実行時に現在の日時を **2013-08-08 16:36:13** のようにレンダリングします。

**使用場所：**

* [データ値の変更](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"}フローステップ
* [注目のアクション](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"}フローステップ
* [タスクの作成](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"}フローステップ
* メールまたはテンプレートの本文

## system.unsubscribeLink {#system-unsubscribelink}

`{{system.unsubscribeLink}}` トークンを使用すると、メール内の登録解除リンクの配置を制御できます。

**使用場所：**

* [システムトークンをメールまたはテンプレートのリンクとして追加](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"}

## system.viewAsWebpageLink {#system-viewaswebpagelink}

`{{system.viewAsWebpageLink}}` トークンを使用すると、メール内の「Web ページとして表示」リンクの配置を制御できます。

**使用場所：**

* [システムトークンをメールまたはテンプレートのリンクとして追加](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"}
