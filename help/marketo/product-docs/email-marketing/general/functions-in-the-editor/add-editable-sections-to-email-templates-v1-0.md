---
unique-page-id: 1900585
description: v1.0 でメールテンプレートに編集可能なセクションを追加する方法を説明します。残りの領域をロックしたまま、特定の領域を編集できるようにします。
title: メールテンプレート v1.0 に編集可能なセクションを追加する
exl-id: f397aa8e-0d0b-4007-91e1-9b9158bd6432
feature: Email Editor
source-git-commit: 7eb2f49718ea02be4a394a142c3a0ff05eeff796
workflow-type: tm+mt
source-wordcount: '110'
ht-degree: 80%

---

# メールテンプレート v1.0 に編集可能なセクションを追加する {#add-editable-sections-to-email-templates-v1.0}

メールテンプレートエディター v1.0 でテンプレートを作成している場合は、任意のセクションを特別な `<div>` で囲んで編集可能にすることができます。

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
