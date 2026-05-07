---
unique-page-id: 1900585
description: v1.0で編集可能なセクションをメールテンプレートに追加する方法について説明します。 特定の領域を編集しながら、他の領域をロックできます。
title: メールテンプレート v1.0 に編集可能なセクションを追加する
exl-id: f397aa8e-0d0b-4007-91e1-9b9158bd6432
feature: Email Editor
source-git-commit: 240b78561db11e169188698880d4707a5c1f64de
workflow-type: tm+mt
source-wordcount: '111'
ht-degree: 59%

---

# メールテンプレート v1.0 に編集可能なセクションを追加する {#add-editable-sections-to-email-templates-v1.0}

メールテンプレートエディターv1.0でテンプレートを作成する場合、その周りに特別な`<div>`を配置することで、任意のセクションを編集可能にすることができます。

>[!NOTE]
>
>**例**
>
>`<pre> <div class="mktEditable" id="UNIQUE_ID">This part is editable</div></pre>`

ルール：

1. HTML は常に有効である必要があります。
1. **mktEditable** のクラスを含める必要があります。
1. この ID は、その HTML 内で一意である必要があります。
1. ID にスペースを含めることはできません。

>[!CAUTION]
>
>mktEditable ステートメントはネストできません。

メールテンプレートエディター v2.0 でこれをおこなう方法については、[メールテンプレート構文](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md)を参照してください。
