---
solution: Marketo Engage
product: marketo
title: メールコンテンツへのカスタム CSS の追加
description: Marketo EngageのメールDesigner内でメールコンテンツに直接カスタム CSS を追加する方法を説明します。
level: Intermediate
feature: Email Designer
exl-id: c191b44a-47ab-41f8-aa95-9268e359e5db
source-git-commit: de3999dd6ede77c8fc591e24a69f062954b8c870
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 29%

---

# メールコンテンツへのカスタム CSS の追加 {#custom-css}

独自のカスタム CSS をMarketo Engage メールDesigner内に直接追加して、高度な特定のスタイル設定を行います。

## カスタム CSS の定義 {#define-custom-css}

1. 少なくとも 1 つのコンポーネントを追加して、メールDesignerでコンテンツの一部が定義されていることを確認します。

1. 左側の **[!UICONTROL ナビゲーションツリー]** または右側のパネルから **[!UICONTROL 本文]** を選択します。 **[!UICONTROL CSS スタイル]** が右側に表示されます。

   ![](assets/custom-css-1.png){width="800" zoomable="yes"}

   >[!NOTE]
   >
   >「**[!UICONTROL CSS スタイル]**」セクションは、エディターにコンテンツが存在する場合にのみ使用できます。

1. 「**[!UICONTROL + カスタム CSS を追加]**」ボタンをクリックします。

   >[!NOTE]
   >
   >「**[!UICONTROL カスタム CSS を追加]**」ボタンは、「**[!UICONTROL 本文]**」が選択されている場合にのみ使用できます。 ただし、コンテンツ内のすべてのコンポーネントにカスタム CSS スタイルを適用できます。

