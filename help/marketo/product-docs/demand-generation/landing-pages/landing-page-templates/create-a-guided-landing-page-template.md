---
unique-page-id: 7515401
description: ガイド付きランディングページテンプレートの作成 — Marketto Docs — 製品ドキュメント
title: ガイド付きランディングページテンプレートの作成
translation-type: tm+mt
source-git-commit: 2969e6f94f5fd781e2167ae2aa8680bb8d134754
workflow-type: tm+mt
source-wordcount: '1269'
ht-degree: 0%

---


# ガイド付きランディングページテンプレートの作成{#create-a-guided-landing-page-template}

>[!NOTE]
>
>読書に飽きた？ [操作手順を順を追って、このクールな](https://youtu.be/3O7e4GdZKsM) ビデオをご覧ください。

ガイド付きランディングページテンプレートには、特別な構文があります。 この構文を使用して、カスタマイズ可能なコンテンツと、テンプレートから作成された各ランディングページ上のコンテンツの最終的な位置を指定します。 編集可能として指定した領域または変数のみが、「ガイド付き」ランディングページエディター内でカスタマイズできます。

>[!TIP]
>
>適切な命名規則を使用すると、マーケティングチームがあなたを好きになります。

ページ上の任意の要素を編集可能にする方法は2つあります。

* オブジェクトを「要素」として宣言します。 ランディングページの作成者は、画像、テキストまたはマーケティング用のアセットを指定された地域に追加できます。
* 文字列を「変数」として宣言します。 ランディングページの作成者は、true/falseレバーからの文字列、色、またはブール値の状態に変数を置き換えることができます。

## 編集可能な要素{#editable-elements}

要素は、通常のDOM要素をテンプレートに追加し、その後、Marketor固有のクラス名で要素を装飾することで宣言されます。

## テキスト{#text}

地域をリッチテキストと定義すると、ユーザーは、マーケティング担当者のリッチテキストエディター](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md)を使用して、そのコンテンツを[編集できます。

必須属性：\
**class**:&quot;mktoText&quot;\
**id**:ID文字列。文字、数字、ダッシュ「 — 」、下線「_」のみが含まれます。 スペースは使用できません。 一意である必要があります。\
**mktoName** :文字列。これは、ランディングページエディターに表示される表示名です。 ベストプラクティスは、わかりやすい名前を使用することです。

オプション：\
mktoTextクラスを持つ要素のコンテンツ（指定されている場合）は、編集可能領域のデフォルト値として使用されます。

例：

`<pre data-theme="Confluence"><div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area.</div></pre>`

### 画像{#image}

編集可能な画像要素を定義するオプションは2つあります。 `<div>`(イメージを挿入するコンテナを指定)または`<img>`タグを使用できます。

## オプション1 - `<div>` {#option-use-a-div}を使用

必須属性：

クラス：&quot;mktoImg&quot;\
id:ID文字列。 文字、数字、ダッシュ「 — 」、下線「_」のみが含まれます。 スペースは使用できません。 一意である必要があります。\
mktoName :文字列。 これは、ランディングページエディターに表示される表示名です。 ベストプラクティスは、わかりやすい名前を使用することです。

オプション：\
mktoImgClass:文字列。 ここでの値は、div内の`<img>`要素のclass属性に追加されます。

例：

`<pre data-theme="Confluence"><div class="mktoImg" id="exampleImg" mktoName="Example Image"></div></pre>`

## オプション2 - `<img>` {#option-use-a-img}を使用

必須属性：\
クラス：&quot;mktoImg&quot;\
id:ID文字列。 文字、数字、ダッシュ「 — 」、下線「_」のみが含まれます。 スペースは使用できません。 一意である必要があります。\
mktoName :文字列。 これは、ランディングページエディターに表示される表示名です。 ベストプラクティスは、わかりやすい名前を使用することです。

オプション：\
src:文字列URL これは、画像のデフォルト値として使用されます。

例：

`<pre data-theme="Confluence"><img class="mktoImg" id="exampleImg" mktoName="Example Image"></pre>`

>[!NOTE]
>
>`<img>`バージョンを使用する場合、レンダリングされたHTMLには、生成されたdivラッパーが`<img>`タグの周りに含まれます。 クラスに設定されます。」mktoImg.mktoGen,&quot;と指定し、display:inline-blockにします。

## フォーム{#form}

例：必須属性：\
**class**:&quot;mktoForm&quot;\
**id**:ID文字列。文字、数字、ダッシュ「 — 」、下線「_」のみが含まれます。 スペースは使用できません。 一意である必要があります。\
**mktoName** :文字列。これは、ランディングページエディターに表示される表示名です。 ベストプラクティスは、わかりやすい名前を使用することです。

`<pre data-theme="Confluence"><div class="mktoForm" id="exampleForm" mktoName="Example Form"></div></pre>`

## スニペット{#snippet}

必須属性：\
**class**:&quot;mktoSnippet&quot;\
**id**:ID文字列。文字、数字、ダッシュ「 — 」、下線「_」のみが含まれます。 スペースは使用できません。 一意である必要があります。\
**mktoName** :文字列。これは、ランディングページエディターに表示される表示名です。 ベストプラクティスは、わかりやすい名前を使用することです。

例：

`<pre data-theme="Confluence"><div class="mktoSnippet" id="exampleSnippet" mktoName="Example Snippet"></div></pre>`

## 共有ボタン{#share-button}

必須属性：\
**class**:&quot;mktoShareButton&quot;\
**id**:ID文字列。文字、数字、ダッシュ「 — 」、下線「_」のみが含まれます。 スペースは使用できません。 一意である必要があります。\
**mktoName** :文字列。これは、ランディングページエディターに表示される表示名です。 ベストプラクティスは、わかりやすい名前を使用することです。

例：

`<pre data-theme="Confluence"><div class="mktoShareButton" id="exampleShareButton" mktoName="Example Share Button"></div></pre>`

## ビデオ{#video}

>[!NOTE]
>
>ランディングページでビデオ要素を使用する場合、MarketoはYouTubeのビデオのみをサポートします。 別のサービスを使用する場合は、リッチテキストボックスを使用し、ビデオの埋め込みコードに貼り付けることをお勧めします。

必須属性：
**クラス**:&quot;mktoVideo&quot;
**id**:ID文字列。 文字、数字、ダッシュ「 — 」、下線「_」のみが含まれます。 スペースは使用できません。 一意である必要があります。
**mktoName** :文字列。これは、ランディングページエディターに表示される表示名です。 ベストプラクティスは、わかりやすい名前を使用することです。

例：

`<pre data-theme="Confluence"><div class="mktoVideo" id="exampleVideo" mktoName="Example Video"></div></pre>`

## 投票{#poll}

必須属性：\
**class**:&quot;mktoPoll&quot;\
**id**:ID文字列。文字、数字、ダッシュ「 — 」、下線「_」のみが含まれます。 スペースは使用できません。 一意である必要があります。\
**mktoName** :文字列。これは、ランディングページエディターに表示される表示名です。 ベストプラクティスは、わかりやすい名前を使用することです。

例：

`<pre data-theme="Confluence"><div class="mktoPoll" id="examplePoll" mktoName="Example Poll"></div></pre>`

## 照会{#referral}

必須属性：\
**class**:&quot;mktoReferral&quot;\
**id**:ID文字列。文字、数字、ダッシュ「 — 」、下線「_」のみが含まれます。 スペースは使用できません。 一意である必要があります。\
**mktoName** :文字列。これは、ランディングページエディターに表示される表示名です。 ベストプラクティスは、わかりやすい名前を使用することです。

例：

`<pre data-theme="Confluence"><div class="mktoReferral" id="exampleReferral" mktoName="Example Referral"></div></pre>`

## 懸賞{#sweepstakes}

必須属性：\
**class**:&quot;mktoSweepstakes&quot;\
**id**:ID文字列。文字、数字、ダッシュ「 — 」、下線「_」のみが含まれます。 スペースは使用できません。 一意である必要があります。\
**mktoName** :文字列。これは、ランディングページエディターに表示される表示名です。 ベストプラクティスは、わかりやすい名前を使用することです。

例：

`<pre data-theme="Confluence"><div class="mktoSweepstakes" id="exampleSweepstakes" mktoName="Example Sweepstakes"></div></pre>`

## 編集可能な変数{#editable-variables}

すべての変数型は、${ }の文字シーケンス内に含まれるid属性の値を参照することで使用されます。 変数は、他の変数宣言内を除き、ドキュメント内の任意の場所で使用できます。

例：

`<pre data-theme="Confluence">${var1}</pre>`

**宣言：**

変数は、テンプレートの`<head>`要素内でmetaタグとして宣言されます。 3種類の変数を使用できます。文字列、色、およびブール値。

## 文字列{#string}

必須属性：\
**class** :&quot;mktoString&quot;,\
**id**:ID文字列。文字、数字、ダッシュ「 — 」、下線「_」のみが含まれます。 スペースは使用できません。 一意である必要があります。\
**mktoName** :文字列。これは、ランディングページエディターに表示される表示名です。 ベストプラクティスは、わかりやすい名前を使用することです。

オプション：\
**default**:属性の文字列値。何も指定しない場合は空白です。\
**allowHtml**:&quot;true&quot;または&quot;false&quot;。値をHTMLエスケープせずに出力するかどうかを制御します。 デフォルトは、設定されていない場合は「false」です。

基本的な例：

`<pre data-theme="Confluence"><meta class="mktoString" id="var1" mktoName="My Variable"></pre>`

すべての属性を持つ例：

`<pre data-theme="Confluence"><meta class="mktoString" id="var1" mktoName="My Variable" default="This is my default value" allowHtml="true"></pre>`

## 色{#color}

必須属性：\
**class** :&quot;mktoColor&quot;,\
**id**:ID文字列。文字、数字、ダッシュ「 — 」、下線「_」のみが含まれます。 スペースは使用できません。 一意である必要があります。\
**mktoName** :文字列。これは、ランディングページエディターに表示される表示名です。 ベストプラクティスは、わかりやすい名前を使用することです。

オプション：\
**default**:7桁の16進数文字のカラーコードです。例：&quot;#336699&quot;

基本的な例：

`<pre data-theme="Confluence"><meta class="mktoColor" id="color1" mktoName="My Color Variable"></pre>`

すべての属性を持つ例：

`<pre data-theme="Confluence"><meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699"></pre>`

## ブール値{#boolean}

必須属性：\
**class** :&quot;mktoBoolean&quot;,\
**id**:ID文字列。文字、数字、ダッシュ「 — 」、下線「_」のみが含まれます。 スペースは使用できません。 一意である必要があります。\
**mktoName** :文字列。これは、ランディングページエディターに表示される表示名です。 ベストプラクティスは、わかりやすい名前を使用することです。

オプション：\
**default**:ブール文字列。&quot;true&quot;または&quot;false&quot;は、値の開始がオンまたはオフの位置にあるかどうかを制御します。 指定されない場合は「false」。\
**false_value**:文字列。変数がオフの位置にあるときに変数に挿入する値です。 指定されない場合は「false」。\
**true_value**:文字列。変数がオンの位置にあるときに変数に挿入される値です。 指定されない場合は「true」。\
**false_value_name**:文字列。値がOFF位置にある場合にランディングページエディタに表示される表示名です。 「OFF」（指定されない場合）。\
**true_value_name**:文字列。値がON位置にある場合にランディングページエディターに表示される表示名です。 「ON」（指定されない場合）。

基本的な例：

`<pre data-theme="Confluence"><meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699"></pre>`

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable"></pre>`

すべての属性を持つ例：

この例は、boolean変数がcss要素の表示を制御する一般的な使用例です。css表示プロパティの値を「block」または「none」に設定し、CSSで要素をIDで表示/非表示にします。 ランディングページエディタは、OFF/ONではなく、表示/非表示という表示名を使用します。

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable" default="true" true_value="block" false_value="none" false_value_name="Hide" true_value_name="Show"> <style> #myConditionalDisplayArea { display: ${boolean1}; } </style></pre>`

>[!NOTE]
>
>プログラムトークン(my.token)は、ガイド付きランディングページやフリーフォームイベントのどこでも使用できます。
