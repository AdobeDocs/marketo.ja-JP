---
solution: Marketo Engage
product: marketo
title: カスタマイズ可能なフラグメント
description: フィールドを編集可能にして、フラグメントをカスタマイズする方法を説明します。 電子メールDesignerで、柔軟な再利用可能なフラグメントを作成します。
level: Beginner, Intermediate
feature: Email Designer
role: User
exl-id: 3e0232c7-13bd-49e2-b7c7-cd389b5f0704
TQID: https://experienceleague.adobe.com/SCmyn9QUECmvQgVltKknlvLuvL15Tz3LYorBFYB1hqI
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2: id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: fdc003d7aed05d85687427d9455bb806eb33d0b2
workflow-type: tm+mt
source-wordcount: 1403
ht-degree: 12%

---

# カスタマイズ可能なフラグメント {#customizable-fragments}

フラグメントがメールまたはメールテンプレートで使用される場合、フラグメントは継承のためにデフォルトでロックされます。つまり、フラグメントに対して行われた変更は、使用されるすべてのアセットに自動的に反映されます。 カスタマイズ可能なフラグメントを使用すると、フラグメント内の特定のフィールドを、フラグメントが電子メールまたは電子メールテンプレートに追加されたときに編集可能として定義できます。 例えば、バナー、テキスト、ボタンを含むフラグメントがある場合、画像やボタンのターゲット URLなどの特定のフィールドを編集可能として指定できます。

カスタマイズ可能なフラグメントを使用すれば、まったく新しいコンテンツブロックを作成したり、フラグメントの継承を中断したりすることなく、コンテンツを管理およびパーソナライズできます。 フラグメントレベルで行われた変更は引き続き反映されますが、電子メールまたは電子メールテンプレートレベルでカスタマイズできます。

ビジュアルフラグメントと式フラグメントの両方をカスタマイズ可能としてマークできます。

## ビジュアルフラグメントへの編集可能なフィールドの追加 {#visual}

ビジュアルフラグメントの一部を編集可能にするには、次の手順に従います。

>[!NOTE]
>
>編集可能なフィールドは、**画像**、**テキスト**、**ボタン**&#x200B;コンポーネントに追加できます。 **HTML** コンポーネントの場合、式フラグメントと同様に、パーソナライゼーションエディターを使用すると、編集可能なフィールドが追加されます。 [ フラグメント内のHTML コンポーネントの編集可能フィールドについて説明します](#editable-html)

1. フラグメントコンテンツ編集画面を開きます。

1. 編集可能なフィールドを設定するフラグメント内のコンポーネントを選択します。

1. コンポーネントのプロパティパネルが右側に開きます。 「**[!UICONTROL 編集可能なフィールド]**」タブを選択し、「**[!UICONTROL 編集を有効にする]**」オプションを切り替えます。

1. 選択したコンポーネントの編集可能なすべてのフィールドがパネルにリストされます。 編集可能なフィールドは、選択したコンポーネントタイプによって異なります。

   以下の例では、「ここをクリック」ボタンのURLが編集可能に設定されています。

   ![](assets/fragment-param-enable.png){width="800" zoomable="yes"}

1. **[!UICONTROL 概要]**&#x200B;をクリックして、編集可能なすべてのフィールドとそのデフォルト値を確認します。

   この例では、ボタンの URL フィールドに、コンポーネントで定義したデフォルト値が表示されます。 ユーザーは、フラグメントをコンテンツに追加した後、この値をカスタマイズできます。

   ![](assets/fragment-param-preview.png){width="800" zoomable="yes"}

1. 完了したら、変更を保存します。

フラグメントをメールに追加すると、ユーザーはフラグメントで設定されたすべての編集可能フィールドをカスタマイズできます。

## フラグメント内の編集可能なHTML コンポーネント {#editable-html}

HTML コンポーネント内では、次の種類のエレメントを編集可能にすることができます。

* **テキストコンテンツ**&#x200B;の一部（見出しやCTA ラベルなど）。
* 完全な&#x200B;**URL**。リンクターゲットまたは画像ソースとして使用されます。 一部のURLはサポートされていません。変数はURL値全体を表す必要があります。
* 完全な&#x200B;**CSS プロパティ値** （フルカラー値、フルパディング値、フルワイド値など）。 部分的なCSS プロパティ値はサポートされていません。

パラメーター化された各CSS プロパティ値は、サフィックスなし、追加テキストなし、複数の変数なし、単一のプロパティ内の連結なし、正確に`{{{varName}}}`である必要があります。

パディングなどのマルチサイドプロパティをパラメーター化するには、次のいずれかの操作を行います。

* 各辺を個別のプロパティ _（推奨）_&#x200B;として宣言するか、
* 完全な短縮値を含む単一の変数を宣言します。

## HTML コンポーネントでの編集可能フィールドの仕組み {#components}

