---
unique-page-id: 11371040
description: メールテンプレートの構文 - Marketo ドキュメント - 製品ドキュメント
title: メールテンプレートの構文
exl-id: 84d6c0a8-1108-4b7e-8b4f-ac0682c6bdbb
source-git-commit: a59b6b2505c6e5a83c6137a1925aa4e60e56eac8
workflow-type: ht
source-wordcount: '2423'
ht-degree: 100%

---

# メールテンプレートの構文 {#email-template-syntax}

Marketo の新しい Email 2.0 エクスペリエンスでは、メールテンプレートは、要素、変数、モジュールまたはコンテナの任意の組み合わせで構成されます。それぞれは、HTML に Marketo 固有の構文を追加することで定義されます。古い（v1.0）メールテンプレートは、Email Editor 2.0 でサポートされていますが、新しいエディターの機能の一部は含まれません。

Marketo メール構文は、テンプレートと個々のメールでのみ機能しますが、スニペットまたはリッチテキストトークンに埋め込まれた場合には機能&#x200B;**しません**。

>[!NOTE]
>
>Marketo サポートは、CSS／HTML については対応できません。CSS や HTML に詳しくない場合は、デベロッパーにお問い合わせください。

>[!CAUTION]
>
>Marketo 構文（mktoModule、mktoContainer、mktoText）を含むクラス値では、大文字と小文字が区別されます。カスタム属性名（mktoimgwidth、mktoname）は使用できません。

## 要素 {#elements}

要素は、メールテンプレート内で編集可能として定義するコンテンツ領域です。要素の編集操作は、要素のタイプに応じて異なり、コンテンツを簡単に操作できます。メールテンプレートに含めることができる要素は次のとおりです。

* リッチテキスト
* 画像
* スニペット
* 動画

## リッチテキスト {#rich-text}

地域をリッチテキストとして定義すると、[Marketo のリッチテキストエディターを使用](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md)してそのコンテンツを編集できます。メールテンプレート内でリッチテキスト要素を定義する方法には、mktEditable と mktoText の 2 つがあります。リッチテキスト要素は、メールエディター内から常にスニペットに変換できます。

### オプション 1 - mktEditable {#option-mkteditable}

Email Editor 2.0 は後方互換性があるので、一部の古いメールテンプレートは、任意の HTML 要素に「class=&quot;mktEditable&quot;」を追加することで、リッチテキスト要素を指定できます。これは引き続きサポートされ、要素の ID は、メールエディター内の表示名として使用されます。

必須の属性

* **class**：&quot;mktEditable&quot;
* **id**：ID 文字列。文字、数字、ダッシュ（-）、アンダースコア（_）のみが含まれます。スペースは使用できません。一意である必要があります。

オプションの属性

* **mktoName**：文字列。これは、Email Editor 2.0 で表示される表示名です。ベストプラクティスは、わかりやすい名前を使用することです。

デフォルト値

「class=&quot;mktEditable&quot;」を含む HTML 要素内のコンテンツ（指定されている場合）が、リッチテキスト要素のデフォルト値として使用されます。

例:

`<pre data-theme="Confluence"><div class="mktEditable" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

### オプション 2 - mktoText {#option-mktotext}

「class=&quot;mktoText&quot;」構文を使用してリッチテキスト要素を指定することをお勧めします。これにより、常に要素に適切な表示名が付けられます。

必須の属性

* **class**：&quot;mktoText&quot;
* **id**：ID 文字列。文字、数字、ダッシュ（-）、アンダースコア（_）のみが含まれます。スペースは使用できません。一意である必要があります。
* **mktoName**：文字列。これは、Email Editor 2.0 で表示される表示名です。ベストプラクティスは、わかりやすい名前を使用することです。

デフォルト値

「class=&quot;mktoText&quot;」を含む HTML 要素内のコンテンツ（指定されている場合）が、リッチテキスト要素のデフォルト値として使用されます。

例:

`<pre data-theme="Confluence"><div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

## 画像 {#images}

