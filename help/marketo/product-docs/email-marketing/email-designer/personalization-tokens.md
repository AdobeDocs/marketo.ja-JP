---
solution: Marketo Engage
product: marketo
title: パーソナライゼーショントークン
description: 新しいMarketo Engage メールDesignerでパーソナライゼーショントークンを使用する方法を説明します
level: Beginner, Intermediate
feature: Email Designer
exl-id: 4828e1a5-822f-48a9-bbb8-b1ffe8421e4f
hide: true
hidefromtoc: true
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '243'
ht-degree: 3%

---

# パーソナライゼーショントークン {#personalization-tokens}

メールデザイナーは、メールのパーソナライゼーショントークンに関して、従来のメールエディターとは異なる形式を使用します。 この変更は、Handlebar スクリプティングとの互換性を向上させ、メール作成プロセスを合理化するために実装されました。

>[!AVAILABILITY]
>
>2025 年 5 月 23 日（PT）以降、この機能は、Marketo Engage ユーザーに一括でプロビジョニングされ、1 週間に 1 つのリージョンが更新されます。 ロールアウト時に、新しいメールデザイナーを使用して作成されたメールは、既存のトークンを新しい形式に自動的に移行します。 この更新により、すべてのトークンが英語でのみ使用できるようになります。

## プライマリのユースケース {#primary-use-case}

この機能強化は、主に [Velocity スクリプティング ](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/email-scripting){target="_blank"} から Handlebar スクリプティングに移行するユーザーにメリットをもたらします。 新しい電子メールデザイナーでは、新しいトークン形式のみをサポートしています。 更新された形式では、スペースが排除され、デフォルトのテキスト構造が改訂されて、よりスムーズで効率的なスクリプティング体験が提供されます。

## トークンエクスペリエンス {#token-experience}

古いトークンと新しいトークンの両方を確認します。

### 古いフォーマット {#old-format}

従来のメールエディターでは、`lead.Anonymous IP` や `member.registration code` などのスペースを使用してトークンを追加できます。 デフォルトのテキストの形式は `{{lead.City:default=fallback}}` でした。

![](assets/personalization-tokens-1.png){width="800" zoomable="yes"}

### 新しい形式 {#new-format}

電子メールデザイナーでは、[ キャメルケース ](https://developer.mozilla.org/en-US/docs/Glossary/Camel_case) またはトークンのアンダースコア（`lead.anonymousIP` や `member.registration_code` など）を使用する必要があります。 デフォルトテキストの形式も `{%=lead.city ?: "fallback" %}` に変更されます。

![](assets/personalization-tokens-2.png){width="800" zoomable="yes"}

## 注意事項 {#things-to-note}

* パーソナライゼーションエディターには、オーサリングを容易にする次の機能もあります。

   * 取り消し/やり直し
   * 検索/検索と置換
   * Autocomplete

* 以前にMarketo Engageでサポートされていた **すべて** トークンは、新しいパーソナライゼーションエディターでサポートされます。
