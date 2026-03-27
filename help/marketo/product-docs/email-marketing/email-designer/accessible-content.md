---
title: アクセシブルなコンテンツのデザイン
description: Marketo Engageでアクセシブルなメールコンテンツをデザインする方法を説明します。 メールがすべての受信者に対して機能するように、ベストプラクティスを適用する。
feature: Email Designer
role: User
level: Beginner, Intermediate
keywords: メール, デザイン, アクセシビリティ
exl-id: 6768d304-54c5-4eea-b3a7-b3a4eb3b4955
source-git-commit: f6893edbfe85d1d6e0958b5a3029d8fd404b1311
workflow-type: tm+mt
source-wordcount: '1374'
ht-degree: 45%

---

# アクセシブルなコンテンツのデザイン {#accessible-content}

[欧州アクセシビリティ法](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32019L0882){target="_blank"}は、加盟国によって異なる国の規則によって引き起こされる障壁を排除することにより、アクセシビリティの高い製品やサービスの国内市場を強化することを目的とした指令です。

この規制では、電子メール、ニュースレター、PDF、ダウンロード可能なコンテンツなど、あらゆるデジタルコミュニケーションにアクセスできるようにすることが求められています。 したがって、受信者のコンテンツを作成する場合は、アクセシブルなフォントや読みやすい形式の使用、画像の代替テキストの提供など、特定のガイドラインに従う必要があります。

Marketo Engage Email Designerを使用すると、Web Content Accessibility Guidelines （WCAG） 2.1 （レベル AA）に基づいて、このディレクティブに簡単に準拠できます。 Marketo Engageを使用して、アクセシブルなコンテンツをデザインするためのベストプラクティスを以下に示します。

>[!NOTE]
>
>このページでは、すべての受信者がコンテンツにアクセスできるように、Marketo Engageでデザインされたメールを読んだり、理解したり、やり取りしたりできるようにします。

## テキストの読みやすさの確保 {#text-readability}

**[!UICONTROL テキスト]** コンポーネントの「**[!UICONTROL スタイル]**」タブを活用して、適切なカラーコントラストやシンプルなフォントを使用するなど、テキストが読みやすいようにします。

<!--![](assets/accessible-text-styles.png){width="80%"}-->

フォントとテキストについては、次のガイドラインに従ってください。

**フォントの選択**

* Arial、Verdana、Tahoma、Helvetica、Open Sansなどのサンセリフフォントを使用します。
* 本文のコンテンツでは、セリフ体、筆記体、装飾的なフォントは使用しないでください。
* 一貫性とフォールバック用に制限されたフォントセットに固執します（例：`font-family: Arial, Helvetica, sans-serif;`）。

**フォントサイズ**

* 本文のフォントサイズは 16 px 以上を確保します。
* 見出しには適切な階層を使用します。

**カラーコントラスト**

* テキストと背景の間のコントラスト比を 4.5:1 以上に維持します。
* 大きなテキスト（≥24pxまたは太字18px）の場合は、少なくとも3:1のコントラストを確保します。
* 白い背景では、ライトグレーまたはパステルのテキストは回避します。
* 意味を伝えるために色だけに頼らないでください。 下線やアイコンなどを使用する

**テキストのアクセシビリティ**

* 画像内のテキストは回避します。
* 本文では大文字を使用しないでください。
* レイアウトを崩すことなく、テキストを最大200%まで拡大できることを確認します。

## 視覚的なアクセシビリティの確保 {#visual-accessibility}

* 重要な情報に対しては色のみのインジケーターの使用は回避します。
* 明確にするためにテキストラベルやアイコンを使用してください。
* ボタンが大きく、適切な間隔が空いていることを確保して、モバイルおよびレスポンシブレイアウト向けにデザインを最適化します。
* デバイスや画面サイズをまたいで定期的にテストすることで、アクセシビリティを維持します。

Marketo Engageでは、電子メールのDesigner **[!UICONTROL スタイル]** ペインのスタイルパラメーターと属性を使用して、コンテンツ内の様々な要素のサイズと間隔をさらに調整できます。

