---
unique-page-id: 2951259
description: カスタムフィールドタイプ用語集 — Marketto Docs — 製品ドキュメント
title: カスタムフィールドタイプ用語集
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 0%

---


# カスタムフィールドタイプ用語集 {#custom-field-type-glossary}

>[!NOTE]
>
>**FYI**
>
>Marketoは現在、すべての購読で言語を標準化しているので、購読およびdocs.marketo.comの人物/人物にリード/リードを表示できます。 これらの用語は同じことを意味し、記事の説明には影響しません。 他にも変化がある。 [詳細情報](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

マーケティングでカスタムフィールドを作成する場合は、タイプをリストして選択できます。

>[!NOTE]
>
>**前提条件**
>
>* [Marketorでのカスタムフィールドの作成](create-a-custom-field-in-marketo.md)

>



>[!TIP]
>
>フィールドのタイプに応じて、フィルター/トリガー [演算子](https://docs.marketo.com/display/public/DOCS/Smart+List+Filter+Operators+Glossary) は異なります。

>[!NOTE]
>
>ほとんどのフィールドは、最大文字数ではなく、バイト数です。 そのため、各フィールドに最終的な文字制限を設けることはできません。 例外は **String**&#x200B;で、最大255文字です。

## ブール値 {#boolean}

**名前の例：** お客様：ユーザーを顧客としてタグ付け

**値の例：** True（チェック済み）/False（チェックなし）

**演算子**:なし

## 通貨 {#currency}

**名前の例：** 予算 —会社の予算の数値を格納します。

**値の例：** 100

**演算子**:が次の値を超える、次の値を超えない、次の値を超える、次よりも小さい、最低でも多い、最大でも空でない、

## 日付 {#date}

**名前の例：** 更新日 — お客様の更新日を保存します。

**値の例：** 8/19/14

**演算子**:がIs、Not Between、Pess Between、Pess Before、Future In、In time frame、After、OnまたはBefore、Emptyの場合、空ではありません

## 日時 {#datetime}

**名前の例：** 作成日 — 個人が作成された日時を保存します。

**値の例：** 8/19/14 2:00

**演算子**:がIs、Not Between、Pess Between、Pess Before、Future In、In time frame、After、OnまたはBefore、Emptyの場合、空ではありません

## 電子メール {#email}

**名前の例：** 代替電子メール — ユーザーの代替電子メールアドレスを保持します（デフォルトの電子メールアドレスフィールドのように、実際にはこのフィールドに電子メールを送信できません。特別な電子メールです）

**値の例：** [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#335d525e5673505c5e43525d4a1d505c5e)

**演算子**:がis、is、not、がある開始、not開始と、contains、not contains、is empty、not empty

## 浮動小数点 {#float}

**名前の例：** 等級ポイント平均 — 個人の等級ポイント平均または小数を持つその他の数値を保持します。

**値の例：** 2.47

**演算子**:between、greater than、less、least than、lest、mast、empty、not empty

## 数式 {#formula}

**名前の例：** 挨拶 — この特別なフィールドを [ソリューションで使用して、性別に基づいて適切な挨拶](create-and-use-a-concatenated-string-formula-field.md) を行います。

**値の例：** リンクされた解決策を確認する

## 整数 {#integer}

**名前の例：** 従業員数 — 小数を必要としない数値を格納します。

**値の例：** 600

**演算子**:が次の値を超える、次の値を超えない、次の値を超える、次よりも小さい、最低でも多い、最大でも空でない、

## パーセント {#percent}

**名前の例：** 購入しそうな場合 — 割合の値を格納します（おそらくCRM側で計算されます）。

**値の例：** 85%

**演算子**:が次の値を超える、次の値を超えない、次の値を超える、次よりも小さい、最低でも多い、最大でも空でない、

## 電話 {#phone}

**名前の例：** 別の電話 — ユーザーの追加の電話番号を保存します。

**値の例：** 650-555-5555

**演算子**:がis、is、not、がある開始、not開始と、contains、not contains、is empty、not empty

## スコア {#score}

**名前の例：** 行動スコア/人口統計スコア — 複数のスコアフィールドを作成して、異なる属性を追跡します。

**値の例：** 14

**演算子**:が次の値を超える、次の値を超えない、次の値を超える、次よりも小さい、最低でも多い、最大でも空でない、

## 文字列 {#string}

**名前の例：** ミドルネーム — 追加のテキスト属性を保存します。

**値の例：** ローズ

**演算子**:がis、is、not、がある開始、not開始と、contains、not contains、is empty、not empty

## テキスト領域 {#text-area}

**名前の例：** コメント — 複数行にわたるテキスト入力を許可するために、フォームにコメントフィールドを追加します。

**値の例：** この記事は素晴らしい！

**演算子**:がis、is、not、がある開始、not開始と、contains、not contains、is empty、not empty

## URL {#url}

**名前の例：** ブログ — 個人のブログのURLを格納するフィールドを作成します。

**値の例：** www.myblog.com

**演算子**:がis、is、not、がある開始、not開始と、contains、not contains、is empty、not empty
