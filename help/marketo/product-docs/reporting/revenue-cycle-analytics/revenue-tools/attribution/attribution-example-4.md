---
unique-page-id: 7514151
description: アトリビューションの例 4 - Marketo ドキュメント - 製品ドキュメント
title: アトリビューションの例 4
exl-id: 98cd7401-3bc7-40a1-b88d-7174a3027d4e
source-git-commit: ''
workflow-type: ht
source-wordcount: '181'
ht-degree: 100%

---

# アトリビューションの例 4 {#attribution-example}

次のシナリオを読み、グリッドに表示する数値を決定してみてください。

* 4月11日｜Michelle が eBook（コンテンツ）をダウンロードする - 成功
* 4月15日｜John が（ウェビナー）に参加する - 成功
* 4月22日｜3,000 ドルで（商談 1）が作成される
* 4月24日｜5,000 ドルで（商談 2）が作成される
* 4月25日｜John と Michelle が&#x200B;**両方**&#x200B;の商談に関連付けられる
* 4月29日｜[商談 1] が成立してクローズされる

| プログラム名 | （コンテンツ） | （ウェビナー） |
|---|---|---|
|  | （商談 1） | （商談 2） | （商談 1） | （商談 2） |
| （MT）創出された商談 | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| （MT）創出されたパイプライン | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` |
| （MT）成立した商談 | `<pre>0.5</pre>` | `<pre>0</pre>` | `<pre>0.5</pre>` | `<pre>0</pre>` |
| （MT）獲得した売上高 | `<pre>$1,500</pre>` | `<pre>$0</pre>` | `<pre>$1,500</pre>` | `<pre>$0</pre>` |

**回答を表示**

>[!NOTE]
>
>**説明**
>
>複数の商談があり、複数の人がプログラムを成功させた場合、人とプログラムの間でクレジットを分割する必要があります。ただし、商談 1 と商談 2 のクレジットは組み合わされません。それぞれが個別のクレジット評価です。
>
>多くの人々が関わると、Marketo は自動的にクレジットを与える商談の端数を計算します。

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

