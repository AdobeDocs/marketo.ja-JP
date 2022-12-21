---
unique-page-id: 7514149
description: アトリビューションの例 3 - Marketo ドキュメント - 製品ドキュメント
title: アトリビューションの例 3
exl-id: d8ca63a2-58de-4cde-b915-ff7f2e6468d9
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 100%

---

# アトリビューションの例 3 {#attribution-example}

次のシナリオを読み、グリッドに表示する数値を決定してみてください。

* 4 月 11 日 | Steve がダウンロード（コンテンツ） — 成功
* 4 月 23 日 | 商談は $3,000 に対して作成される（Steve と Jason の両方が役割を持つ）
* 4 月 25 日｜Jason が（ウェビナー）に参加する - 成功
* 4 月 30 日｜商談が成立してクローズされる

| 属性指標 | （コンテンツ） | （ウェビナー） |
|---|---|---|
| （MT）創出された商談 | `<pre>1</pre>` | `<pre>0</pre>` |
| （MT）創出されたパイプライン | `<pre>$3,000</pre>` | `<pre>$0</pre>` |
| （MT）成立した商談 | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| （MT）獲得した売上高 | `<pre>$1,500</pre>` | `<pre>$1,500</pre>` |

**回答を表示**

>[!NOTE]
>
>**説明**
>
>属性ルール #3 を思い出してください。Jason は、商談の作成後にプログラムを成功させました。したがって、オンラインセミナーは商談の作成に対するクレジットを受け取ることができません。受け取るのは、商談の獲得に対するクレジットのみです。
>
>したがって、（コンテンツ）は商談の作成およびパイプラインのクレジットの 100% を獲得しますが、商談のクレジットの 50% のみを獲得します。

>[!NOTE]
>
>**アトリビューションルール**
>
>1. クレジットは均等に分割される
>1. 獲得した以上のクレジットは付与できない
>1. 過去に発生したことに対してクレジットは付与できない


すべての例を試してみて、アトリビューションの達人になりましょう。

>[!MORELIKETHIS]
>
>* [アトリビューションの例 1](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-1.md)
>* [アトリビューションの例 2](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-2.md)
>* [アトリビューションの例 4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)

