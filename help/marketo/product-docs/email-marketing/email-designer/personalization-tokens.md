---
solution: Marketo Engage
product: marketo
title: Personalizationトークン
description: 新しいMarketo Engage メールDesignerでパーソナライゼーショントークンを使用する方法を説明します
level: Beginner, Intermediate
hide: true
hidefromtoc: true
source-git-commit: 0abb2a7499541b8efbf3000bcd9fc9c1a79e43e1
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 1%

---

# Personalizationトークン {#personalization-tokens}

メールDesignerは、メールパーソナライゼーショントークンに関して、従来のメールエディターとは異なるフォーマットを使用します。 この変更は、Handlebar スクリプティングとの互換性を向上させ、メール作成プロセスを合理化するために実装されました。

>[!AVAILABILITY]
>
>2025 年 5 月 23 日（PT）以降、この機能は、Marketo Engage ユーザーに一括でプロビジョニングされ、1 週間に 1 つのリージョンが更新されます。 ロールアウト時に、新しいメールデザイナーを使用して作成されたメールは、既存のトークンを新しい形式に自動的に移行します。 この更新により、すべてのトークンが英語でのみ使用できるようになります。

## プライマリのユースケース {#primary-use-case}

この機能強化は、主に [Velocity スクリプティング ](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/email-scripting){target="_blank"} から Handlebar スクリプティングに移行するユーザーにメリットをもたらします。 新しいメールDesignerでは、新しいトークン形式のみをサポートしています。 更新された形式では、スペースが排除され、デフォルトのテキスト構造が改訂されて、よりスムーズで効率的なスクリプティング体験が提供されます。

## トークンエクスペリエンス {#token-experience}

古いトークンと新しいトークンの両方を確認します。

### 古いフォーマット {#old-format}

従来のメールエディターでは、`lead.Anonymous IP` や `member.registration code` などのスペースを使用してトークンを追加できます。 デフォルトのテキストの形式は `{{lead.City:default=fallback}}` でした。

![](assets/personalization-tokens-1.png){width="500" zoomable="yes"}

### 新しい形式 {#new-format}

電子メールデザイナーでは、[ キャメルケース ](https://developer.mozilla.org/en-US/docs/Glossary/Camel_case) や、トークンのアンダースコア（`lead.anonymousIP` や `member.registration_code` など）に適応する必要があります。 デフォルトテキストの形式も `{%=lead.city ?: "fallback" %}` に変更されます。

![](assets/personalization-tokens-2.png){width="600" zoomable="yes"}

## 注意事項 {#things-to-note}

* パーソナライゼーションエディターには、オーサリングを容易にする次の機能もあります。

   * 取り消し/やり直し
   * 検索/検索と置換
   * Autocomplete

* 以前にMarketo Engageでサポートされていた **すべて** トークンは、新しいパーソナライゼーションエディターでサポートされます。
