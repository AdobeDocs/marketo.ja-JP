---
unique-page-id: 1900585
description: 電子メールテンプレートv1.0 - Marketto Docs — 製品ドキュメントに編集可能な追加セクション
title: 電子メールテンプレートv1.0に追加編集可能なセクション
translation-type: tm+mt
source-git-commit: f27e2bac90570f9f795dc6bdd5fcf208c446be14
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 0%

---


# 電子メールテンプレートv1.0に追加編集可能なセクション {#add-editable-sections-to-email-templates-v1.0}

Email Template Editor v1.0でテンプレートを作成する場合は、セクションの周囲に特別な文字を配置することで、任意のセクションを編集可能にするこ `<div>` とができます。

>[!NOTE]
>
>**例**
>`<pre> <div class="mktEditable" id="UNIQUE_ID">This part is editable</div></pre>`

ルール：

1. HTMLは常に有効である必要があります。
1. mktEditableのクラスを含める **必要があります** 。
1. IDは、そのHTML内で一意である必要があります。
1. IDにスペースは含めません。

>[!CAUTION]
>
>mktEditableステートメントは入れ子にできません。

電子メールテンプレートエディタv2.0でこの方法を学習する場合は、 [電子メールテンプレートの構文をチェックアウトします](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md)。
