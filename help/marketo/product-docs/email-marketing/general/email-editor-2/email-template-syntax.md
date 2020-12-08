---
unique-page-id: 11371040
description: 電子メールテンプレート構文 — Marketto Docs — 製品ドキュメント
title: 電子メールテンプレートの構文
translation-type: tm+mt
source-git-commit: f27e2bac90570f9f795dc6bdd5fcf208c446be14
workflow-type: tm+mt
source-wordcount: '2397'
ht-degree: 0%

---


# 電子メールテンプレートの構文 {#email-template-syntax}

Marketingの新しい電子メール2.0エクスペリエンスでは、電子メールテンプレートは、コンテナ、変数、モジュールまたは要素の任意の組み合わせで構成されます。 それぞれは、HTMLにMarketor固有の構文を追加することで定義します。 古い(v1.0)電子メールテンプレートは、電子メールエディタ2.0でサポートされています。ただし、エディタの新機能の一部は含まれません。

マーケティング担当者の電子メールの構文は、テンプレートと個々の電子メールでのみ機能します。スニペットやリッチテキストのトークンに埋め込まれている場合 **は** 、機能しません。

>[!NOTE]
>
>Marketorのサポートは、CSS/HTMLを支援するために設定されていません。 CSS/HTMLに詳しくない場合は、開発者にお問い合わせください。

>[!CAUTION]
>
>Marketo構文を含むクラス値（mktoModule、mktoContainer、mktoTextなど）では大文字と小文字が区別されます。 カスタム属性名（例： mktoimgwidth, mktoname）は使用できません。

## 要素 {#elements}

要素とは、電子メールテンプレートで編集可能として定義したコンテンツ領域です。 要素の編集操作は、要素のタイプやオファーに固有のもので、コンテンツを簡単に操作できます。 電子メールテンプレートに含めることのできる要素は次のとおりです。

* リッチテキスト
* 画像
* スニペット
* ビデオ

## リッチテキスト {#rich-text}

地域をリッチテキストとして定義すると、ユーザーは、マーケティング担当者のリッチテキストエディター [を使用して、そのコンテンツを編集できます](../../../../product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md)。 電子メールテンプレート内にリッチテキスト要素を定義する方法は2つあります。mktEditableとmktoText。 リッチテキスト要素は、電子メールエディター内から常にスニペットに変換できます。

### オプション1 - mktEditable {#option-mkteditable}

電子メールエディタ2.0は下位互換性があるので、一部の古い電子メールテンプレートでは、任意のHTML要素にclass=&quot;mktEditable&quot;を追加することで、リッチテキスト要素を指定できます。 これは引き続きサポートされ、要素のIDが電子メールエディター内の表示名として使用されます。

必須属性

* **class**:&quot;mktEditable&quot;と表示されます。
* **id**:ID文字列。 文字、数字、ダッシュ「 — 」、下線「_」のみが含まれます。 スペースは使用できません。 一意である必要があります。

オプションの属性

* **mktoName** :文字列。 これは、電子メールエディタ2.0で表示される表示名です。説明的な名前を使用することをお勧めします。

デフォルト値

class=&quot;mktEditable&quot;で指定されているHTML要素内のコンテンツは、リッチテキスト要素のデフォルト値として使用されます。

例：

`<pre data-theme="Confluence"><div class="mktEditable" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

### オプション2 - mktoText {#option-mktotext}

class=&quot;mktoText&quot;構文を使用してリッチテキスト要素を指定することをお勧めします。 これにより、要素に対して常に適切な表示名が付けられます。

必須属性

* **class**:&quot;mktoText&quot;
* **id**:ID文字列。 文字、数字、ダッシュ「 — 」、下線「_」のみが含まれます。 スペースは使用できません。 一意である必要があります。
* **mktoName** :文字列。 これは、電子メールエディタ2.0で表示される表示名です。説明的な名前を使用することをお勧めします。

デフォルト値

class=&quot;mktoText&quot;と共にHTML要素内のコンテンツ（指定されている場合）が、リッチテキスト要素のデフォルト値として使用されます。

例：

`<pre data-theme="Confluence"><div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

## 画像 {#images}