1. ポップアップ表示される専用のテキスト領域に CSS コードを入力します。カスタム CSS [ が有効で、適切な構文に従っていることを確認します ](#use-valid-css)。 終了したら「**保存**」をクリックします。

   ![](assets/custom-css-2.png)

   >[!NOTE]
   >
   >[ コンテンツがロックされたテンプレート ](/help/marketo/product-docs/email-marketing/email-designer/content-locking.md) を使用する場合、カスタム CSS をコンテンツに追加することはできません。 ボタンのラベルが **[!UICONTROL カスタム CSS を表示]** に変わり、表示されるカスタム CSS は読み取り専用になります。

1. CSS がコンテンツに適用されていることを確認します。 表示されない場合は、[ トラブルシューティング ](#troubleshooting) の節を確認してください。

   ![](assets/custom-css-3.png)

   >[!NOTE]
   >
   >すべてのコンテンツを削除すると、セクションが非表示になり、以前に定義したカスタム CSS は適用されなくなります。 コンテンツを追加して **[!UICONTROL CSS スタイル]** セクションを再表示します。 カスタム CSS が再度適用されます。

## 有効な CSS の使用 {#using-valid-css}

「**[!UICONTROL カスタム CSS を追加]**」テキスト領域に有効な CSS 文字列を入力できます。適切に書式設定した CSS はコンテンツにすぐに適用されます。

>[!CAUTION]
>
>カスタム CSS のセキュリティはユーザーが担当します。 CSS によって脆弱性が発生したり、既存のコンテンツと競合したりしていないことを確認します。
>
>意図せずコンテンツのレイアウトや機能が壊れる可能性がある CSS の使用は避けます。

+++ 有効な CSS のサンプル

有効な CSS の例を以下に示します。

```css
.acr-component[data-component-id="form"] {
  display: flex;
  justify-content: center;
  background: none;
}

.acr-Form {
  width: 100%;
  padding: 20px 100px;
  border-spacing: 0px 8px;
  box-sizing: border-box;
  margin: 0;
}

.acr-Form .spectrum-FieldLabel {
  width: 20%;
}

.acr-Form.spectrum-Form--labelsAbove .spectrum-FieldLabel,
.acr-Form [data-form-item="checkbox"] .spectrum-FieldLabel {
  width: auto;
}

.acr-Form .spectrum-Textfield {
  width: 100%;
}

#acr-form-error,
#acr-form-confirmation {
  width: 100%;
  padding: var(--spectrum-global-dimension-static-size-500);
  display: flex;
  align-items: center;
  flex-direction: column;
  justify-content: center;
  gap: var(--spectrum-global-dimension-static-size-200);
}

.spectrum-Form-item.is-required .spectrum-FieldLabel:after{
  content: '*';
  font-size: 1.25rem;
  margin-left: 5px;
  position: absolute;
}

/* Error field placeholder */
.spectrum-HelpText {
  display: none !important;
}

.spectrum-HelpText.is-invalid,
.is-invalid ~ .spectrum-HelpText {
  display: flex !important;
}
```

```css
@media only screen and (min-width: 600px) {
  .acr-paragraph-1 {
    width: 100% !important;
  }
}
```

+++


+++ 無効な CSS のサンプル

無効な CSS を入力すると、CSS を保存できないことを示すエラーメッセージが表示されます。 無効な CSS の例を以下に示します。

`<style>` タグの使用は許可されていません。

```html
<style type="text/css">
  .acr-Form {
    width: 100%;
    padding: 20px 100px;
    border-spacing: 0px 8px;
    box-sizing: border-box;
    margin: 0;
  }
</style>
```

中括弧の欠落などの無効な構文は許可されていません。

```css
body {
  background: red;
```

+++

## 技術的な実装 {#implementation}

次の例に示すように、カスタム CSS は、`data-name="global-custom"` 属性を持つ `<style>` タグの一部として `<head>` セクションの末尾に追加されます。これにより、カスタムスタイルがコンテンツにグローバルに適用されます。

+++ サンプルを参照

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="content-version" content="3.3.31">
    <meta name="x-apple-disable-message-reformatting">
    <meta name="viewport" content="width=device-width,initial-scale=1.0">
    <style data-name="default" type="text/css">
      td { padding: 0; }
      th { font-weight: normal; }
    </style>
    <style data-name="grid" type="text/css">
      .acr-grid-table { width: 100%; }
    </style>
    <style data-name="acr-theme" type="text/css" data-theme="default" data-variant="0">
      body { margin: 0; font-family: Arial; }
    </style>
    <style data-name="media-default-max-width-500px" type="text/css">
      @media screen and (max-width: 500px) {
        body { width: 100% !important; }
      }
    </style>
    <style data-name="global-custom" type="text/css">
      /* Add you custom CSS here */
    </style>
  </head>
  <body>
    <!-- Minimal content -->
  </body>
</html>
```

+++


カスタム CSS は、E メールデザイナーの&#x200B;**[!UICONTROL 設定]**&#x200B;パネルでは解釈または検証されません。これは完全に独立しており、「**[!UICONTROL カスタム CSS を追加]**」オプションを通じてのみ変更できます。

### ガードレール – 読み込まれたコンテンツ {#guardrails}

E メールデザイナーに読み込んだコンテンツでカスタム CSS を使用する場合は、次の点を考慮します。

* CSS を含むコンテンツを [ 外部HTMLの読み込み ](/help/marketo/product-docs/email-marketing/email-designer/email-authoring.md#import-html) する場合、そのコンテンツを変換しない限り、コンテンツは **[!UICONTROL 互換モード]** になり、「**[!UICONTROL CSS スタイル]**」セクションは使用できません。

* メールのDesignerで作成されたコンテンツに、「**[!UICONTROL カスタム CSS を追加]**」オプションを通じて適用された CSS が含まれている場合、以前に適用された CSS は、同じオプションから表示および編集できます。

## トラブルシューティング {#troubleshooting}

カスタム CSS が適用されていない場合は、以下の提案を試してください。

* CSS が有効で、構文エラー（中括弧の欠落、プロパティ名の誤りなど）がないことを確認します。 [方法についてはこちらを参照](#use-valid-css)

* CSS が、`<style>` 属性を持つ `data-name="global-custom"` タグに追加されていることを確認します。

* `global-custom` スタイルタグの属性 `data-disabled` が `true` に設定されているかどうかを確認します。 その場合、カスタム CSS は適用されません。

+++ 例：

  ```html
  <style data-name="global-custom" type="text/css" data-disabled="true"> body: { color: red; } </style>
  ```

+++

* CSS が他の CSS ルールによって上書きされていないことを確認します。

   * ブラウザーの開発者ツールを使用して、コンテンツを調べ、CSS が正しいセレクターをターゲットにしていることを確認します。

   * 必ず優先されるように、宣言に `!important` を追加することを検討してください。

+++ 例：

     ```css
     .acr-Form {
       background: red !important;
     }
     ```

+++

>[!NOTE]
>
>Marketo Engage サポートは、カスタム CSS のトラブルシューティングを支援するように設定されていません。 CSS のサポートについては、web 開発者にお問い合わせください。
