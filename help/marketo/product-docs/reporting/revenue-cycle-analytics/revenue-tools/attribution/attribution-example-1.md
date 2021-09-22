---
unique-page-id: 7514126
description: アトリビューションの例 1 - Marketo ドキュメント - 製品ドキュメント
title: アトリビューションの例 1
exl-id: 851cbad3-0f6d-4ea0-857f-8b15337c7540
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '170'
ht-degree: 100%

---

# アトリビューションの例 1 {#attribution-example}

次のシナリオを読み、グリッドに表示する数値を決定してみてください。

* 4月11日｜Fred が（展示会）によって獲得される
* 4月15日｜Margo が（ウェビナー）に参加する - 成功
* 4月22日｜Fred が商談への（役割）に関連付けられる
* 4月22日｜3,000 ドルで商談が創出される

| プログラム名 | （展示会） | （ウェビナー） |
|---|---|---|
| （FT）創出された商談 | `<pre>1</pre>` | `<pre>0</pre>` |
| （FT）創出されたパイプライン | `<pre>$3,000</pre>` | `<pre>$0</pre>` |
| （FT）成立した商談 | `<pre>0</pre>` | `<pre>0</pre>` |
| （FT）獲得した売上高 | `<pre>0</pre>` | `<pre>0</pre>` |

**回答を表示**

>[!NOTE]
>
>**説明**
>
>まず、カウント型と通貨型があることを理解します。創出された商談はカウント（整数）です。パイプラインは通貨です。Marketo では、通貨は管理ロケールの設定に従います。
>
>展示会が全てのクレジットを受け取ったのは、Margo が商談内の役割に関連付けられていなかったからです。役割がなければ、クレジットも受け取れません。

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
>* [アトリビューションの例 2](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-2.md)
>* [アトリビューションの例 3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)
>* [アトリビューションの例 4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)