編集可能な画像要素を定義するには、2 つのオプションがあります。`<img>` が挿入されるコンテナを指定する `<div>` または `<img>` タグを使用します。エンドユーザが（DOM ではなく）画像 URL を返す画像を選択するだけの場合、以下の節の「画像変数」を参照してください。次の 2 つのオプションを使用すると、HTML `<img>` 要素が挿入されます。

### オプション 1 - `<div>` の使用 {#option-use-a-div}

必須の属性

* **class**：&quot;mktoImg&quot;.
* **id**：ID 文字列。文字、数字、ダッシュ（-）、アンダースコア（_）のみが含まれます。スペースは使用できません。一意である必要があります。
* **mktoName**：文字列。これは、Email Editor 2.0 で表示される表示名です。ベストプラクティスは、わかりやすい名前を使用することです。

オプションの属性

* **mktoImgClass**：文字列。ここでの値は、div 内の `<img>` 要素のクラス属性に追加されます。
* **mktoImgSrc**：この div 内に配置される画像のデフォルト値として使用されます。省略した場合は、プレースホルダーが使用されます。
* **mktoImgLink**：`<img>` がこの宛先では `<a>` タグに囲まれているはずであることを示します。これは、Email Editor で変更できます。
* **mktoImgLinkTarget：** mktoImgLink 属性の `<a>` タグがこのターゲットを使用する必要があることを示します。mktoImgLink も使用されていない場合は無効です。
* **mktoImgWidth**：閉じた `<img>` の幅として使用されます。
* **mktoImgHeight**：閉じた `<img>` の高さとして使用されます。
* **mktoLockImgSize**：`<img>` 要素の height および width プロパティをエンドユーザが変更できるようにロック解除するために使用します（省略した場合のデフォルトは true）。
* **mktoLockImgStyle**：`<img>` 要素の style プロパティをロックするために使用されます（デフォルトは false）。

デフォルト値（オプション）

**`<img>`**：画像を配置する `<img>` 要素として使用されます。画像にインラインスタイルを追加する場合に役立ちます。ユーザがリンクを追加してもスタイル設定が削除されないように、必ず前後に `<a> </a>` タグを使用してください。

例:

`<pre data-theme="Confluence"><div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="https://www.marketo.com"> <a><img style="border:10px solid red;"></a> </div></pre>`

### オプション 2 - \&lt;img\> の使用 {#option-use-an-img}

>[!NOTE]
>
>このオプションでは、エンドユーザは画像にリンクを追加できません。これがテンプレートにとって重要な場合は、オプション 1 を使用してください。

必須の属性

* **class**：&quot;mktoImg&quot;.
* **id**：ID 文字列。文字、数字、ダッシュ（-）、アンダースコア（_）のみが含まれます。スペースは使用できません。一意である必要があります。
* **mktoName**：文字列。これは、Email Editor 2.0 で表示される表示名です。ベストプラクティスは、わかりやすい名前を使用することです。デフォルト値（オプション）
* **src**：画像のデフォルト値として使用します。省略した場合は、プレースホルダーが使用されます。
* **mktoLockImgSize**：`<img>` 要素の height および width プロパティをエンドユーザが変更できるようにロック解除するために使用します（省略した場合のデフォルトは true）。
* **mktoLockImgStyle**：`<img>` 要素の style プロパティをロックするために使用されます（デフォルトは false）。

例：
`<pre data-theme="Confluence"><img class="mktoImg" id="exampleImg" mktoName="Example Image"></pre>`

## スニペット {#snippets}

地域をスニペットとして定義すると、エンドユーザはこの地域に挿入する承認済みの[スニペット](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-snippet-to-an-email.md)を選択できるようになります。リッチテキスト要素は、メールエディター内からスニペットに変換できますが、特に領域をスニペットとして定義する場合は、リッチテキストに変換できません。スニペット領域を指定するには、`<div>` と「class=”mktoSnippet”」を使用します。

必須の属性

* **id**：ID 文字列。文字、数字、ダッシュ（-）、アンダースコア（_）のみが含まれます。スペースは使用できません。一意である必要があります。
* **mktoName**：文字列。これは、Email Editor 2.0 で表示される表示名です。ベストプラクティスは、わかりやすい名前を使用することです。