編集可能な画像要素を定義するオプションは2つあります。 には、挿入するコンテナ `<div>`を指定するタグ、また `<img>` は `<img>` タグを使用できます。 エンドユーザーが（DOMではなく）画像URLを返す画像を選択する場合は、以下の節の「画像変数」を参照してください。 次の2つのオプションは、HTML `<img>` 要素を挿入します。

### オプション1 - \&lt;div\>を使用 {#option-use-a-div}

必須属性

* **クラス：** &quot;mktoImg&quot;.
* **id:** ID文字列。 文字、数字、ダッシュ「 — 」、下線「_」のみが含まれます。 スペースは使用できません。 一意である必要があります。
* **mktoName :** 文字列。 これは、電子メールエディタ2.0で表示される表示名です。説明的な名前を使用することをお勧めします。

オプションの属性

* **mktoImgClass:** 文字列。 ここの値は、div内の `<img>` 要素のclass属性に追加されます。
* **mktoImgSrc:** このdiv内に配置される画像のデフォルト値として使用されます。 これを省略すると、プレースホルダが使用されます。
* **mktoImgLink:** このリンク先URLを含む `<img>``<a>` タグで囲む必要があることを示します。 ユーザーは、電子メールエディターでこれを変更できます。
* **mktoImgLinkTarget:** mktoImgLink属性の `<a>` タグでこのターゲットを使用する必要があることを示します。 mktoImgLinkも使用しない場合は無効です。
* **mktoImgWidth:** 囲まれた領域の幅として使用され `<img>`ます。
* **mktoImgHeight:** 囲まれたオブジェクトの高さとして使用され `<img>`ます。
* **mktoLockImgSize:** エンドユーザーが変更できるように、 `<img>` 要素のheightとwidthのプロパティのロックを解除するために使用します（省略した場合のデフォルトはtrueです）。
* **mktoLockImgStyle:** 要素のstyleプロパティをロックするために使用します（デフォルトはfalse）。 `<img>`

デフォルト値（オプション）

**`<img>`**:画像を配置する `<img>` 要素として使用します。 画像にインラインスタイルを追加する場合に役立ちます。 周囲の `<a> </a>` タグを必ず含めてください。ユーザーがリンクを追加した場合、スタイルは削除されません。

例：

`<pre data-theme="Confluence"><div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="http://www.marketo.com"> <a><img style="border:10px solid red;"></a> </div></pre>`

### オプション2 - \&lt;img\> {#option-use-an-img}

>[!NOTE]
>
>このオプションでは、エンドユーザーは画像にリンクを追加できません。 これがテンプレートにとって重要な場合は、オプション1を使用します。

必須属性

* **クラス：** &quot;mktoImg&quot;.
* **id:** ID文字列。 文字、数字、ダッシュ「 — 」、下線「_」のみが含まれます。 スペースは使用できません。 一意である必要があります。
* **mktoName:** 文字列。 これは、電子メールエディタ2.0で表示される表示名です。説明的な名前を使用することをお勧めします。  デフォルト値（オプション）
* **src:** 画像のデフォルト値として使用されます。 これを省略すると、プレースホルダが使用されます。
* **mktoLockImgSize:** エンドユーザーが変更できるように、 `<img>` 要素のheightとwidthのプロパティのロックを解除するために使用します（省略した場合のデフォルトはtrueです）。
* **mktoLockImgStyle:** 要素のstyleプロパティをロックするために使用します（デフォルトはfalse）。 `<img>`

例：
`<pre data-theme="Confluence"><img class="mktoImg" id="exampleImg" mktoName="Example Image"></pre>`

## スニペット {#snippets}

地域をスニペットとして定義する場合、エンドユーザーは、この地域に挿入する承認済みの [](../../../../product-docs/email-marketing/general/functions-in-the-editor/add-a-snippet-to-an-email.md)Snippetを選択できます。 リッチテキスト要素は電子メールエディター内からスニペットに変換できますが、特に領域をスニペットとして定義する場合は、リッチテキストに変換できません。 スニペット領域は、class=&quot;mktoSnippet&quot; `<div>` を使用して指定できます。

必須属性

