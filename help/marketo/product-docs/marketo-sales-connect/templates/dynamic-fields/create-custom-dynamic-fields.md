---
unique-page-id: 14352508
description: カスタム動的フィールドの作成 —Marketoドキュメント — 製品ドキュメント
title: カスタム動的フィールドの作成
exl-id: 860511d2-4a8a-47a4-8362-ba4e715e44e9
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# カスタム動的フィールドの作成{#create-custom-dynamic-fields}

カスタムダイナミックフィールドを作成する方法は2つあります。

## 1人または数人の連絡先用のカスタムフィールドの保存{#saving-custom-fields-for-one-or-a-few-contacts}

1. 「人」ページで、連絡先の名前をクリックします。

1. 「登録解除」の横のドロップダウンを選択し、「**編集**」を選択します。

1. 編集ページの一番下までスクロールします。 その後、フィールドの名前と値を作成できます。

1. 「**保存**」をクリックします。

## 多数の連絡先用のカスタムフィールドを保存する{#saving-custom-fields-for-many-contacts}

1. 独自の列にカスタムフィールドを含むCSVスプレッドシートを作成します。

1. [通常のCSVアップロードプロセス](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md)に従い、フィールドマッピング画面で終了します。

1. プリセットフィールドの1つの代わりに、ドロップダウンから追加新しいカスタムフィールド&#x200B;**を選択します。**

1. 目的のフィールド名を入力し、「**OK**」をクリックします。

1. CSVのアップロードを完了します。 ユーザー設定フィールドが追加された連絡先が表示されます。

>[!NOTE]
>
>カスタムフィールドを作成した後、テンプレートエディターの動的フィールドドロップダウンにフィールドが表示されるまでに約30分かかる場合があります。

## テンプレートでのカスタムフィールドの使用方法{#how-to-use-your-custom-fields-in-a-template}

上記の方法を使用してカスタムフィールドを保存すると、テンプレートでそれらを参照できます。

1. [テン](/help/marketo/product-docs/marketo-sales-connect/templates/create-a-new-template.md) プレートを作成し、通常と同じように **動的** フィールドボタンをクリックします。

1. 表示されるドロップダウンから[**カスタムフィールド**]を選択します。

1. 事前に保存されているカスタムフィールドが表示され、テンプレートに入力するフィールドを選択できます。