例えば、背景を更新したり、余白、パディング、整列を変更したりして、視覚的なアクセシビリティを向上させることができます。

<!--![](assets/accessible-styles.png){width="80%"}-->

Marketo Engageの電子メールDesignerを使用すると、様々なデバイスや画面サイズに合わせてプレビューを表示し、デザインを最適化できます。 いつでも&#x200B;**[!UICONTROL ライブビュー]**&#x200B;に切り替えて、様々なデバイスサイズでコンテンツがどのようにレンダリングされるかを確認できます。

<!--![](assets/accessible-live-view.png){width="80%"}-->

>[!CAUTION]
>
>ライブビューは、様々なデバイスサイズでコンテンツがどのようにレンダリングされるかを比較するために設計された汎用的なプレビューです。 最終的なレンダリングは、受信者のメールクライアントによって異なる場合があります。

## 画像用の代替テキストの使用 {#alt-text}

**[!UICONTROL 画像]** コンポーネントを使用して、画像に代替テキストを指定します。

<!--![](assets/accessible-alt-text.png){width="90%"}-->

* 画像の目的を簡潔に文脈に沿って説明します。
* 「…の画像」のような冗長なフレーズを回避し、装飾的な画像には空の代替テキストを使用します。
* 意味のあるアイコンには分かりやすいラベルを付け、複雑な画像には簡潔な代替テキストと、別の場所でより長い説明を使用します。

## 読み取り可能な形式の使用 {#readable-format}

電子メール Designerに関連する構造とコンテンツコンポーネント、および&#x200B;**[!UICONTROL スタイル]** ペインのオプションを使用して、すべてのユーザーがアクセスできる明確かつ論理的で簡潔な方法でコンテンツを整理します。

<!--![](assets/accessible-components.png){width="100%"}-->

* 適切な見出し、段落、リスト、テーブルを含む、構造化されたセマンティック HTML を使用します。
* コンテンツが左から右、上から下の論理的なフローに従っていることを確認します。
* 明確で簡潔な言語を使用します。
* PDF とインフォグラフィックには代替形式を用意します。
* テキストのサイズ変更とリフローを許可し、すべての形式で適切なカラーコントラストを使用してタイポグラフィを読み取れるようにします。

## コンテンツの読みやすさの確保 {#readability}

コンテンツを読みやすくするためには、視覚的、認知的、読書的な課題を抱える人や、支援技術を利用している人など、誰もが明確で、適切に構造化され、使用できる必要があります。 アクセス可能なコンテンツを作成する際に考慮すべき点を以下に示します。

* 文章は20語以内に収めましょう。
* コピーは直接的かつ簡潔に編集します。
* アクティブなボイスを使用して、文構造をシンプルに保ちます。
* よく知らない人がいるかもしれませんが、スラングや専門用語、地域の単語は避けましょう。

