---
unique-page-id: 7514146
description: アトリビューションの例 2 - Marketo ドキュメント - 製品ドキュメント
title: アトリビューションの例 2
exl-id: 8f00abb5-85f8-4f05-874e-57aa6442548c
source-git-commit: ''
workflow-type: ht
source-wordcount: '162'
ht-degree: 100%

---

# アトリビューションの例 2 {#attribution-example}

次のシナリオを読み、グリッドに表示する数値を決定してみてください。

* 4月11日｜Bill が（展示会）によって獲得される
* 4月15日｜Joan が（ウェビナー）によって獲得される
* 4月22日｜6,000 ドルで（商談 1）が作成される
* 4月24日｜10,000 ドルで（商談 2）が作成される
* 4月25日｜Bill と Joan が&#x200B;**両方**&#x200B;の商談の役割に関連付けられる
* 4月29日｜（商談 1）が成立してクローズされる

| プログラム名 | （展示会） | （ウェビナー） |
|---|---|---|
| （FT）創出された商談 | `<pre>1</pre>` | `<pre>1</pre>` |
| （FT）創出されたパイプライン | `<pre>$8,000</pre>` | `<pre>$8,000</pre>` |
| （FT）成立した商談 | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| （FT）獲得した売上高 | `<pre>$3,000</pre>` | `<pre>$3,000</pre>` |

**回答を表示**

>[!NOTE]
>
>**説明**
>
>Bill と Joan が 2 人とも&#x200B;**両方**&#x200B;の商談の役割に関連付けられていたので、システムは（ルールに従って）クレジットを均等に分割します。
>
>各プログラム（8,000 ドル）に対して作成されたパイプラインは、クレジットとして与えられる合計（16,000 ドル）の半分です。

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
>* [アトリビューションの例 3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)
>* [アトリビューションの例 4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)

