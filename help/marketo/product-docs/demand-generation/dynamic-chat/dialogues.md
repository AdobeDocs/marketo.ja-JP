---
description: ダイアログ — Marketoドキュメント — 製品ドキュメント
title: ダイアログ
hide: true
hidefromtoc: true
source-git-commit: c46902686f1d5af63a51f5eaae2dc0e6afe99629
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# ダイアログ {#dialogues}

ダイアログは、設定した特定のチャット会話です。 見た目や見た目をカスタマイズできます。

## 新しいダイアログの作成 {#create-a-new-dialogue}

1. **ダイアログ**&#x200B;をクリックします。

PICC

1. 「**新規作成**」ボタンをクリックします。

PICC

1. 名前を入力し（説明はオプション）、優先度レベルを設定し、「**保存**」をクリックします。

PICC

>[!NOTE]
>
>優先度レベルの説明

## オーディエンス条件 {#audience-criteria}

Marketoのスマートリストと同様に、オーディエンス条件属性を使用してターゲットオーディエンスを定義できます。

選択できる属性は複数あります。 この例では、「リードの状態」を&#x200B;_「Is_ California」に選択し、「会社の規模」を&#x200B;_「_」より大きくします。

1. リードの状態(Lead State)アトリビュートを取得し、右にドラッグします。

PICC

1. __ Isはデフォルトで設定されます。「値の選択」フィールドに「 CA 」と入力します（ドロップダウンをクリックして、リストから「 」を選択することもできます）。

PICC

1. 会社サイズ属性を取得し、右にドラッグします。

PICC

1. 演算子のドロップダウンをクリックし、「次よりも大きい」を選択します。

PICC

1. 「 50 」と入力し、画面の別の場所をクリックして保存します。

PICC

## グループの追加 {#add-groups}

すべての特定の属性を別の属性の「いずれか」と共に持つ場合に備えて、属性のグループ化も選択できます。

終了

## ターゲット {#target}

ここで、特定のダイアログを表示する特定のURLを入力します。

指定できる形式：

* `http://website.com`
* `https://*.website.com`
* `http://website.com/folder/*`
* `https://*.website.com/folder/*`

>[!NOTE]
>
>アスタリスクを使用すると、包括的なワイルドカードとして機能します。 したがって、`https://*.website.com`は、サブドメインを含むサイトのすべてのページにダイアログを配置します(例：support.website.com)を参照してください。 `https://website.com/folder/*`は、後続のフォルダー内のすべてのHTMLページにダイアログを配置します(例：この場合、フォルダーが「sports」であるとします。そのため、次のようになります。website.com/sports/baseball.html、website.com/sports/football.htmlなど)。