メールの読みやすさを評価するには、Microsoft Word に含まれている一番人気の [Flesch Reading Ease テスト](https://support.microsoft.com/ja-jp/office/get-your-document-s-readability-and-level-statistics-85b4969e-e80a-4777-8dd3-f7fc3c8b3fd2){target="_blank"}を使用します。このテストでは、コンテンツの読みやすさを 0～100 のスケールで計算します。

## コンテンツのテスト {#test}

コンテンツのアクセシビリティを検証するには、Marketo Engageのテスト機能を使用できます。 これらは、コンテンツが完全にアクセス可能かどうかを確認するのに特別に設計されたものではありませんが、第 1 レベルの検証を提供できます。

* テストプロファイルを使用してコンテンツをプレビューします。

* Litmus を活用した「[メールレンダリング](/help/marketo/product-docs/email-marketing/email-designer/test-email-rendering.md){target="_blank"}」オプションを使用して、主要なメールクライアント（Apple メール、Gmail、Outlook）でデザインをシミュレートし、テキスト、色、画像によってコンテンツがアクセス可能になるかどうかを確認します。<!--Litmus includes accessibility testing-->

* プルーフを送信して、実際のオーディエンスにコンテンツを送信する前に、コンテンツのレンダリングをテストします。

<!--![](assets/accessible-simulate.png){width="90%"}-->

コンテンツに確実にアクセスできるかどうかをより一貫した方法で確認するには、次のような特定の外部ツールを使用します。

* コントラストとコンプライアンスを評価する [WebAim コントラストチェッカー](https://webaim.org/resources/contrastchecker/){target="_blank"}および [WAVE web アクセシビリティ評価ツール](https://wave.webaim.org/){target="_blank"}。

* スクリーンリーダー（例：[NVDA](https://www.nvaccess.org/download/){target="_blank"}、iPhoneの[VoiceOver](https://support.apple.com/ja-jp/guide/iphone/iph3e2e415f/ios){target="_blank"}など）などの支援テクノロジーを利用して、視覚障害のあるユーザーの視点からメールを体験できます。

## ダークモードの使用 {#dark-mode}

[ ダークモード ](/help/marketo/product-docs/email-marketing/email-designer/dark-mode.md){target="_blank"}は、光感度または視覚障害を持つユーザーの視覚的アクセシビリティを向上させ、視聴体験を向上させます。

<!--![](assets/accessible-dark-mode.png){width="90%"}-->

ダークモードでコンテンツをデザインするためのベストプラクティスには、次のようなものがあります。

* 透明なPNGまたはSVGの使用
* 適切なメタタグとCSSの設定
* ダークモードがサポートされていない場合は、アクセス可能なフォールバックスタイルを提供します。

あらゆるメールコンテンツやUI要素をライトモードとダークモードの両方でテストすることで、メールがダークモードで正しくレンダリングされるようにします。

## アクセシビリティに対する特定の属性の使用 {#attributes}

### 言語属性 {#language}

デザインを作成する際は、コンテンツ本体に `lang`（言語）属性と `dir`（テキスト方向）属性を含めます。これらの属性は、アシスタントテクノロジー（スクリーンリーダーなど）がコンテンツを適切な方法で解釈し、表示するのに役立ちます。

* `lang` 属性は、支援テクノロジーに対するメールの言語を示し、単語が正しく発音されるようにします。

  +++例

  英語の例：

  ```
  <body lang="en">
  ```

  フランス語の例：

  ```
  <body lang="fr">
  ```

  +++

* `dir` 属性は、テキストの方向を指定します。英語やフランス語を含むほとんどの言語は左から右（ltr）に読みますが、アラビア語やヘブライ語などの言語は右から左（rtl）に読みます。

  +++例

  英語の例（左から右）：

  ```html
  <body lang="en" dir="ltr">
  ```

  アラビア語の例（右から左）：

  ```html
  <body lang="ar" dir="rtl">
  ```

  +++

スクリーンリーダーは、正しい発音ルールを適用するために `lang` 属性に依存し、テキストの方向によって、左から右または右から左の言語でコンテンツが自然に流れるようになります。これらの属性がないと、ユーザーは読み取り順序に混乱したり、発音が間違ったりする場合があります。電子メール本文は、必ず適切な`lang`属性と`dir`属性で囲んでください。

>[!TIP]
>
>メールに複数の言語が含まれている場合は、各部分が正しく読まれるように、特定のセクション（`<table>` ブロックや`<td>` ブロックなど）に適切な言語属性を割り当てます。

### テーブル {#tables}

HTML コンテンツでは、表はレイアウトに頻繁に使用されます。 デフォルトでは、スクリーンリーダーはすべての `<table>` をデータテーブルとして処理し、行、列、構造を読み上げます。テーブルが書式設定のみに使用されている場合、混乱を招くことがあります。

レイアウトテーブルに `role="presentation"`（または `role="none"`）を追加して、支援テクノロジーが構造をスキップし、実際のコンテンツにのみ焦点を当てられるようにします。

+++例 – レイアウトテーブル （`role="presentation"`）

```html
<table role="presentation" border="0" cellpadding="0" cellspacing="0" width="100%"> 
  <tr> 
    <td align="center"> 
      <h1>Hello World</h1> 
      <p>Welcome to our newsletter</p> 
    </td> 
  </tr> 
</table>
```

スクリーンリーダーは次のように内容を読み上げます。
「Hello World。ニュースレターへようこそ。」_（行、列、テーブルに関する読み上げはされません）_

+++

+++例 – データテーブル （`role="presentation"`を除く）

```html
<table border="1" cellpadding="5" cellspacing="0">
  <tr>
    <th scope="col">Name</th>
    <th scope="col">Score</th>
  </tr>
  <tr> 
    <td>Peter</td>
    <td>19</td>
  </tr>
  <tr>
    <td>Parker</td>
    <td>62</td>
  </tr>
</table>
```

スクリーンリーダーは次ように内容を読み上げます。
「2 列 3 行のテーブルです。」

「名前、ピーター。 スコア、19。」

「名前、パーカー。 スコア、62。」

+++

>[!TIP]
>
>`role="presentation"` は、レイアウトテーブルにのみ使用します。データテーブルの場合、スクリーンリーダーがヘッダーと関係を正しく読み上げることができるように、セマンティック `<table>` 構造を保持します。

### リンクのテキスト {#links}

スクリーンリーダーは、リンクのテキストを使用してリンクを読み上げます。リンクに「こちらをクリック」または「詳細情報」のみのラベルが付いている場合、支援テクノロジーのユーザーは宛先を知りません。アクセシビリティを確保するには、ターゲットやアクションを明確に示す説明テキストが必要です。

電子メールDesignerを使用して、コンテンツにリンクを追加し、ラベルを編集して、識別しやすく（表示しやすく）、説明的に（目的を明確に）表示します。 「こちら」や「詳細」など、あいまいなラベルは回避します。

<!--![](assets/accessible-link.png){width="70%"}-->

+++例 – 適切なリンク（説明的）: 

```
<p>Learn more in the  
<a href="https://adobe.com/release-notes">August release notes</a>. 
</p>
```

スクリーンリーダーは次のように内容を読み上げます。
「リンク、8月リリースノート」

+++

+++例 – 不正なリンク（記述的ではない）

```
<p>Learn more about our new features.  
  <a href="https://adobe.com/release-notes">Click here</a>. 
</p>
```

スクリーンリーダーは次のように内容を読み上げます。
「リンク、こちらをクリック。」*（読み取り順序からコンテキストが提供されない）*

+++

<!--for Landing Pages-->

<!--
## Provide keyboard navigation and focus support {#keyboard}

Providing keyboard navigation and focus support allows people who cannot use a mouse to fully access and interact with content. It also improves overall usability by giving all users a clear and consistent way to move through information.

* Focus via keyboard
    * Ensure all interactive elements (such as buttons, checkboxes, links) have `tabindex="0"` so they are included in the natural tab order. 
    * Allow navigation using the Tab and arrow keys (↑ ↓ ← →), which should visibly highlight the focused element. 
* Custom focus styling 
    * Apply clear and distinguishable styles for focusing on actionable elements: 
        +++Example (CSS)

        ```
        [tabindex="0"] : focus { 
        outline: 2px solid #00AEEF;  /* Cyan border */ 
        background-color: #20CEFF;   /* Optional background */ 
        }
        ```
        
        +++

    * Ensure that focus indicators meet the WCAG 2.2 focus appearance standards, including: 
        * Minimum area: 2 CSS pixel thick outline.
        * Contrast ratio: ≥ 3:1 between focused and unfocused state. 

* Keyboard activation support 
    * Ensure checkboxes and buttons respond to the Enter and Space keys. 
    * Validate the interaction using the keyboard alone: 
        * Enter or Space should toggle checkboxes.
        * Enter or Space should trigger the buttons.
-->
