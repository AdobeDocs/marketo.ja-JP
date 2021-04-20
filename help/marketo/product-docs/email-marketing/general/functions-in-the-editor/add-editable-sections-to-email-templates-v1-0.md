---
unique-page-id: 1900585
description: 電子メールテンプレートv1.0 -Marketoドキュメント — 製品ドキュメントに編集可能な追加セクション
title: 電子メールテンプレートv1.0に追加編集可能なセクション
exl-id: f397aa8e-0d0b-4007-91e1-9b9158bd6432
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 2%

---

# 電子メールテンプレートv1.0 {#add-editable-sections-to-email-templates-v1.0}追加に編集可能なセクション

Email Template Editor v1.0でテンプレートを作成している場合は、特別な`<div>`を囲むことで、任意のセクションを編集可能にできます。

>[!NOTE]
>
>**例**
>
>`<pre> <div class="mktEditable" id="UNIQUE_ID">This part is editable</div></pre>`

ルール:

1. HTMLは常に有効である必要があります。
1. **mktEditable**&#x200B;のクラスを含める必要があります。
1. IDは、そのHTML内で一意である必要があります。
1. IDにスペースは含めません。

>[!CAUTION]
>
>mktEditableステートメントは入れ子にできません。

電子メールテンプレートエディタv2.0でこの方法を学ぶには、[電子メールテンプレート構文](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md)を参照してください。
