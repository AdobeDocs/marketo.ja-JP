---
unique-page-id: 7514146
description: Marketo Engageのアトリビューション例2の詳細（アトリビューション例2 アトリビューション例を含む）を説明します。 このガイドを使用して、次のステップを完了してください。
title: アトリビューションの例 2
exl-id: 8f00abb5-85f8-4f05-874e-57aa6442548c
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
source-wordcount: '197'
ht-degree: 88%
---
# アトリビューションの例 2 {#attribution-example}

次のシナリオを読み、グリッドに表示する数値を決定してみてください。

* 4月11日｜Bill を（展示会）で獲得
* 4月15日｜Joan を（ウェビナー）で獲得
* 4月22日｜6,000 ドルの（商談 1）を作成
* 4月24日｜10,000 ドルの（商談 2）を作成
* 4 月 25 日｜Bill と Joan が&#x200B;**両方**&#x200B;の商談の役割に関連付けられる
* 4月29日｜（商談 1）がクローズ（成約）

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
>各プログラムのパイプライン（8,000 ドル）は、クレジットとして付与できる合計額（16,000 ドル）の半分です。

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
