---
unique-page-id: 2951259
description: ブール値、通貨、日付、電子メール、数式など、Marketoのカスタムフィールドタイプのリファレンスです。
title: カスタムフィールドタイプの用語集
exl-id: 495d4deb-28f1-4044-98d3-27c20756fe73
feature: Field Management
source-git-commit: cbf6c6c480eb9959f4f1f8367deffcef2728f068
workflow-type: tm+mt
source-wordcount: '601'
ht-degree: 61%

---

# カスタムフィールドタイプの用語集 {#custom-field-type-glossary}

Marketoでカスタムフィールドを作成する場合は、選択できるタイプのリストがあります。

>[!PREREQUISITES]
>
>[Marketo でのカスタムフィールドの作成](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)

>[!TIP]
>
>フィールドタイプに応じて、フィルター／トリガー[演算子](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/smart-list-filter-operators-glossary.md)は異なる値になります。

>[!NOTE]
>
>ほとんどのフィールドは、文字数ではなく、バイト数で最大化されます。 そのため、Marketoでは各フィールドに対して最終的な文字制限を指定できません。 例外は&#x200B;**文字列**（最大 255 文字）です。

## ブール値 {#boolean}

**名前の例：**&#x200B;は顧客 – ユーザーを顧客としてタグ付け

**値の例**：True（オン）／False（オフ）

**演算子**：なし

## 通貨 {#currency}

**名前の例**：Budget — 会社の予算に対する数値を格納します

**値の例**：100

**演算子**：is、not、between、greater、less than、at least、at most、is empty、is not empty

## 日 {#date}

**例：名前：**&#x200B;更新日 – 顧客の更新日を保存

**値の例：** 8/19/14

**演算子**：is、not、between、in past、in past before、in future、in future after、in time frame、after、before、on or after、on or before、is empty、is not empty

## 日時 {#datetime}

**名前の例**：Created Date — ユーザーが作成された日時を保存します

**値の例：** 8/19/14 2:00

**演算子**：is、not、between、in past、in past before、in future、in future after、in time frame、after、before、on or after、on or before、is empty、is not empty

## メール {#email}

**例：名前：**&#x200B;代替電子メール – 人物の代替メールアドレスを保持します（デフォルトの電子メールアドレス フィールドのように、実際にこのフィールドに電子メールを送信することはできません）

**値の例：** <name@company.com>

**演算子**：is、is not、starts with、not starts with、contains、not contains、is empty、is not empty

## 浮動 {#float}

**名前の例**：Grade Point Average — ユーザーの等級ポイント平均または小数点を持つその他の数値を保持します

**値の例**：2.47

**演算子**：between、greater than、less than、at least、at most、is empty、is not empty

## 数式 {#formula}

**例の名前：**&#x200B;件の挨拶 – [&#x200B; ソリューションでこの特別なフィールドを使用して、性別に基づいて適切な挨拶](/help/marketo/product-docs/administration/field-management/create-and-use-a-concatenated-string-formula-field.md)を取得します

**値の例：** リンクされたソリューションを確認する

## 整数 {#integer}

**例：名前：**&#x200B;従業員数 – 10進数を必要としない数値を格納します

**値の例**：600

**演算子**：is、not、between、greater、less than、at least、at most、is empty、is not empty

## パーセント {#percent}

**サンプル名：**&#x200B;購入する可能性があります – パーセント値を格納します（CRMで計算）

**値の例**：85%

**演算子**：is、not、between、greater、less than、at least、at most、is empty、is not empty

## 電話 {#phone}

**名前の例：**&#x200B;代替電話 – 追加の電話番号をユーザーに保存します

**値の例**：650-555-5555

**演算子**：is、is not、starts with、not starts with、contains、not contains、is empty、is not empty

## スコア {#score}

**例の名前：**&#x200B;行動スコア / デモグラフィックスコア – 複数のスコアフィールドを作成して、異なる属性を追跡します

**値の例**：14

**演算子**：is、not、between、greater、less than、at least、at most、is empty、is not empty

## 文字列 {#string}

**サンプル名：** ミドル名 – 追加のテキスト属性を格納します

**値の例**：Rose

**演算子**：is、is not、starts with、not starts with、contains、not contains、is empty、is not empty

## テキストエリア {#text-area}

**サンプル名：** コメント – 複数行のテキスト入力を許可するために、フォームにコメントフィールドを追加します

**値の例**：This article is fantastic!

**演算子**：is、is not、starts with、not starts with、contains、not contains、is empty、is not empty

## URL {#url}

**例の名前：** ブログ – 個人のブログ URLを保存するフィールドを作成します

**値の例：** &lt;www.myblog.com>

**演算子**：is、is not、starts with、not starts with、contains、not contains、is empty、is not empty
