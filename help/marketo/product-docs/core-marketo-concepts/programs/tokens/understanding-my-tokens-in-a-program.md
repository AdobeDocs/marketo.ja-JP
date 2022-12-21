---
unique-page-id: 1147114
description: プログラム内のマイトークンの理解 - Marketo ドキュメント - 製品ドキュメント
title: プログラム内のマイトークンの理解
exl-id: 01b42272-c419-4cd5-ad30-87413ceb2032
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 100%

---

# プログラム内のマイトークンの理解 {#understanding-my-tokens-in-a-program}

トークンは、メール、ランディングページ、スマートキャンペーンで使用する変数で、これにより作業が手軽になります。

マイトークンに加えて、プログラムに組み込まれた任意のトークンを使用することもできます。詳しくは、[トークンの概要](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md)を参照してください

## マイトークン  {#my-tokens}

マイトークンは、誰でも作成できるカスタム変数です。これらは、キャンペーンフォルダーまたはプログラム内で[作成](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md)されます。

マイトークンは次のように表示されます。`{{my.Name Of Token}}`

例：

* `{{my.Event Date}}`
* `{{my.Webinar Speaker}}`

<table> 
 <thead> 
  <tr> 
   <th>トークンのタイプ</th> 
   <th>説明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>カレンダーファイル <img alt="--" src="assets/image2014-9-25-16-3a44-3a19.png" data-linked-resource-id="3083230" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>このトークンを使用して、<a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/create-a-calendar-event-ics-file.md">カレンダーイベントファイル（.i</a><a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/create-a-calendar-event-ics-file.md">cs）</a>をメールとランディングページに追加します。</td> 
  </tr> 
  <tr> 
   <td><p>日 <img alt="--" src="assets/image2014-9-25-16-3a44-3a47.png" data-linked-resource-id="3083231" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></p></td> 
   <td>このトークンは日付値を保持します。日付は、年 - 月 - 日（例：2016-05-23）と表示されます。</td> 
  </tr> 
  <tr> 
   <td>メールスクリプト <img alt="--" src="assets/image2014-9-25-16-3a45-3a4.png" data-linked-resource-id="3083232" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>このトークンを使用して、メールで Velocity スクリプトを実行します。詳細は<a href="https://developers.marketo.com/documentation/email-scripting/" title="リンク先" rel="nofollow">こちら</a>を参照してください。 </td> 
  </tr> 
  <tr> 
   <td>数字<span> <img alt="--" src="assets/image2014-9-25-16-3a45-3a25.png" data-linked-resource-id="3083233" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></span></td> 
   <td>任意の整数。マイナスになることもあります。</td> 
  </tr> 
  <tr> 
   <td>リッチテキスト <img alt="--" src="assets/image2014-9-25-16-3a46-3a22.png" data-linked-resource-id="3083234" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>これは HTML です。メールとランディングページで使用します。</td> 
  </tr> 
  <tr> 
   <td>スコア <img alt="--" src="assets/image2014-9-25-16-3a46-3a39.png" data-linked-resource-id="3083235" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>このトークンを、<a href="/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md">スコアの変更フローステップ</a>で使用します。 </td> 
  </tr> 
  <tr> 
   <td colspan="1">SFDC キャンペーン <img alt="--" src="assets/sfdc-campaign-icon.jpg" data-linked-resource-id="11379761" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114" title="--"></td> 
   <td colspan="1">このトークンを使用すると、Marketo プログラムの一部となるリードを、SFDC キャンペーンが追加されているすべてのリードにも追加できます。</td> 
  </tr> 
  <tr> 
   <td>テキスト <img alt="--" src="assets/image2014-9-25-16-3a46-3a54.png" data-linked-resource-id="3083236" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>テキストです。HTML が過剰な場合に使用します。テキストトークンのサイズ制限は 524,288 文字（UTF-8）または 2 MB です。</td> 
  </tr> 
 </tbody> 
</table>

>[!CAUTION]
>
>Microsoft Dynamics または Salesforce の Sales Insight からメールを送信しても、マイトークンは解決されません。標準のトークン（リード、会社など）のみが入力されます。ただし、トークンのデフォルト値は&#x200B;_機能します_。

## トークンのネスト {#nesting-tokens}

新しいトークンを作成すると、そのトークンをツリー内の他のオブジェクトで参照できます。管理を容易にするために、トークンが作成された場所に命名構造があります。

* **ローカルトークン：**&#x200B;そのプログラムまたはフォルダーで適切に作成されたトークン。
* **継承されたトークン：**&#x200B;ツリーの上位のプログラムまたはフォルダーの任意の場所に作成されたトークン。
* **上書きされたトークン：**&#x200B;継承された後に、このプログラムまたはフォルダーでは例外とされたトークン。

グローバル変数を作成して、ツリーの下位レベルで上書きできます。

プログラムやフォルダーの移動はトークンにも影響を与えます。移動するときに参照が壊れていないことを必ず確認してください。

>[!NOTE]
>
>エンゲージメントプログラムから送信したメールが、デフォルトプログラムの子メールの場合（エンゲージメントプログラムのローカルメールではない場合）、メールで使用されるマイトークンは、子メールが存在するデフォルトプログラムから解決されます。

>[!MORELIKETHIS]
>
>* [トークンの概要](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md)
>* [マイトークンの管理](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md)