* **id:** ID文字列。 文字、数字、ダッシュ「 — 」、下線「_」のみが含まれます。 スペースは使用できません。 一意である必要があります。
* **mktoName:** 文字列。 これは、電子メールエディタ2.0で表示される表示名です。説明的な名前を使用することをお勧めします。

デフォルト値（オプション）

**mktoDefaultSnippetId**:デフォルトで表示される必要があるマーケティング担当者のスニペットの数値ID（そのIDを持つスニペットが存在し、そのワークスペースで承認されている場合のみ機能します）。

例：

`<pre data-theme="Confluence"><div class="mktoSnippet" id="unsubscribeFooter" mktoName="Unsubscribe Footer" mktoDefaultSnippetId="12"></div></pre>`

## ビデオ {#video}

領域をビデオとして定義する場合、エンドユーザーは、電子メール内にサムネール画像（「再生」ボタン付き）として表示されるYouTubeまたはVimeoのURLを挿入できます。 ビデオ領域は、class=&quot;mktoVideo&quot; `<div>` を使用して指定できます

必須属性

* **id:** ID文字列。 文字、数字、ダッシュ「 — 」、下線「_」のみが含まれます。 スペースは使用できません。 一意である必要があります。
* **mktoName:** 文字列。 これは、電子メールエディタ2.0で表示される表示名です。説明的な名前を使用することをお勧めします。

オプションの属性

* **mktoImgClass:** 文字列。 ここでの値は、div `<img>` 内のビデオサムネールのclass属性に追加されます。

例：

`<pre data-theme="Confluence"><div class="mktoVideo" id="productVideo" mktoName="Product Announcement Video"></div></pre>`

## 変数 {#variables}

変数はトークンに似ています。 最初に、タグを使用して電子メールテンプレートの `<head>` セクション内で `<meta>` タグを定義し、テンプレート全体で必要な回数だけ使用します。 エンドユーザーはテンプレート内で定義されているので、ルールに従って値を変更できます。 変数は、スコープ内でローカルまたはグローバルとして定義できます。 変数を「モジュール」内で使用し（下記を参照）、そのモジュールをエンドユーザー重複で使用する場合、ローカル変数は独立した値を持ち、グローバル変数は両方のモジュールに適用されます。

## 文字列 {#string}

変数を文字列(String)として指定した場合、エンドユーザーは電子メールエディターのテキストボックス内にテキストを入力できます。 String変数は、class=&quot;mktoString&quot; `<meta>` と共に指定します。

必須属性

* **id:** 電子メールテンプレート内での変数の参照方法。
* **mktoName:** 文字列。 これは、電子メールエディタ2.0で表示される表示名です。説明的な名前を使用することをお勧めします。

オプションの属性

* **allowHTML:** ブール値。 変数の値がHTMLエスケープかどうかを制御します。 省略した場合はFalseをデフォルトにします。
* **default**:文字列のデフォルト値。 省略した場合は空白。
* **mktoModuleScope**:ブール値。 変数をモジュールで使用する場合に、変数をローカル(true)にするかグローバル(false)にするかを制御します。 省略した場合はFalseをデフォルトにします。

宣言の例：

`<pre data-theme="Confluence"><meta class="mktoString" id="textHeader" mktoName="Text Header" default="Edit Me"></pre>`

使用例：

`<pre data-theme="Confluence">${textHeader}</pre>`

## リスト {#list}

変数をリストとして指定すると、エンドユーザーは電子メールエディターで定義した値のセットから選択できます。 リスト変数は、class=&quot;mktoList&quot; `<meta>` と共に指定します。

必須属性

* **id**:電子メールテンプレート内での変数の参照方法。
* **mktoName:** 文字列。 これは、電子メールエディタ2.0で表示される表示名です。説明的な名前を使用することをお勧めします。
* **値：** 値のコンマ区切りリスト。 文字列が少なくとも1つ必要です。

オプションの属性

* **デフォルト：** 選択ドロップダウンのデフォルト値。 省略した場合は、「values」属性の最初の値が使用されます。
* **mktoModuleScope**:ブール値。 変数をモジュールで使用する場合に、変数をローカル(true)にするかグローバル(false)にするかを制御します。 省略した場合はFalseをデフォルトにします。

宣言の例：

