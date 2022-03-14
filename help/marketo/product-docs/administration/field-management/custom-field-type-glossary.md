---
unique-page-id: 2951259
description: カスタムフィールドタイプの用語集 - Marketo ドキュメント - 製品ドキュメント
title: カスタムフィールドタイプの用語集
exl-id: 495d4deb-28f1-4044-98d3-27c20756fe73
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '583'
ht-degree: 100%

---

# カスタムフィールドタイプの用語集 {#custom-field-type-glossary}

Marketo でカスタムフィールドを作成する場合、タイプのリストから選択できます。

>[!PREREQUISITES]
>
>[Marketo でのカスタムフィールドの作成](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)

>[!TIP]
>
>フィールドタイプに応じて、フィルター／トリガー[演算子](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/smart-list-filter-operators-glossary.md)は異なる値になります。

>[!NOTE]
>
>ほとんどのフィールドの上限は、文字数ではなくてバイト数です。そのため、各フィールドで確定的な文字制限を指定できません。例外は&#x200B;**文字列**（最大 255 文字）です。

## ブール値 {#boolean}

**名前の例**：Is Customer — 顧客を顧客としてタグ付けします

**値の例**：True（オン）／False（オフ）

**演算子**：なし

## 通貨 {#currency}

**名前の例**：Budget — 会社の予算に対する数値を格納します

**値の例**：100

**演算子**：is、not、between、greater、less than、at least、at most、is empty、is not empty

## 日 {#date}

**名前の例：** Renewal Date — 顧客の更新日を保存します

**値の例：** 8/19/14

**演算子**：is、not、between、in past、in past before、in future、in future after、in time frame、after、before、on or after、on or before、is empty、is not empty

## 日時 {#datetime}

**名前の例**：Created Date — ユーザーが作成された日時を保存します

**値の例**：8/19/14 2:00

**演算子**：is、not、between、in past、in past before、in future、in future after、in time frame、after、before、on or after、on or before、is empty、is not empty

## メール {#email}

**名前の例**：Alternate Email — ユーザーの代替メールアドレスを保持します（デフォルトのメールアドレスフィールドのように、実際にはこのフィールドにメールを送信することはできません。特別なメールです）

**値の例**：name@company.com

**演算子**：is、is not、starts with、not starts with、contains、not contains、is empty、is not empty

## 浮動 {#float}

**名前の例**：Grade Point Average — ユーザーの等級ポイント平均または小数点を持つその他の数値を保持します

**値の例**：2.47

**演算子**：between、greater than、less than、at least、at most、is empty、is not empty

## 数式 {#formula}

**名前の例**：Salutations — この特殊なフィールドを性別に基づく[適切な敬称を得るための解決策](/help/marketo/product-docs/administration/field-management/create-and-use-a-concatenated-string-formula-field.md)を得るために使用します

**値の例**：リンクされたソリューションを確認してください

## 整数 {#integer}

**名前の例**：Number of Employees — 小数を必要としない数値を格納します

**値の例**：600

**演算子**：is、not、between、greater、less than、at least、at most、is empty、is not empty

## パーセント {#percent}

**名前の例**：Likely To Buy - 割合値を保存します（おそらく CRM 側で計算）

**値の例**：85%

**演算子**：is、not、between、greater、less than、at least、at most、is empty、is not empty

## 電話 {#phone}

**名前の例**：Alternate Phone - ユーザーの代替電話番号を格納します

**値の例**：650-555-5555

**演算子**：is、is not、starts with、not starts with、contains、not contains、is empty、is not empty

## スコア {#score}

**名前の例**：Behavioral Score／Demographic Score - 異なる属性を追跡するために複数のスコアフィールドを作成します

**値の例**：14

**演算子**：is、not、between、greater、less than、at least、at most、is empty、is not empty

## 文字列 {#string}

**名前の例**：Middle Name - 追加のテキスト属性を格納します

**値の例**：Rose

**演算子**：is、is not、starts with、not starts with、contains、not contains、is empty、is not empty

## テキストエリア {#text-area}

**名前の例**：Comments - 複数行テキストを入力できるように、フォームにコメントフィールドを追加します

**値の例**：This article is fantastic!

**演算子**：is、is not、starts with、not starts with、contains、not contains、is empty、is not empty

## URL {#url}

**名前の例**：Blog - ユーザーブログ URL を格納するフィールドを作成します

**値の例**：www.myblog.com

**演算子**：is、is not、starts with、not starts with、contains、not contains、is empty、is not empty
