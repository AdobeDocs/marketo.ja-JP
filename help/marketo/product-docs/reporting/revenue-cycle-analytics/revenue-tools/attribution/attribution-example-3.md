---
unique-page-id: 7514149
description: Marketo Engageのアトリビューション例3の詳細（アトリビューション例3のアトリビューション例を含む）を説明します。 このガイドを使用して、次のステップを完了してください。
title: アトリビューションの例 3
exl-id: d8ca63a2-58de-4cde-b915-ff7f2e6468d9
feature: Reporting, Revenue Cycle Analytics
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
    internal-label: Reporting
  - id: 126e34f9-e02a-505e-9978-ea36537f3ef9
    internal-label: Revenue Cycle Analytics
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 88%
---
# アトリビューションの例 3 {#attribution-example}

次のシナリオを読み、グリッドに表示する数値を決定してみてください。

* 4 月 11 日 | Steve がダウンロード（コンテンツ） — 成功
* 4月22日 | $3,000 の商談が作成される（Steve と Jason の両方がロールを持つ）
* 4 月 25 日｜Jason が（ウェビナー）に参加する - 成功
* 4月30日｜商談がクローズ（成約）になる

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
>アトリビューションルール #3 を思い出してください。 Jason は、商談が作成された後にプログラムで成功ステータスになりました。 したがって、ウェビナーは商談の作成に対するクレジットを得ることはできません。 そのため、獲得した商談に対するクレジットだけが付与されます。
>
>したがって、（コンテンツ）は商談の作成およびパイプラインに対するクレジットの 100% を獲得しますが、獲得した商談に対するクレジットは 50% のみを獲得します。

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
