---
unique-page-id: 2360403
description: プログラムアナライザーを使用したプログラムの効果の比較 - Marketo ドキュメント - 製品ドキュメント
title: プログラムアナライザーを使用したプログラムの効果の比較
exl-id: 6e54d0a4-3cff-46cf-be0d-1992a39d8c03
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 100%

---

# [!UICONTROL プログラムアナライザー]を使用したプログラムの効果の比較 {#compare-program-effectiveness-with-the-program-analyzer}

[!UICONTROL プログラムアナライザー]を使用して、プログラムコスト、メンバー獲得、パイプライン、収益を比較することで、最も効果の高いまたは最も効果の低いプログラムを特定します。

>[!PREREQUISITES]
>
>[[!UICONTROL プログラムアナライザーの作成]](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/create-a-program-analyzer.md)

1. 「**[!UICONTROL 分析]**」をクリックします。

   ![](assets/image2014-9-17-18-3a50-3a30.png)

1. 「プログラムアナライザー」を選択します。

   ![](assets/image2014-9-17-18-3a50-3a37.png)

1. 「表示」を「**[!UICONTROL プログラム別]**」に変更します。

   ![](assets/image2014-9-17-18-3a50-3a44.png)

1. **[!UICONTROL チャネルフィルター]**&#x200B;を使用して、表示を 1 つまたは 2 つのチャネルに縮小します。ここでは、**[!UICONTROL Tradeshow]** チャネルのプログラムについて見てみましょう。

   ![](assets/image2014-9-17-18-3a51-3a2.png)

   >[!TIP]
   >
   >プログラムを 1 つのチャネルに絞り込む簡単な方法は、**[!UICONTROL 表示]**／**[!UICONTROL チャネル別]**&#x200B;を選択し、そのチャネルのバブルをクリックして、ポップアップダイアログでチャネル名をクリックすることです。

1. 「**[!UICONTROL X 軸]**」ドロップダウンを使用して、横軸の指標を選択します。まず、「**[!UICONTROL プログラムコスト]**」から始めます。

   ![](assets/image2014-9-17-18-3a52-3a16.png)

1. 「**[!UICONTROL Y 軸]**」ドロップダウンを使用して、縦軸の指標を選択します。新しいリードをキャプチャするのに適したプログラムを見つけるには、「**[!UICONTROL 新しい名前]**」を選択します。

   ![](assets/image2014-9-17-18-3a52-3a26.png)

1. スライダーをオンにしてズームインします。

   ![](assets/image2014-9-17-18-3a53-3a9.png)

   >[!TIP]
   >
   >また、線形から対数スケールに変更したり、その逆に変更したりして、表示を向上させることもできます。上部の&#x200B;**[!UICONTROL 拡大・縮小]**&#x200B;メニューを使用します。

1. 結果のグラフを表示します。

   ![](assets/image2014-9-17-18-3a53-3a49.png)

   この例では、[!DNL Origami Expo] は、そのチャネル内の他のすべてのプログラムよりも、新しい名前の取得にはるかに優れており、コストも中程度であることがわかります。ただし、それだけではありません。さらに 2 つの指標を追加して、より深く理解できるようにします。

1. 「**[!UICONTROL バブルサイズ]**」ドロップダウンを使用して、バブルのサイズで比較する指標を選択します。例として、「**[!UICONTROL （FT）獲得した収益]**」を選択します。

   ![](assets/image2014-9-17-18-3a54-3a25.png)

   >[!NOTE]
   >
   >プログラムアナライザーで選択できる指標の多くは、ファーストタッチ（FT）計算とマルチタッチ（MT）計算で利用できます。[FT と MT のアトリビューションの違い](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md)を理解することが重要です。

1. グラフ内でバブルのサイズが変化することを確認します。

   ![](assets/image2014-9-17-18-3a54-3a57.png)

   「**[!UICONTROL （FT）獲得した収益]**」を加えると、[!DNL Origami Expo] が多くの新しい名前を獲得したのに対し、比較的少ない収益に終わったことがすぐにわかります。また、[!DNL Paper Fest 12] プログラムは、獲得した名前は少ないですが、より多くの収益の獲得に影響を与えた（より大きなバブル）ため、優れた名前を獲得したことが確認できます。

1. 「カラー」ドロップダウンを使用して、4 つ目の指標を追加します。「**[!UICONTROL （FT）収益対投資]**」を見てみましょう。

   ![](assets/image2014-9-17-18-3a55-3a33.png)

1. グラフのカラーの変化を確認します。

   ![](assets/image2014-9-17-18-3a55-3a47.png)

[!DNL Paper Fest 12] プログラムは、より多くの収益（より大きなバブル）に影響を与えるだけでなく、比較的高いプログラムコスト（右端）にもかかわらず、[!UICONTROL 展示会] チャネルの全プログラムの中で最も高い投資収益率（最も緑色のバブル）を持ちます。

>[!TIP]
>
>1 つのチャネルの複数のプログラムを、他のチャネルのプログラムと簡単に比較できます。ウィンドウ上部の「**チャネルフィルター**」を使用して、チャネルを追加するだけです。

>[!MORELIKETHIS]
>
>* [[!UICONTROL プログラムアナライザー]](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/explore-program-and-channel-details-with-the-program-analyzer.md)を使用したプログラムおよびチャネルの詳細の調査
>* [[!UICONTROL プログラムアナライザー]](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/compare-channel-effectiveness-with-the-program-analyzer.md)を使用したチャネルの効果の比較
