---
unique-page-id: 7504676
description: 期間原価について - Marketo ドキュメント - 製品ドキュメント
title: 期間原価について
exl-id: 99f50eaf-28cf-4a8b-8ebd-89a4beef986a
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 100%

---

# 期間原価について {#understanding-period-costs}

## 概要 {#overview}

期間原価とは、ある特定の月にプログラムのために費やしたコストのことです。

>[!NOTE]
>
>**例**
>
>7 月に公開する eBook 用のイラストレーターに 1000 ドルを支払ったとします。この場合、この eBook プログラムの 7 月の期間原価は 1000 ドルとなります。
>
>また Google Adwords に 1 か月 200 ドルを費やしている場合、この Google Adwords プログラムの期間原価は&#x200B;**毎月** 200 ドルです。

>[!NOTE]
>
>[プログラムについて](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)
>
>[プログラムメンバーシップについて](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)

## 期間原価の計算方法 {#how-period-costs-are-calculated}

ここでは 3 月に開催されるウェビナーを例に考えてみましょう。新規リードは事前の 1 月と 2 月の宣伝によって獲得されます。またイベント後の 4 月と 5 月にも、ウェビナーのダウンロードを通じて新規連絡先が獲得されます。

1. 期間原価を 3 月の 1 期間に計上した場合…

   ![](assets/graph1.png)

   …その前と後の月に獲得された連絡先&#x200B;*のみ*&#x200B;が 3 月分に計上されます。

   ![](assets/graph2.png)

1. 1 月、2 月、3 月に期間原価を計上した場合…

   ![](assets/graph3.png)

   …3 月以降に獲得された連絡先のみが 3 月分に計上されます。

   ![](assets/graph4.png)

1. 1 月と 4 月に期間原価を計上した場合…

   ![](assets/graph5.png)

   ...1 月から 3 月に追加された連絡先は、1 月分に計上されます。…4 月と 5 月に追加した連絡先は、4 月分に計上されます。

   ![](assets/graph6.png)

   >[!NOTE]
   >
   >まとめ：期間原価のない月分は、期間原価の計上された直前の月にさかのぼって計上されます。もしそれ以前に期間原価のある月が存在しなければ、その月以降で最初に期間原価が計上された月に繰り越して計上されます。期間原価が&#x200B;_どの_&#x200B;月にも計上されていない場合、そのプログラムの RCE レポートは利用できません。

   >[!MORELIKETHIS]
   >
   >* [プログラムでの期間原価の使用](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/using-period-costs-in-a-program.md)
   >* [プログラムレポートを期間原価でフィルター](/help/marketo/product-docs/core-marketo-concepts/programs/program-performance-report/filter-a-program-report-by-period-cost.md)

