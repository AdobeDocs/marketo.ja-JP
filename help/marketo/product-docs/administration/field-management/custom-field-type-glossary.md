---
unique-page-id: 2951259
description: カスタムフィールドタイプ用語集 — Marketto Docs — 製品ドキュメント
title: カスタムフィールドタイプ用語集
translation-type: tm+mt
source-git-commit: f865630638e7c0fe6ac2a449e196a7de4fbfeea1
workflow-type: tm+mt
source-wordcount: '583'
ht-degree: 0%

---


# カスタムフィールドタイプ用語集{#custom-field-type-glossary}

マーケティングでカスタムフィールドを作成する場合は、タイプをリストして選択できます。

>[!PREREQUISITES]
>
>[Marketorでのカスタムフィールドの作成](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)

>[!TIP]
>
>フィールドのタイプに応じて、フィルタ/トリガー[演算子](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/smart-list-filter-operators-glossary.md)は異なります。

>[!NOTE]
>
>ほとんどのフィールドは、最大文字数ではなく、バイト数です。 そのため、各フィールドに最終的な文字制限を設けることはできません。 例外は&#x200B;**String**&#x200B;で、最大255文字です。

## ブール値{#boolean}

**名前の例：** is Customer — ユーザーに顧客のタグを付ける

**例：** True（チェック済み）/False（チェックなし）

**演算子**:なし

## 通貨{#currency}

**例名：** Budget -会社の予算に対する数値を格納する

**値の例：** 100

**演算子**:が次の値を超える、次の値を超えない、次の値を超える、次よりも小さい、最低でも多い、最大でも空でない、

## 日付{#date}

**名前の例：** 更新日 — 顧客の更新日を保存する

**値の例：** 8/19/14

**演算子**:がIs、Not Between、Pess Between、Pess Before、Future In、In time frame、After、OnまたはBefore、Emptyの場合、空ではありません

## 日時{#datetime}

**例名：** 作成日 — 人が作成された日時を格納します。

**値の例：** 8/19/14 2:00

**演算子**:がIs、Not Between、Pess Between、Pess Before、Future In、In time frame、After、OnまたはBefore、Emptyの場合、空ではありません

## 電子メール{#email}

**例名：** 代替電子メール — ユーザーの代替電子メールアドレスを保持します（実際には、デフォルトの電子メールアドレスフィールドのように、特別な電子メールアドレスをこのフィールドに送信することはできません）

**値の例：** name@company.com

**演算子**:がis、is、not、がある開始、not開始と、contains、not contains、is empty、not empty

## 浮動小数点{#float}

**例名：** 等級ポイント平均 — 個人の等級ポイント平均または小数点を持つその他の数値を保持します。

**値の例：** 2.47

**演算子**:between、greater than、less、least than、lest、mast、empty、not empty

## 数式{#formula}

**例：** 挨拶 — この特別なフィールドを [ソリューションで使用して、性別に基づいて適切な](/help/marketo/product-docs/administration/field-management/create-and-use-a-concatenated-string-formula-field.md) 挨拶を得ます。

**例の値：リンクされたソリューションの** 確認

## 整数{#integer}

**例名：従業員** 数 — 小数を必要としない数値を格納する

**値の例：** 600

**演算子**:が次の値を超える、次の値を超えない、次の値を超える、次よりも小さい、最低でも多い、最大でも空でない、

## パーセント{#percent}

**例名：** 購入する可能性が高い — 割合の値を格納する（おそらくCRM側で計算される）

**値の例：** 85%

**演算子**:が次の値を超える、次の値を超えない、次の値を超える、次よりも小さい、最低でも多い、最大でも空でない、

## 電話{#phone}

**例名：** 代替電話 — ユーザーに追加の電話番号を保存する

**例値：** 650-555-5555

**演算子**:がis、is、not、がある開始、not開始と、contains、not contains、is empty、not empty

## スコア{#score}

**例名：** 行動スコア/人口統計スコア — 複数のスコアフィールドを作成して、異なる属性を追跡します。

**値の例：** 14

**演算子**:が次の値を超える、次の値を超えない、次の値を超える、次よりも小さい、最低でも多い、最大でも空でない、

## 文字列{#string}

**例名：** ミドルネーム — 追加のテキスト属性を格納する

**値の例：** Rose

**演算子**:がis、is、not、がある開始、not開始と、contains、not contains、is empty、not empty

## テキスト領域{#text-area}

**例名：** コメント — 複数行にわたるテキストの入力を許可するために、フォームにコメントフィールドを追加します。

**値の例：** この記事は素晴らしい！

**演算子**:がis、is、not、がある開始、not開始と、contains、not contains、is empty、not empty

## URL {#url}

**例名：** ブログ — 個人のブログURLを格納するフィールドの作成

**値の例：** www.myblog.com

**演算子**:がis、is、not、がある開始、not開始と、contains、not contains、is empty、not empty
