---
solution: Marketo Engage
product: marketo
title: パーソナライゼーショントークン
description: メールDesignerでパーソナライゼーショントークンを使用する方法を説明します。 メールコンテンツに動的な受信者データを追加。
level: Beginner, Intermediate
feature: Email Designer
exl-id: 4828e1a5-822f-48a9-bbb8-b1ffe8421e4f
hide: true
TQID: https://experienceleague.adobe.com/2F6SP0sUvcScw0Y86X10nRTfL2b45krGTLeSi-td7Uc
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 263
ht-degree: 6%

---

# パーソナライゼーショントークン {#personalization-tokens}

メールデザイナーは、メールパーソナライゼーショントークンに関して、従来のメールエディターとは異なる形式を使用します。 この変更は、Handlebar スクリプトとの互換性を改善し、メール作成プロセスを合理化するために実装されました。

>[!AVAILABILITY]
>
>2025年5月23日（PT）以降、この機能はMarketo Engage ユーザーに一括でプロビジョニングされ、1週間に1つのリージョンが更新されます。 ロールアウト中、新しいメールデザイナーを使用して作成されたメールは、既存のトークンを新しい形式に自動的に移行します。 今回のアップデートでは、すべてのトークンが英語でのみ利用可能になります。

## プライマリの使用例 {#primary-use-case}

この機能強化は、主に[速度スクリプト &#x200B;](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/email-scripting){target="_blank"}からHandlebar スクリプトに移行するユーザーにメリットをもたらします。 新しい電子メールデザイナーは、新しいトークン形式のみをサポートしています。 更新された形式では、スペースが不要になり、デフォルトのテキスト構造が修正され、よりスムーズで効率的なスクリプト作成が可能になります。

## トークンエクスペリエンス {#token-experience}

古いものと新しいものの両方のトークン体験を調べます。

### 古い形式 {#old-format}

従来のメールエディターでは、`lead.Anonymous IP`や`member.registration code`などのスペースを含むトークンを追加できます。 既定のテキストの形式は`{{lead.City:default=fallback}}`でした

![](assets/personalization-tokens-1.png){width="800" zoomable="yes"}

### 新しい形式 {#new-format}

電子メールデザイナーでは、トークンに[&#x200B; キャメルケース &#x200B;](https://developer.mozilla.org/en-US/docs/Glossary/Camel_case)またはアンダースコア（`lead.anonymousIP`または`member.registration_code`など）を使用する必要があります。 既定のテキストの形式も`{%=lead.city ?: "fallback" %}`に変更されます。

![](assets/personalization-tokens-2.png){width="800" zoomable="yes"}

## 注意事項 {#things-to-note}

* パーソナライゼーションエディターには、オーサリングを容易にするための次の機能も搭載されています。

   * 取り消し/やり直し
   * 検索/検索と置換

* 以前Marketo Engageでサポートされていた&#x200B;**すべて**&#x200B;のトークンは、新しいパーソナライゼーションエディターでサポートされています。