HTML コンポーネントの編集可能なフィールドは、コンポーネントのソースコード内でインライン変数を直接宣言することによって作成されます。 各変数には一意のIDとデフォルト値があります。 次に、編集可能な値がマークアップに表示される場所で変数が参照されます。

フラグメントを保存して公開すると、HTML コンポーネントで宣言されたすべての変数が、フラグメントがメールに追加されたときに編集可能なパラメーターとして自動的に表示されます。

その後、メール作成者は、メールDesignerの任意の変数のデフォルト値を上書きできます（例えば、背景色の変更、CTA URLの入れ替え、見出しの更新など）。元となるHTMLを変更する必要はありません。

## 構文参照 {#syntax}

編集可能なフィールドは、次の2つのパターンを使用して定義および参照されます。

### 変数の宣言 {#declaring}

インライン宣言を使用して、一意のIDとデフォルト値を持つ変数を定義します。

```handlebars
{{#inline "variableID"}}default_value{{/inline}}
```

`variableID`を編集可能なフィールドの一意のIDに置き換えます。 IDは、コンポーネント内で一意である必要があり、スペースを含めることはできません。

`default_value`を、メール作成者が上書きしない場合に使用する値に置き換えます。

### 変数の参照 {#referencing}

3つの中括弧を使用して、変数の値がマークアップに表示される場所を参照します。

```handlebars
{{{variableID}}}
```

同じ変数IDは、HTML内で何度でも参照できます。 すべての参照は、メール作成者が設定した値（上書きが指定されていない場合はデフォルト値）に解決されます。

### オプションのパラメーター {#optional}

インライン宣言では、編集可能なフィールドの表示方法や処理方法を変更するオプションのパラメーターをサポートしています。

| アクション | パラメーター | 例 |
|---|---|---|
| 編集可能フィールドを&#x200B;**デフォルト値**&#x200B;と共に宣言します。 フラグメントがメールに追加される場合、作成者がフラグメントを上書きしない限り、このデフォルト値が使用されます。 | インラインタグの間にデフォルト値を追加します。 | `{{#inline "editableFieldID"}}default_value{{/inline}}` |
| 編集可能フィールドの&#x200B;**ラベル**&#x200B;を定義します。 このラベルは、メール作成者がフラグメントのフィールドを編集したときに、メールDesignerに表示されます。 | `name="title"` | `{{#inline "editableFieldID" name="title"}}default_value{{/inline}}` |
| **画像ソース**&#x200B;を含む編集可能なフィールドを宣言します。 | `assetType="image"` | `{{#inline "editableFieldID" assetType="image"}}default_value{{/inline}}` |
| 追跡が必要な&#x200B;**URL**&#x200B;を含む編集可能なフィールドを宣言します。 | `assetType="url"` | `{{#inline "editableFieldID" assetType="url"}}default_value{{/inline}}` |

## HTML コンポーネントへの編集可能フィールドの追加 {#adding-editable-fields}

ビジュアルフラグメント内のHTML コンポーネントの一部を編集可能にするには、次の手順に従います。

1. 電子メールDesignerで、編集用のビジュアルフラグメントを開きます。
1. コンポーネントパネルから&#x200B;**HTML コンポーネント**&#x200B;をフラグメントに追加するか、既存のHTML コンポーネントを選択します。
1. HTML コンポーネントを選択した状態で、**ソースコードを表示**&#x200B;をクリックして、パーソナライゼーションエディターでHTML ソースビューを開きます。
1. パーソナライゼーションエディターで、インライン宣言構文を使用して編集可能な各変数を宣言します。 読みやすくするために、すべての変数宣言をコンポーネントの上部に配置し、各変数に一意のIDを割り当てます。
1. 編集可能な値が表示される場所で、`{{{variableID}}}`構文を使用してHTML マークアップの各変数を参照します。 同じコンポーネント内で同じ変数を複数回参照できます。
1. HTML コンポーネントを保存してから、フラグメントを保存します。
1. フラグメントを公開して、メールで使用できるようにします。

## メールでのフラグメントの使用 {#using-fragment}

フラグメントが公開されると、HTML コンポーネントで宣言されたすべての変数が、電子メールDesignerで編集可能なパラメーターとして表示されます。

メールでフラグメントを使用する際にカスタマイズするには、次の手順を実行します。

1. Marketo Engage電子メールDesignerで電子メールを開くか、作成します。
1. 公開したフラグメントをメールキャンバスに追加します。
1. フラグメントを選択してプロパティパネルを開きます。 編集可能なフィールドのリストは、**編集可能なフィールド** セクションの下に表示され、各フィールドには変数ID （または`name` パラメーターで指定されたわかりやすいラベル）でラベル付けされます。
1. プロパティパネルから編集可能なフィールドの値を直接更新します。 変更は現在の電子メールにのみ適用されます。公開されたフラグメントと、それを参照する他の電子メールは影響を受けません。
1. 電子メールを保存します。

