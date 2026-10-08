---
unique-page-id: 7514151
description: Marketo Engageのアトリビューション例4について説明します。アトリビューション例4のアトリビューション例も含まれます。 このガイドを使用して、次のステップを完了してください。
title: アトリビューションの例 4
exl-id: 98cd7401-3bc7-40a1-b88d-7174a3027d4e
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
source-wordcount: '221'
ht-degree: 90%
---
# アトリビューションの例 4 {#attribution-example}

次のシナリオを読み、グリッドに表示する数値を決定してみてください。

* 4月11日｜Michelle が eBook（コンテンツ）をダウンロード - 成功
* 4月15日｜John が（ウェビナー）に参加 - 成功
* 4月22日｜3,000 ドルで（商談 1）が作成
* 4 月 24 日｜5,000 ドルで（商談 2）が作成される
* 4 月 25 日｜John と Michelle が&#x200B;**両方**&#x200B;の商談に関連付けられる
* 4 月 29 日｜[商談 1] が成立してクローズされる

| プログラム名 | （コンテンツ） | （ウェビナー） | | |
|---|---|---|---|---|
|   | （商談 1） | （商談 2） | （商談 1） | （商談 2） |
| （MT）創出された商談 | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| （MT）創出されたパイプライン | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` |
| （MT）成立した商談 | `<pre>0.5</pre>` | `<pre>0</pre>` | `<pre>0.5</pre>` | `<pre>0</pre>` |
| （MT）獲得した売上高 | `<pre>$1,500</pre>` | `<pre>$0</pre>` | `<pre>$1,500</pre>` | `<pre>$0</pre>` |

**回答を表示**

>[!NOTE]
>
>**説明**
>
>複数の商談があり、複数の人がプログラムを成功させた場合、人とプログラムの間でクレジットを分割する必要があります。 ただし、商談 1 と商談 2 のクレジットは組み合わされません。 それぞれが個別のクレジット評価です。
>
>多くの人が関わる場合、Marketo は商談に対して付与されるクレジットの割合を自動的に計算します。

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
>* [アトリビューションの例 3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)
