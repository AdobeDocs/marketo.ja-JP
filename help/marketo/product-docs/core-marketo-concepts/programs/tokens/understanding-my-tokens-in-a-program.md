---
unique-page-id: 1147114
description: プログラム内のマイトークンについて — Marketto Docs — 製品ドキュメント
title: プログラム内のマイトークンについて
translation-type: tm+mt
source-git-commit: d78ecbec87d69cde66b583d21d7e0c95539bb6ec
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---


# プログラム{#understanding-my-tokens-in-a-program}内のマイトークンについて

トークンは、電子メール、ランディングページ、スマートキャンペーンで使用できる変数で、生活を容易にします。

「マイトークン」に加えて、プログラムに組み込みの任意のトークンを使用することもできます。 [トークンの概要](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md)を調べます。

## マイトークン{#my-tokens}

マイトークンは、誰でも作成できるカスタム変数です。 これらは、キャンペーンーフォルダーまたはプログラムーの[作成](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md)されます。

マイトークンは次のように表示されます。`{{my.Name Of Token}}`

例：

* `{{my.Event Date}}`
* `{{my.Webinar Speaker}}`

<table> 
 <thead> 
  <tr> 
   <th>トークンタイプ</th> 
   <th>説明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>カレンダーファイル <img alt="—" src="assets/image2014-9-25-16-3a44-3a19.png" data-linked-resource-id="3083230" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>このトークンを使用して、電子メールやランディングページにカレンダーイベントファイル(.i<a href="../../../../product-docs/email-marketing/general/functions-in-the-editor/create-a-calendar-event-ics-file.md"></a>cs)<a href="../../../../product-docs/email-marketing/general/functions-in-the-editor/create-a-calendar-event-ics-file.md">を追加します。</a></td> 
  </tr> 
  <tr> 
   <td><p>日付 <img alt="—" src="assets/image2014-9-25-16-3a44-3a47.png" data-linked-resource-id="3083231" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></p></td> 
   <td>このトークンは日付値を保持します。 日付は、年 — 月 — 日（例： 2016-05-23）として表示されます。</td> 
  </tr> 
  <tr> 
   <td>電子メールスクリプト <img alt="—" src="assets/image2014-9-25-16-3a45-3a4.png" data-linked-resource-id="3083232" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>このトークンを使用して、電子メールでVelocityスクリプトを実行します。 詳細<a href="http://developers.marketo.com/documentation/email-scripting/" title="リンク先を表示" rel="nofollow">こちら</a>。 </td> 
  </tr> 
  <tr> 
   <td>数値<span> <img alt="—" src="assets/image2014-9-25-16-3a45-3a25.png" data-linked-resource-id="3083233" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></span></td> 
   <td>任意の整数。 否定的にもなる。</td> 
  </tr> 
  <tr> 
   <td>リッチテキスト <img alt="—" src="assets/image2014-9-25-16-3a46-3a22.png" data-linked-resource-id="3083234" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>これはHTMLです。 電子メールやランディングページで使用します。</td> 
  </tr> 
  <tr> 
   <td>スコア <img alt="—" src="assets/image2014-9-25-16-3a46-3a39.png" data-linked-resource-id="3083235" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>このトークンは、<a href="../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md">変更スコアフロー手順</a>で使用します。 </td> 
  </tr> 
  <tr> 
   <td colspan="1">SFDCキャンペーン <img alt="—" src="assets/sfdc-campaign-icon.jpg" data-linked-resource-id="11379761" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114" title="—"></td> 
   <td colspan="1">このトークンを使用すると、Marketorプログラムの一部となるリードも、SFDCキャンペーンが追加されたリードに追加できます。</td> 
  </tr> 
  <tr> 
   <td>テキスト <img alt="—" src="assets/image2014-9-25-16-3a46-3a54.png" data-linked-resource-id="3083236" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>ただのテキスト。 HTMLが過剰殺しの場合に使用します。 テキストトークンのサイズ制限は、524,288文字(UTF-8)または2 MBです。</td> 
  </tr> 
 </tbody> 
</table>

>[!CAUTION]
>
>Microsoft DynamicsまたはSalesforceのSales Insightから電子メールを送信すると、マイトークンが解決しません。標準のトークンのみが設定されます(リード、会社など)。 ただし、トークン&#x200B;*のデフォルト値は*&#x200B;機能します。

## トークンのネスト{#nesting-tokens}

新しいトークンを作成すると、ツリー内の他のオブジェクトから参照できます。 管理を容易にするためにトークンが作成された場所の命名構造があります。

* **ローカルトークン：** トークンは、そのプログラムーまたはフォルダーに直接作成されました。
* **継承トークン：ト** ークンは、ツリーの上位レベルのプログラムーまたはフォルダーに作成されました。
* **上書きされたトークン：ト** ークンが継承され、その後、誰かがこのプログラムーまたはフォルダーで例外を作成しました。

グローバル変数を作成し、ツリー内の下位レベルでそれらを上書きできます。

プログラムやフォルダの移動は、トークンにも影響します。 移動中に参照が壊れていないことを必ず確認してください。

>[!NOTE]
>
>エンゲージメントプログラムから送信した電子メールが、(エンゲージメントプログラムのローカルではなく)デフォルトのプログラムの子電子メールである場合、電子メールで使用されるマイトークンは、その子電子メールが存在するデフォルトのプログラムから解決されます。

>[!MORELIKETHIS]
>
>* [トークンの概要](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md)
>* [マイトークンの管理](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md)