フラグメントは、カスタマイズされた値でレンダリングされますが、公開されたフラグメントに対して行われた将来の構造更新は引き続き継承されます。

### 例：編集可能なテキスト、カラー、URLを含むシンプルなフラグメント {#example}

次の例では、4つの編集可能なフィールドを含む小さなプロモーションバナーを作成します。

* 背景色
* 見出しのテキスト
* CTAラベル
* CTAのURL

フラグメントを公開した後、メール作成者は、フラグメントをメールに追加する際に、これらの値のいずれかを上書きできます。

**シンプルな編集可能バナー**

```html
<!-- Define editable variables -->
{{#inline "bgColor"}}#0057FF{{/inline}}
{{#inline "headlineText"}}Example Headline{{/inline}}
{{#inline "ctaText"}}Learn More{{/inline}}
{{#inline "ctaUrl" assetType="url"}}https://www.example.com{{/inline}}

<!-- Use the variables in the HTML -->
<table width="100%" cellpadding="0" cellspacing="0"
       style="background-color:{{{bgColor}}}; border-radius:8px;" >
  <tr>
    <td style="padding:30px; text-align:center; font-family:Arial,sans-serif;">
      <h2 style="color:#ffffff; font-size:24px; margin:0;">
        {{{headlineText}}}
      </h2>
      <a href="{{{ctaUrl}}}"
         style="display:inline-block; margin-top:16px; padding:12px 28px;
                background:#ffffff; color:{{{bgColor}}};
                font-weight:bold; border-radius:4px; text-decoration:none;">
        {{{ctaText}}}
      </a>
    </td>
  </tr>
</table>
```

この例では、次のようになります。

* `bgColor`は2回参照されます。1回はテーブルの背景色、1回はCTAのテキストカラーです。 両方の参照は同じ値に解決されるので、1回の編集は両方の場所に反映されます。
* `ctaUrl`は`assetType="url"`で宣言され、値をトラッキング URLとして処理する必要があることを示します。

## ベストプラクティス {#best-practices}

* 変数のデフォルト値の中に単位（`px`、`em`、`%`）を含めることで、変数が完全なCSS値を表します。 これは、サポートされていない連結を回避します。
* 各辺を個別に編集する必要がある場合は、短縮形よりも辺ごとの長文CSS プロパティ （`padding-top`、`padding-right`、`padding-bottom`、`padding-left`）を優先します。
* URLを追跡する必要がある場合は、`assetType="url"`で宣言します。
* 編集可能なフィールドに画像ソースが含まれる場合は、`assetType="image"`を使用して宣言します。
* ドラフトメールにフラグメントを追加し、すべての編集可能フィールドがプロパティパネルに表示され、上書きされたときに正しく解決されることを確認して、フラグメントをテストします。

## 知っておくべきこと {#things-to-know}

* HTML コンポーネントの編集可能なフィールドでは、フルテキストコンテンツ、完全なURL、完全なCSS プロパティ値をサポートしています。 部分的なURLと部分的なCSS プロパティ値はパラメーター化できません。
* 単一のCSS プロパティ値では、変数を追加の静的テキストまたは別の変数と組み合わせることはできません。 パラメーター化された各プロパティ値は、1つの変数参照のみを使用する必要があります。
* 変数IDは、HTML コンポーネント内で一意である必要があり、スペースを含めることはできません。
* 購読解除リンクやミラーページ URLなどの、すぐに使用できるシステムリンクを、編集可能なフィールドに変換することはできません。

<!--
## Add editable fields in HTML components and expression fragments {#expression}

To make portions of an HTML component or an expression fragment editable, you must use a specific syntax in the expression editor. This involves declaring a _variable_ with a default value that users can override after adding the fragment to their content.

For example, suppose you want to create a fragment to add to your emails, and allow users to customize a specific color used in different locations, such as frames or buttons' background colors. When creating your fragment, you need to declare a variable with a _unique ID_ (e.g., "color"), and call it at the desired locations in the fragment content where you want to apply this color. When adding the fragment to their content, users will be able to customize the color used wherever the variable is referenced.

For HTML components, only specific elements can become editable fields. Expand the section below for more information.

+++Editable elements in HTML components:

The elements below can become editable fields in an HTML component:

* A portion of text
* A full URL for link or image (doesn't work with portion of a URL)
* Entire CSS property (doesn't work with partial property)

For example, in the code below, each element highlighted in red can become a property:

![](assets/fragment-html.png){width="500" zoomable="yes"}

+++
-->

>[!MORELIKETHIS]
>
>[フラグメント](/help/marketo/product-docs/email-marketing/email-designer/fragments.md){target="_blank"}
