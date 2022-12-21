---
unique-page-id: 7515401
description: ガイド付きランディングページテンプレートの作成 - Marketo ドキュメント - 製品ドキュメント
title: ガイド付きランディングページテンプレートの作成
exl-id: 7d097162-d862-4d09-9440-aba1628450c2
source-git-commit: 115b6e97978778a1d1e13478adf6fee625aa5257
workflow-type: tm+mt
source-wordcount: '1254'
ht-degree: 100%

---

# ガイド付きランディングページテンプレートの作成 {#create-a-guided-landing-page-template}

ガイド付きランディングページテンプレートには、特別な構文があります。この構文を使用して、カスタマイズ可能な内容と、テンプレートから作成された各ランディングページで最終的にコンテンツが生成される場所を指定します。「ガイド付き」ランディングページエディター内でカスタマイズできるのは、編集可能として指定した地域または変数のみです。

>[!TIP]
>
>命名規則を適切に使用すると、マーケティングチームに感謝されるでしょう。

ページ上の何かを編集可能にする必要があると宣言する方法は 2 つあります。

* オブジェクトを「要素」として宣言します。ランディングページ作成者は、画像、テキストまたは Marketo のアセットを指定された領域に追加できます。
* 文字列を「変数」として宣言します。ランディングページ作成者は、true／false のレバーから、その変数を文字列、色またはブール値の状態に置き換えることができます。

## 編集可能な要素 {#editable-elements}

要素は、通常の DOM 要素をテンプレートに追加し、その要素を Marketo 固有のクラス名で修飾することで宣言されます。

## テキスト {#text}

地域をリッチテキストとして定義すると、[Marketo のリッチテキストエディターを使用](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md)してそのコンテンツを編集できます。

必須属性：\
**class**：&quot;mktoText&quot;\
**id**：ID 文字列。文字、数字、ダッシュ（-）、アンダースコア（_）のみが含まれます。スペースは使用できません。一意である必要があります。\
**mktoName**：文字列。これは、ランディングページエディターに表示される表示名です。ベストプラクティスは、わかりやすい名前を使用することです。

任意:\
mktoText クラスを持つ要素のコンテンツ（指定されている場合）は、編集可能領域のデフォルト値として使用されます。

例:

`<div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area.</div>`

## 画像 {#image}

編集可能な画像要素を定義するには、2 つのオプションがあります。画像を挿入するコンテナを指定する `<div>`、または `<img>` タグのいずれかを使用できます。

## オプション 1 - `<div>` の使用 {#option-use-a-div}

必須属性：

class：&quot;mktoImg&quot;\
id：ID 文字列。文字、数字、ダッシュ（-）、アンダースコア（_）のみが含まれます。スペースは使用できません。一意である必要があります。\
mktoName：文字列。これは、ランディングページエディターに表示される表示名です。ベストプラクティスは、わかりやすい名前を使用することです。

任意:\
mktoImgClass：文字列。ここでの値は、div 内の `<img>` 要素のクラス属性に追加されます。

例:

`<div class="mktoImg" id="exampleImg" mktoName="Example Image"></div>`

## オプション 2 - `<img>` の使用 {#option-use-a-img}

必須属性：\
class：&quot;mktoImg&quot;\
id：ID 文字列。文字、数字、ダッシュ（-）、アンダースコア（_）のみが含まれます。スペースは使用できません。一意である必要があります。\
mktoName：文字列。これは、ランディングページエディターに表示される表示名です。ベストプラクティスは、わかりやすい名前を使用することです。

任意:\
src：文字列 URL。これは、画像のデフォルト値として使用されます。

例:

`<img class="mktoImg" id="exampleImg" mktoName="Example Image">`

>[!NOTE]
>
>`<img>` バージョンを使用する場合、レンダリングされた HTML には `<img>` タグの周りに生成された div ラッパーが含まれます。クラス「mktoImg.mktoGen」に指定されて、display:inline-block となります。

## フォーム {#form}

例：必須属性：\
**class**：&quot;mktoForm&quot;\
**id**：ID 文字列。文字、数字、ダッシュ（-）、アンダースコア（_）のみが含まれます。スペースは使用できません。一意である必要があります。\
**mktoName**：文字列。これは、ランディングページエディターに表示される表示名です。ベストプラクティスは、わかりやすい名前を使用することです。

`<div class="mktoForm" id="exampleForm" mktoName="Example Form"></div>`

## スニペット {#snippet}

必須属性：\
**class**：&quot;mktoSnippet&quot;\
**id**：ID 文字列。文字、数字、ダッシュ（-）、アンダースコア（_）のみが含まれます。スペースは使用できません。一意である必要があります。\
**mktoName**：文字列。これは、ランディングページエディターに表示される表示名です。ベストプラクティスは、わかりやすい名前を使用することです。

例:

`<div class="mktoSnippet" id="exampleSnippet" mktoName="Example Snippet"></div>`

## 共有ボタン {#share-button}

必須属性：\
**class**：&quot;mktoShareButton&quot;\
**id**：ID 文字列。文字、数字、ダッシュ（-）、アンダースコア（_）のみが含まれます。スペースは使用できません。一意である必要があります。\
**mktoName**：文字列。これは、ランディングページエディターに表示される表示名です。ベストプラクティスは、わかりやすい名前を使用することです。

例:

`<div class="mktoShareButton" id="exampleShareButton" mktoName="Example Share Button"></div>`

## 動画 {#video}

>[!NOTE]
>
>ランディングページでビデオ要素を使用する場合、Marketo は YouTube のビデオのみをサポートします。別のサービスを使用する場合は、リッチテキストボックスを使用してビデオの埋め込みコードに貼り付けることをお勧めします。