`<pre data-theme="Confluence"><meta class="mktoList" id="textFontFamily" mktoName="Main Text Font Family" values="Arial,Verdana,Times New Roman"></pre>`

使用例：

`<pre data-theme="Confluence">${textFontFamily}</pre>`

## 数値 {#number}

変数をNumberとして指定した場合、エンドユーザーは電子メールエディターで数値を入力できます。 Number変数は、class=&quot;mktoNumber&quot; `<meta>` と共に指定します。

必須属性

* **id**:電子メールテンプレート内での変数の参照方法。
* **mktoName**:文字列。 これは、電子メールエディタ2.0で表示される表示名です。説明的な名前を使用することをお勧めします。
* **デフォルト：** 変数のデフォルトの数値。

オプションの属性

* **min:** 最小許容値。
* **max:** 許容される最大値。
* **数量：** 数値に追加する単位(例：px、pt、emなど) と表示されます。
* **手順：** number変数の増減単位数（0.1、1、10など）。 省略した場合、デフォルトは1です。
* **mktoModuleScope**:ブール値。 変数をモジュールで使用する場合に、変数をローカル(true)にするかグローバル(false)にするかを制御します。 省略した場合はFalseをデフォルトにします。

宣言の例：

`<pre data-theme="Confluence"><meta class="mktoNumber" id="textFontSize" mktoName="Main Text Font Size" default="12" min="8" max="18" units="px" step="1"> </pre>`

使用例：

`<pre data-theme="Confluence">${textFontSize}</pre>`

## カラー {#color}

変数をColorとして指定した場合、エンドユーザーは16進値を入力したり、電子メールエディター内のカラーピッカーから色を選択したりできます。 Color変数は、class=&quot;mktoColor&quot; `<meta>` と共に指定します。

必須属性

* **id**:電子メールテンプレート内での変数の参照方法。
* **mktoName**:文字列。 これは、電子メールエディタ2.0で表示される表示名です。説明的な名前を使用することをお勧めします。

オプションの属性

* **デフォルト：** 色のデフォルト値。 6桁の16進数カラーコード。 例：#ffffff.
* **mktoModuleScope**:ブール値。 変数をモジュールで使用する場合に、変数をローカル(true)にするかグローバル(false)にするかを制御します。 省略した場合はFalseをデフォルトにします。

宣言の例：

`<pre data-theme="Confluence"><meta class="mktoColor" id="textColor" mktoName="Main Text Color" default="#FFFFFF"></pre>`

使用例：

`<pre data-theme="Confluence">${textColor}</pre>`

## ブール値 {#boolean}

変数をブール値として指定した場合、エンドユーザーは電子メールエディター内でオプションのオン/オフを切り替えることができます。 Boolean変数は、class=&quot;mktoBoolean&quot; `<meta>` と共に指定します。

必須属性

* **id**:電子メールテンプレート内での変数の参照方法。
* **mktoName**:文字列。 これは、電子メールエディタ2.0で表示される表示名です。説明的な名前を使用することをお勧めします。

オプションの属性

* **デフォルト：** トグルスイッチのデフォルト状態を決定するブール値。 省略した場合はfalse。
* **false_value:** トグルがオフの位置にある場合に挿入される値。 省略した場合はfalse。
* **true_value:** トグルがオンの位置にある場合に挿入される値。 省略した場合はtrue。
* **false_value_name:** OFF位置の場合にトグルに表示されるUI。 省略した場合はfalse。
* **true_value_name:** オンの位置にある場合にトグルに表示されるUI。 省略した場合はtrue。
* **mktoModuleScope**:ブール値。 変数をモジュールで使用する場合に、変数をローカル(true)にするかグローバル(false)にするかを制御します。 省略した場合はFalseをデフォルトにします。