デフォルト値（オプション）

**mktoDefaultSnippetId**：デフォルトで表示される Marketo スニペットの数値 ID です（この ID のスニペットが存在し、そのワークスペースで承認されている場合にのみ機能します）。

例:

`<pre data-theme="Confluence"><div class="mktoSnippet" id="unsubscribeFooter" mktoName="Unsubscribe Footer" mktoDefaultSnippetId="12"></div></pre>`

## 動画 {#video}

地域をビデオとして定義すると、エンドユーザは、メールの内部にサムネール画像（「再生」ボタン付き）として表示される YouTube または Vimeo の URL を挿入できます。ビデオ領域を指定するには、`<div>` と「class=”mktoVideo&quot;」を使用します。

必須の属性

* **id**：ID 文字列。文字、数字、ダッシュ（-）、アンダースコア（_）のみが含まれます。スペースは使用できません。一意である必要があります。
* **mktoName**：文字列。これは、Email Editor 2.0 で表示される表示名です。ベストプラクティスは、わかりやすい名前を使用することです。

オプションの属性

* **mktoImgClass**：文字列。ここで指定した値は、div 内のビデオサムネール `<img>` の class 属性に追加されます。

例:

`<pre data-theme="Confluence"><div class="mktoVideo" id="productVideo" mktoName="Product Announcement Video"></div></pre>`

## 変数 {#variables}

変数はトークンに似ています。まず、`<meta>` タグを使用してメールテンプレートの `<head>` セクションで定義し、テンプレート全体で必要な回数だけ使用します。テンプレートで定義されているので、エンドユーザはルールに従って値を変更できます。変数は、スコープ内でローカルまたはグローバルとして定義できます。「モジュール」内で変数を使用し（以下を参照）、エンドユーザがそのモジュールを重複した場合、ローカル変数には独立した値が設定され、グローバル変数は両方のモジュールに適用されます。

## 文字列 {#string}

変数を String として指定した場合、エンドユーザはメールエディターのテキストボックス内にテキストを入力できます。String 変数を指定するには、`<meta>` と「class=“mktoString”」を使用します

必須の属性

* **id**：メールテンプレート内で変数を参照する方法。
* **mktoName**：文字列。これは、Email Editor 2.0 で表示される表示名です。ベストプラクティスは、わかりやすい名前を使用することです。

オプションの属性

* **allowHTML**：ブール値。変数の値が HTML エスケープされているかどうかを制御します。省略した場合のデフォルト値は False です。
* **default**：文字列のデフォルト値。省略した場合は空白です。
* **mktoModuleScope**：ブール値。モジュールで使用する場合に、変数をローカル（true）にするかグローバル（false）にするかを制御します。省略した場合のデフォルト値は False です。

宣言の例：

`<pre data-theme="Confluence"><meta class="mktoString" id="textHeader" mktoName="Text Header" default="Edit Me"></pre>`

使用例：

`<pre data-theme="Confluence">${textHeader}</pre>`

## リスト {#list}

変数を List として指定した場合、エンドユーザはメールエディターで定義した値のセットから選択できます。List 変数を指定するには、`<meta>` と「class=“mktoList”」を使用します。

必須の属性

* **id**：メールテンプレート内で変数を参照する方法。
* **mktoName**：文字列。これは、Email Editor 2.0 で表示される表示名です。ベストプラクティスは、わかりやすい名前を使用することです。
* **values**：値のコンマ区切りリスト。少なくとも 1 つの文字列が必要です。

オプションの属性

* **default**：選択ドロップダウンのデフォルト値。省略した場合は、「values」属性の最初の値が使用されます。
* **mktoModuleScope**：ブール値。モジュールで使用する場合に、変数をローカル（true）にするかグローバル（false）にするかを制御します。省略した場合のデフォルト値は False です。

宣言の例：

`<pre data-theme="Confluence"><meta class="mktoList" id="textFontFamily" mktoName="Main Text Font Family" values="Arial,Verdana,Times New Roman"></pre>`

使用例：

