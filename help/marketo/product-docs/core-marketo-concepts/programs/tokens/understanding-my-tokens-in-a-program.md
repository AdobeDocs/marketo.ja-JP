---
unique-page-id: 1147114
description: プログラムのマイトークンについて説明します。 トークンを使用して、プログラムまたはメンバーのデータでコンテンツをパーソナライズします。
title: プログラム内のマイトークンについて
exl-id: 01b42272-c419-4cd5-ad30-87413ceb2032
feature: Tokens
TQID: 'https://experienceleague.adobe.com/UYz7UtSHFbDdslMLdaGmIbdaHKedxjAhU-K8RhkgmS4'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
    internal-label: Smart Campaigns
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
    internal-label: Programs
  - id: a6d52c76-712f-5f64-a879-9c65c1499322
    internal-label: Tokens
subfeature_v2:
  - id: ad89fb33-8541-4339-afe7-bb13d1633714
    internal-label: Flow Step
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '441'
ht-degree: 93%
---
# プログラム内のマイトークンについて {#understanding-my-tokens-in-a-program}

トークンは、メール、ランディングページ、スマートキャンペーンで使用する変数で、これにより作業が手軽になります。

マイトークンに加えて、プログラム内で任意のビルトイントークンを使用することもできます。 [ トークンの概要](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md){target="_blank"}を参照してください。

## マイトークン  {#my-tokens}

マイトークンは、誰でも作成できるカスタム変数です。 ローカルでは、これらは、キャンペーンフォルダーまたはプログラム内で[作成](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md){target="_blank"}されます。

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
   <td>このトークンは日付値を保持します。 日付は、年 - 月 - 日（例：2016-05-23）と表示されます。</td>
  </tr>
  <tr>
   <td>メールスクリプト <img alt="--" src="assets/image2014-9-25-16-3a45-3a4.png" data-linked-resource-id="3083232" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td>
   <td>このトークンを使用すると、メール内で Velocity スクリプトを実行できます。 詳細は<a href="https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/email-scripting" title="リンク先" rel="nofollow">こちら</a>を参照してください。 </td>
  </tr>
  <tr>
   <td>数字<span> <img alt="--" src="assets/image2014-9-25-16-3a45-3a25.png" data-linked-resource-id="3083233" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></span></td>
   <td>任意の整数。 マイナスになることもあります。</td>
  </tr>
  <tr>
   <td>リッチテキスト <img alt="--" src="assets/image2014-9-25-16-3a46-3a22.png" data-linked-resource-id="3083234" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td>
   <td>これは HTML です。 メールとランディングページで使用します。</td>
  </tr>
  <tr>
   <td>スコア <img alt="--" src="assets/image2014-9-25-16-3a46-3a39.png" data-linked-resource-id="3083235" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td>
   <td>このトークンを、<a href="/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md">スコアの変更フローステップ</a>で使用します。 </td>
  </tr>
  <tr>
   <td colspan="1">SFDC キャンペーン <img alt="--" src="assets/sfdc-campaign-icon.jpg" data-linked-resource-id="11379761" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114" title="--"></td>
   <td colspan="1">このトークンを使用すると、Marketo プログラムの一部となったリードを、指定された SFDC キャンペーンにも追加できます。</td>
  </tr>
  <tr>
   <td>テキスト <img alt="--" src="assets/image2014-9-25-16-3a46-3a54.png" data-linked-resource-id="3083236" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td>
   <td>テキストです。 HTML が過剰な場合に使用します。 テキストトークンのサイズ制限は 524,288 文字（UTF-8）または 2 MB です。</td>
  </tr>
 </tbody>
</table>

>[!CAUTION]
>
>[!DNL Microsoft Dynamics] または [!DNL Salesforce] のセールスインサイトからメールを送信しても、マイトークンは解決されません。標準のトークン（リード、会社など）のみが入力されます。 ただし、トークンのデフォルト値は&#x200B;_機能します_。

## トークンのネスト {#nesting-tokens}

新しいトークンを作成すると、そのトークンをツリー内の他のオブジェクトで参照できます。 管理を容易にするために、トークンがどこで作成されたかに基づく命名構造が用意されています。

* **ローカルトークン：**&#x200B;そのプログラムまたはフォルダーで適切に作成されたトークン。
* **継承されたトークン：**&#x200B;ツリーの上位のプログラムまたはフォルダーの任意の場所に作成されたトークン。
* **上書きされたトークン：**&#x200B;継承された後に、このプログラムまたはフォルダーでは例外とされたトークン。

グローバル変数を作成して、ツリーの下位レベルで上書きできます。

プログラムやフォルダーの移動はトークンにも影響を与えます。 移動するときに参照が壊れていないことを必ず確認してください。

>[!IMPORTANT]
>
>ネストされたトークンは、[ バッチキャンペーン ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/understanding-batch-and-trigger-smart-campaigns.md#batch-campaign){target="_blank"}ではサポートされていません。

>[!NOTE]
>
>エンゲージメントプログラムから送信したメールがデフォルトプログラムの子メールの場合（エンゲージメントプログラムのローカルメールではない場合）、メールで使用されるマイトークンは、その子メールが存在するデフォルトプログラムから参照されます。

>[!MORELIKETHIS]
>
>* [トークンの概要](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md){target="_blank"}
>* [マイトークンの管理](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md){target="_blank"}