宣言の例：

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="showFooter" mktoName="Show Footer BG?" default="false" false_value="transparent" true_value="black" false_value_name="NO" true_value_name="YES"></pre>`

使用例：

`<pre data-theme="Confluence">${showFooter}</pre>`

## HTMLブロック {#html-block}

変数をHTMLブロックとして指定した場合、エンドユーザーは電子メールエディター内から字句のHTMLを入力できます。 HTMLブロック変数は、class=&quot;mktoHTML&quot; `<meta>` と共に指定します。

必須属性

* **id**:電子メールテンプレート内での変数の参照方法。
* **mktoName**:文字列。 これは、電子メールエディタ2.0で表示される表示名です。説明的な名前を使用することをお勧めします。

オプションの属性

* **デフォルト：** ブロックのデフォルトコンテンツとして機能するHTMLエンコード値。
* **mktoModuleScope**:ブール値。 変数をモジュールで使用する場合に、変数をローカル(true)にするかグローバル(false)にするかを制御します。 省略した場合はFalseをデフォルトにします。

宣言の例：

`<pre data-theme="Confluence"><meta class="mktoHTML" id="trackingPixel" mktoName="Add Tracking Pixel"></pre>`

使用例：

`<pre data-theme="Confluence">${trackingPixel}</pre>`

## 画像変数 {#image-variable}

変数を画像として指定した場合、エンドユーザーは電子メールエディター内の画像選択から画像を選択できます。 選択した画像URLが変数の値になります。 画像変数を指定するには、class=&quot;mktoImg&quot; `<meta>` を使用します

必須属性

* **id**:電子メールテンプレート内での変数の参照方法。
* **mktoName**:文字列。 これは、電子メールエディタ2.0で表示される表示名です。説明的な名前を使用することをお勧めします。

オプションの属性

* **デフォルト：** 要素の初期設定の画像URL。
* **mktoModuleScope**:ブール値。 変数をモジュールで使用する場合に、変数をローカル(true)にするかグローバル(false)にするかを制御します。 省略した場合はFalseをデフォルトにします。

宣言の例：

`<pre data-theme="Confluence"><meta class="mktoImg" id="heroBackgroundImage" mktoName="Hero Background Image" default="http://www.company.com/image.jpg"></pre>`

使用例：

`<pre data-theme="Confluence">${heroBackgroundImage}</pre>`

## モジュール {#modules}

モジュールは、テンプレートレベルで定義されたテンプレート化されたセクションで、エンドユーザーが電子メールに挿入できるように表示されます。 これらのモジュールは事前にビルドされているので、モジュールが残りの電子メールコンテンツを適切に（完全にレスポンシブな方法で）やり取りするようにできます。 コンテナには1つのモジュールのみを入れることができます。

**コンテナのタイプ `<table>`、、、、、 `<tbody>`、 `<thead>`または `<tfoot>`:**

class=&quot;mktoModule&quot; `<tr>` を使用して指定

**コンテナのタイプ `<td>`:**

class=&quot;mktoModule&quot; `<table>` を使用して指定

必須属性

* **id**:電子メールテンプレート内でのモジュールの参照方法。
* **mktoName**:文字列。 これは、電子メールエディタ2.0で表示される表示名です。説明的な名前を使用することをお勧めします。

オプションの属性

* **mktoActive:** 電子メールエディター内のモジュールのリストにこのモジュールを表示するかどうかを指定します。 デフォルトはtrueです。 falseの場合、エンドユーザーはモジュールを電子メールに追加できません。
* **mktoAddByDefault:** 作成時にこのテンプレートを使用する新しい電子メールのキャンバスにこのモジュールを含めるかどうかを指定します。 デフォルトはtrueです（mktoActiveがfalseの場合、この値は無視されます）。

>[!NOTE]
>
>**Reminder**
>
>Marketo構文を含むクラス値（mktoModule、mktoContainer、mktoTextなど）では大文字と小文字が区別されます。 カスタム属性名（例： mktoimgwidth, mktoname）は使用できません。

## コンテナ {#containers}

コンテナにはModulesが格納され、それらを配置できる場所が定義されます。 エンドユーザーがモジュールの順序を変更し、電子メールにモジュールを挿入する場合、コンテナがどこに移動するかを制御します。

**、、、 `<table>`または `<tbody>``<thead>``<tfoot>``<td>` class=&quot;mktoContainer&quot;を使用して指定します。**

必須属性

**id**:電子メールテンプレート内でのモジュールの参照方法。

>[!CAUTION]
>
>コンテナにはModulesのみを含めることができます。他に何かある場合、コンテナは無効と見なされます。 1つのテンプレートにつき1つのコンテナのみ使用できます。