`<pre data-theme="Confluence">${textFontFamily}</pre>`

## 数字 {#number}

変数を数値として指定した場合、エンドユーザはメールエディターで数値を入力できます。Number 変数を指定するには、`<meta>` と「class=“mktoNumber”」を使用します。

必須の属性

* **id**：メールテンプレート内で変数を参照する方法。
* **mktoName**：文字列。これは、Email Editor 2.0 で表示される表示名です。ベストプラクティスは、わかりやすい名前を使用することです。
* **default**：変数のデフォルトの数値。

オプションの属性

* **min**：最小許容値。
* **max**：最大許容値。
* **units**：メールエディターおよび結果のコードに表示される場合に、数値に追加する単位（例：px、pt、em など）。
* **step**：数値変数の増減単位数（0.1、1、10 など）。省略した場合のデフォルト値は 1 です。
* **mktoModuleScope**：ブール値。モジュールで使用する場合に、変数をローカル（true）にするかグローバル（false）にするかを制御します。省略した場合のデフォルト値は False です。

宣言の例：

`<pre data-theme="Confluence"><meta class="mktoNumber" id="textFontSize" mktoName="Main Text Font Size" default="12" min="8" max="18" units="px" step="1"> </pre>`

使用例：

`<pre data-theme="Confluence">${textFontSize}</pre>`

## 色 {#color}

変数を Color として指定した場合、エンドユーザは 16 進数の色値を入力したり、メールエディター内のカラーピッカーから色を選択したりできます。Color 変数を指定するには、`<meta>` と「class=“mktoColor”」を使用します。

必須の属性

* **id**：メールテンプレート内で変数を参照する方法。
* **mktoName**：文字列。これは、Email Editor 2.0 で表示される表示名です。ベストプラクティスは、わかりやすい名前を使用することです。

オプションの属性

* **default**：カラーのデフォルト値。6 桁の 16 進数カラーコード（例：#ffffff）。
* **mktoModuleScope**：ブール値。モジュールで使用する場合に、変数をローカル（true）にするかグローバル（false）にするかを制御します。省略した場合のデフォルト値は False です。

宣言の例：

`<pre data-theme="Confluence"><meta class="mktoColor" id="textColor" mktoName="Main Text Color" default="#FFFFFF"></pre>`

使用例：

`<pre data-theme="Confluence">${textColor}</pre>`

## ブール値 {#boolean}

変数をブール値として指定した場合、エンドユーザはメールエディター内でオプションのオンとオフを切り替えることができます。Boolean 変数を指定するには、`<meta>` と「class=“mktoBoolean”」を使用します。

必須の属性

* **id**：メールテンプレート内で変数を参照する方法。
* **mktoName**：文字列。これは、Email Editor 2.0 で表示される表示名です。ベストプラクティスは、わかりやすい名前を使用することです。

オプションの属性

* **default**：切り替えスイッチのデフォルトの状態を決定するブール値。省略した場合は False です。
* **false_value**：切り替えがオフの場合に挿入される値。省略した場合は False です。
* **true_value**：切り替えがオンの場合に挿入される値。省略した場合は True です。
* **false_value_name**：OFF の場合にトグルに表示される UI。省略した場合は False です。
* **true_value_name**：ON の場合にトグルに表示される UI。省略した場合は True です。
* **mktoModuleScope**：ブール値。モジュールで使用する場合に、変数をローカル（true）にするかグローバル（false）にするかを制御します。省略した場合のデフォルト値は False です。