必須属性：
**class**：&quot;mktoVideo&quot;
**id**：ID 文字列。文字、数字、ダッシュ（-）、アンダースコア（_）のみが含まれます。スペースは使用できません。一意である必要があります。**mktoName**：文字列。これは、ランディングページエディターに表示される表示名です。ベストプラクティスは、わかりやすい名前を使用することです。

例:

`<div class="mktoVideo" id="exampleVideo" mktoName="Example Video"></div>`

## 投票 {#poll}

必須属性：\
**class**：&quot;mktoPoll&quot;\
**id**：ID 文字列。文字、数字、ダッシュ（-）、アンダースコア（_）のみが含まれます。スペースは使用できません。一意である必要があります。\
**mktoName**：文字列。これは、ランディングページエディターに表示される表示名です。ベストプラクティスは、わかりやすい名前を使用することです。

例:

`<div class="mktoPoll" id="examplePoll" mktoName="Example Poll"></div>`

## 参照元 {#referral}

必須属性：\
**class**：&quot;mktoReferral&quot;\
**id**：ID 文字列。文字、数字、ダッシュ（-）、アンダースコア（_）のみが含まれます。スペースは使用できません。一意である必要があります。\
**mktoName**：文字列。これは、ランディングページエディターに表示される表示名です。ベストプラクティスは、わかりやすい名前を使用することです。

例:

`<div class="mktoReferral" id="exampleReferral" mktoName="Example Referral"></div>`

## 懸賞 {#sweepstakes}

必須属性：\
**class**：&quot;mktoSweepstakes&quot;\
**id**：ID 文字列。文字、数字、ダッシュ（-）、アンダースコア（_）のみが含まれます。スペースは使用できません。一意である必要があります。\
**mktoName**：文字列。これは、ランディングページエディターに表示される表示名です。ベストプラクティスは、わかりやすい名前を使用することです。

例:

`<div class="mktoSweepstakes" id="exampleSweepstakes" mktoName="Example Sweepstakes"></div>`

## 編集可能な変数 {#editable-variables}

すべての変数型は、${ } 文字シーケンスで囲まれた id 属性の値を参照することで使用されます。これらは、他の変数宣言内を除き、ドキュメント内の任意の場所で使用できます。

例:

`${var1}`

**宣言：**

変数は、テンプレートの `<head>` 要素内でメタタグとして宣言されます。使用できる変数は文字列、色、およびブール値の 3 種類です。

## 文字列 {#string}

必須属性：\
**class**：&quot;mktoString&quot;,\
**id**：ID 文字列。文字、数字、ダッシュ（-）、アンダースコア（_）のみが含まれます。スペースは使用できません。一意である必要があります。\
**mktoName**：文字列。これは、ランディングページエディターに表示される表示名です。ベストプラクティスは、わかりやすい名前を使用することです。

任意:\
**default**：属性の文字列値。何も指定しない場合は空白です。\
**allowHtml**：&quot;true&quot; または &quot;false&quot;HTML をエスケープせずに値を出力するかどうかを制御します。未設定の場合はデフォルトで「false」に設定されます。

基本的な例：

`<meta class="mktoString" id="var1" mktoName="My Variable">`

すべての属性の例：

`<meta class="mktoString" id="var1" mktoName="My Variable" default="This is my default value" allowHtml="true">`

## 色 {#color}

必須属性：\
**class**：&quot;mktoColor&quot;\
**id**：ID 文字列。文字、数字、ダッシュ（-）、アンダースコア（_）のみが含まれます。スペースは使用できません。一意である必要があります。\
**mktoName**：文字列。これは、ランディングページエディターに表示される表示名です。ベストプラクティスは、わかりやすい名前を使用することです。

任意:\
**default**：7 桁の 16 進数のカラーコード。例：#336699

基本的な例：

`<meta class="mktoColor" id="color1" mktoName="My Color Variable">`

すべての属性の例：

`<meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699">`

## ブール値 {#boolean}

必須属性：\
**class**：&quot;mktoBoolean&quot;\
**id**：ID 文字列。文字、数字、ダッシュ（-）、アンダースコア（_）のみが含まれます。スペースは使用できません。一意である必要があります。\
**mktoName**：文字列。これは、ランディングページエディターに表示される表示名です。ベストプラクティスは、わかりやすい名前を使用することです。

任意:\
**default**：ブール文字列。「true」と「false」は、値が ON の位置で始まるか OFF の位置で始まるかを制御します。指定しない場合は「false」です。\
**false_value**：文字列。変数が OFF 位置にあるときに挿入される値です。指定しない場合は「false」です。\
**true_value**：文字列。変数が ON 位置にあるときに挿入される値です。指定されない場合は「true」です。\
**false_value_name**：文字列。値がオフの位置にあるときにランディングページエディターに表示される表示名です。指定されていない場合は「OFF」です。\
**true_value_name**：文字列。値がオンの位置にある場合にランディングページエディターに表示される表示名です。指定されていない場合は「ON」です。

基本的な例：

`<meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699">`

`<meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable">`

すべての属性の例：

この例は、CSS で要素を ID で表示／非表示にする CSS 表示プロパティの値を「block」または「none」に設定して、ブール変数が CSS 要素の表示／非表示を制御する一般的な使用例を示しています。ランディングページエディターでは、「オフ」／「オン」の代わりに、「表示」／「非表示」という表示名が使用されます。

`<meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable" default="true" true_value="block" false_value="none" false_value_name="Hide" true_value_name="Show"> <style> #myConditionalDisplayArea { display: ${boolean1}; } </style>`

>[!NOTE]
>
>プログラムトークン（my.token）は、ガイド付きまたはフリーフォームのランディングページの任意の場所で使用することもできます。
