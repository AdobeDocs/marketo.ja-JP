---
unique-page-id: 14352508
description: カスタム動的フィールドの作成 - Marketo ドキュメント - 製品ドキュメント
title: カスタム動的フィールドの作成
exl-id: 860511d2-4a8a-47a4-8362-ba4e715e44e9
source-git-commit: ''
workflow-type: ht
source-wordcount: '236'
ht-degree: 100%

---

# カスタム動的フィールドの作成 {#create-custom-dynamic-fields}

カスタム動的フィールドを作成する方法は 2 つあります。

## 1 つまたは複数の連絡先のカスタムフィールドの保存 {#saving-custom-fields-for-one-or-a-few-contacts}

1. リードページで連絡先の名前をクリックします。

1. 「登録解除」の横のドロップダウンを選択し、「**編集**」を選択します。

1. 下にスクロールして編集ページの下部に移動します。フィールドの名前と値を作成できます。

1. 「**保存**」をクリックします。

## 複数の連絡先のカスタムフィールドの保存 {#saving-custom-fields-for-many-contacts}

1. 独自の列にカスタムフィールドを含む CSV スプレッドシートを作成します。

1. [通常の CSV アップロードプロセス](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md)に従い、フィールドマッピング画面で停止します。

1. 事前設定されたフィールドではなく、「**新しいカスタムフィールドを追加**」をドロップダウンから選択します。

1. 目的のフィールド名を入力し、「**OK**」をクリックします。

1. CSV のアップロードが完了しました。連絡先に追加されたカスタムフィールドが表示されます。

>[!NOTE]
>
>カスタムフィールドを作成した後、テンプレートエディターの動的フィールドドロップダウンにフィールドが表示されるまで、約 30 分かかる場合があります。

## テンプレートでカスタムフィールドを使用する方法 {#how-to-use-your-custom-fields-in-a-template}

上記の方法を使用してカスタムフィールドを保存したら、テンプレートで参照できます。

1. [テンプレートを作成](/help/marketo/product-docs/marketo-sales-connect/templates/create-a-new-template.md)し、通常どおりに「**動的フィールド**」ボタンをクリックします。

1. 表示されるドロップダウンから「**カスタムフィールド**」を選択します。

1. 事前に保存されているカスタムフィールドが表示され、テンプレートに入力するカスタムフィールドを選択できます。