宣言の例：

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="showFooter" mktoName="Show Footer BG?" default="false" false_value="transparent" true_value="black" false_value_name="NO" true_value_name="YES"></pre>`

使用例：

`<pre data-theme="Confluence">${showFooter}</pre>`

## HTML ブロック {#html-block}

変数を HTML ブロックとして指定した場合、エンドユーザはメールエディター内から字句の HTML を入力できます。HTML Block 変数を指定するには、`<meta>` と「class=“mktoHTML”」を使用します

必須の属性

* **id**：メールテンプレート内で変数を参照する方法。
* **mktoName**：文字列。これは、Email Editor 2.0 で表示される表示名です。ベストプラクティスは、わかりやすい名前を使用することです。

オプションの属性

* **default**：HTML エンコードされた値。ブロックのデフォルトコンテンツとして機能します。
* **mktoModuleScope**：ブール値。モジュールで使用する場合に、変数をローカル（true）にするかグローバル（false）にするかを制御します。省略した場合のデフォルト値は False です。

宣言の例：

`<pre data-theme="Confluence"><meta class="mktoHTML" id="trackingPixel" mktoName="Add Tracking Pixel"></pre>`

使用例：

`<pre data-theme="Confluence">${trackingPixel}</pre>`

## 画像変数 {#image-variable}

変数を Image として指定した場合、エンドユーザはメールエディター内の画像ピッカーから画像を選択できます。選択した画像 URL が変数の値になります。Image 変数を指定するには、`<meta>` と「class=“mktoImg”」を使用します。

必須の属性

* **id**：メールテンプレート内で変数を参照する方法。
* **mktoName**：文字列。これは、Email Editor 2.0 で表示される表示名です。ベストプラクティスは、わかりやすい名前を使用することです。

オプションの属性

* **default**：要素のデフォルトの画像 URL。
* **mktoModuleScope**：ブール値。モジュールで使用する場合に、変数をローカル（true）にするかグローバル（false）にするかを制御します。省略した場合のデフォルト値は False です。

宣言の例：

`<pre data-theme="Confluence"><meta class="mktoImg" id="heroBackgroundImage" mktoName="Hero Background Image" default="https://www.company.com/image.jpg"></pre>`

使用例：

`<pre data-theme="Confluence">${heroBackgroundImage}</pre>`

## モジュール {#modules}

モジュールは、テンプレートレベルで定義されるテンプレート化されたセクションで、エンドユーザがメールに挿入するために表示されます。これらのモジュールは事前に作成されているので、残りのメールコンテンツと適切に（完全にレスポンシブな方法で）やり取りできます。コンテナに配置できるのはモジュールのみです。

>[!IMPORTANT]
>
>定義済みのモジュールコンポーネントを含むメールテンプレートからメールが生成されると、テンプレートのモジュールに対して行われた変更は、当該メールにプッシュ&#x200B;**されません**。

**`<table>`、`<tbody>`、`<thead>`、`<tfoot>` のいずれかのタイプのコンテナの場合：**

`<tr>` と「class=”mktoModule”」を使用して指定

**タイプのコンテナの場合 `<td>`：**

`<table>` と「class=”mktoModule”」を使用して指定

必須の属性

* **id**：メールテンプレート内でのモジュールの参照方法。
* **mktoName**：文字列。これは、Email Editor 2.0 で表示される表示名です。ベストプラクティスは、わかりやすい名前を使用することです。

オプションの属性

* **mktoActive**：このモジュールをメールエディター内のモジュールのリストに表示するかどうかを決定します。デフォルトは True です。False の場合、エンドユーザはモジュールをメールに追加できません。
* **mktoAddByDefault**：作成時にこのテンプレートを使用する新しいメールのキャンバスにこのモジュールを配置するかどうかを指定します。デフォルトは True です（mktoActive が False の場合、この値は無視されます）。

>[!NOTE]
>
>Marketo 構文（mktoModule、mktoContainer、mktoText）を含むクラス値では、大文字と小文字が区別されます。カスタム属性名（mktoimgwidth、mktoname）は使用できません。

## コンテナ {#containers}

コンテナにはモジュールが格納され、それらを配置できる場所を定義します。エンドユーザがモジュールを並べ替えてメールに挿入する際、コンテナは、モジュールの移動先を制御します。

**`<table>`、`<tbody>`、`<thead>`、`<tfoot>`、`<td>` のいずれかと「class=”mktoContainer”」で指定されます**。

必須の属性

**id**：メールテンプレート内でのモジュールの参照方法。

>[!CAUTION]
>
>コンテナには、モジュールのみを含めることができます。他に何かが存在する場合、コンテナは無効と見なされます。1 つのテンプレートにつき、1 つのコンテナのみを使用できます。
