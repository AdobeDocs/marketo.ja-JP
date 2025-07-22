---
unique-page-id: 2360403
description: プログラムアナライザーを使用したプログラムの効果の比較 - Marketo ドキュメント - 製品ドキュメント
title: プログラムアナライザーを使用したプログラムの効果の比較
exl-id: 6e54d0a4-3cff-46cf-be0d-1992a39d8c03
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 45%

---

# [!UICONTROL &#x200B; プログラムアナライザ &#x200B;] を使用したプログラムの有効性の比較 {#compare-program-effectiveness-with-the-program-analyzer}

[!UICONTROL &#x200B; プログラムアナライザー &#x200B;] を使用すると、プログラムのコスト、メンバーの獲得、パイプライン、収益を比較して、最も効果が高いプログラムと最も効果が低いプログラムを特定できます。

>[!PREREQUISITES]
>
>[ プログラムアナライザ [!UICONTROL &#x200B; の作成 &#x200B;]](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/create-a-program-analyzer.md)

1. 「**[!UICONTROL 分析]**」をクリックします。

   ![](assets/image2014-9-17-18-3a50-3a30.png)

1. 「プログラムアナライザー」を選択します。

   ![](assets/image2014-9-17-18-3a50-3a37.png)

1. ビューを **[!UICONTROL プログラム別]** に変更します。

   ![](assets/image2014-9-17-18-3a50-3a44.png)

1. **[!UICONTROL チャネルフィルター]** を使用すると、ビューを 1～2 つのチャネルに縮小できます。 ここでは、**[!UICONTROL Tradeshow]** チャネルのプログラムについて説明します。

   ![](assets/image2014-9-17-18-3a51-3a2.png)

   >[!TIP]
   >
   >プログラムを 1 つのチャネルに絞り込む簡単な方法は、**[!UICONTROL 表示]**／**[!UICONTROL チャネル別]**&#x200B;を選択し、そのチャネルのバブルをクリックして、ポップアップダイアログでチャネル名をクリックすることです。

1. 「**[!UICONTROL X 軸]**」ドロップダウンを使用して、横軸の指標を選択します。まず、**[!UICONTROL プログラムコスト]** から始めます。

   ![](assets/image2014-9-17-18-3a52-3a16.png)

1. **[!UICONTROL Y 軸]** ドロップダウンを使用して、垂直軸の指標を選択します。 新しいリードの獲得に優れたプログラムを見つけるには、**[!UICONTROL 新しい名前]** を選択します。

   ![](assets/image2014-9-17-18-3a52-3a26.png)

1. スライダーをオンにしてズームインします。

   ![](assets/image2014-9-17-18-3a53-3a9.png)

   >[!TIP]
   >
   >また、線形から対数スケールに変更したり、その逆に変更したりして、表示を向上させることもできます。上部の&#x200B;**[!UICONTROL 拡大・縮小]**&#x200B;メニューを使用します。

1. 結果のグラフを表示します。

   ![](assets/image2014-9-17-18-3a53-3a49.png)

   この例では、新しい名前を取り込む際に、[!DNL Origami Expo] がチャネル内の他のすべてのプログラムよりもはるかに優れており、中程度のコストで学習します。 ただし、それだけではありません。さらに 2 つの指標を追加して、より深く理解できるようにします。

1. **[!UICONTROL バブルサイズ]** ドロップダウンを使用して、バブルのサイズで比較する指標を選択します。 この例では、「**[!UICONTROL （FT） Revenue Won]**」を選択します。

   ![](assets/image2014-9-17-18-3a54-3a25.png)

   >[!NOTE]
   >
   >プログラムアナライザーで選択できる指標の多くは、ファーストタッチ（FT）計算とマルチタッチ（MT）計算で利用できます。[FT と MT のアトリビューションの違い](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md)を理解することが重要です。

1. グラフ内でバブルのサイズが変化することを確認します。

   ![](assets/image2014-9-17-18-3a54-3a57.png)

   **[!UICONTROL （FT） Revenue Won]** を追加すると、[!DNL Origami Expo] が多くの新しい名前を取得した一方で、比較的売上高が少ないことが迅速に分かります。 また、[!DNL Paper Fest 12] プログラムの名前は少なくなっていますが、より多くの売上高に影響を与えるため、より良い名前になっています（より大きなバブル）。

1. 「カラー」ドロップダウンを使用して、4 つ目の指標を追加します。**[!UICONTROL （FT）の投資収益]** を見てみよう。

   ![](assets/image2014-9-17-18-3a55-3a33.png)

1. グラフのカラーの変化を確認します。

   ![](assets/image2014-9-17-18-3a55-3a47.png)

[!DNL Paper Fest 12] プログラムは、より多くの収益（より大きなバブル）に影響を与えるだけでなく、比較的高いプログラムコスト（右側）にもかかわらず、[!UICONTROL &#x200B; トレードショー &#x200B;] チャネルのすべてのプログラムの投資への最良のリターン（最も環境に優しいバブル）を持っています。

>[!TIP]
>
>1 つのチャネルの複数のプログラムを、他のチャネルのプログラムと簡単に比較できます。ウィンドウ上部の「**チャネルフィルター**」を使用して、チャネルを追加するだけです。

>[!MORELIKETHIS]
>
>* [ プログラムアナライザーを使用したプログラムとチャネルの詳細の調査 ](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/explore-program-and-channel-details-with-the-program-analyzer.md)
>* [ チャネルの有効性と [!UICONTROL &#x200B; プログラムアナライザーの比較 &#x200B;]](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/compare-channel-effectiveness-with-the-program-analyzer.md)
