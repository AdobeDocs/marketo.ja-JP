---
unique-page-id: 14352508
description: カスタム動的フィールドの作成 - Marketo ドキュメント - 製品ドキュメント
title: カスタム動的フィールドの作成
exl-id: 860511d2-4a8a-47a4-8362-ba4e715e44e9
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 91%

---

# カスタム動的フィールドの作成 {#create-custom-dynamic-fields}

カスタム動的フィールドを作成する方法は 2 つあります。

## 1 つまたは複数の連絡先のカスタムフィールドの保存 {#saving-custom-fields-for-one-or-a-few-contacts}

1. [!UICONTROL  人物 ] ページで連絡先の名前をクリックします。

1. [!UICONTROL  登録解除 ] の横のドロップダウンを選択し、「**[!UICONTROL 編集]**」を選択します。

1. 下にスクロールして編集ページの下部に移動します。フィールドの名前と値を作成できます。

1. 「**[!UICONTROL 保存]**」をクリックします。

## 複数の連絡先のカスタムフィールドの保存 {#saving-custom-fields-for-many-contacts}

1. 独自の列にカスタムフィールドを含む CSV スプレッドシートを作成します。

1. [通常の CSV アップロードプロセス](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md)に従い、フィールドマッピング画面で停止します。

1. 事前設定されたフィールドではなく、「**[!UICONTROL 新しいカスタムフィールドを追加]**」をドロップダウンから選択します。

1. 目的のフィールド名を入力し、「**[!UICONTROL OK]**」をクリックします。

1. CSV のアップロードが完了しました。連絡先に追加されたカスタムフィールドが表示されます。

>[!NOTE]
>
>カスタムフィールドを作成した後、テンプレートエディターの動的フィールドドロップダウンにフィールドが表示されるまで、約 30 分かかる場合があります。

## テンプレートでカスタムフィールドを使用する方法 {#how-to-use-your-custom-fields-in-a-template}

上記の方法を使用してカスタムフィールドを保存したら、テンプレートで参照できます。

1. [テンプレートを作成](/help/marketo/product-docs/marketo-sales-connect/templates/create-a-new-template.md)し、通常どおりに「**[!UICONTROL 動的フィールド]**」ボタンをクリックします。

1. 表示されるドロップダウンから「**[!UICONTROL カスタムフィールド]**」を選択します。

1. 事前に保存されているカスタムフィールドが表示され、テンプレートに入力するカスタムフィールドを選択できます。
