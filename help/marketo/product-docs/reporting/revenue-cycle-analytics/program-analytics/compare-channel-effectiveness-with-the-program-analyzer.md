---
unique-page-id: 2360401
description: プログラムアナライザーを使用したチャネルの効果の比較 - Marketo ドキュメント - 製品ドキュメント
title: プログラムアナライザーを使用したチャネルの効果の比較
exl-id: bfe635a7-b077-4074-889d-fc2256102cd5
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 100%

---

# [!UICONTROL プログラムアナライザー]を使用したチャネルの効果の比較 {#compare-channel-effectiveness-with-the-program-analyzer}

[!UICONTROL プログラムアナライザー]を使用して、チャネルコスト、メンバー獲得、パイプライン、売上高などを比較し、最も効果が高いチャネルと最も効果が低いチャネルを特定します。

>[!PREREQUISITES]
>
>[[!UICONTROL プログラムアナライザーの作成]](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/create-a-program-analyzer.md)

1. **[!UICONTROL My Marketo]** で「**分析**」をクリックします。

   ![](assets/image2014-9-17-18-3a36-3a13.png)

1. 「プログラムアナライザー」を選択します。

   ![](assets/image2014-9-17-18-3a36-3a40.png)

1. 「表示」を「**[!UICONTROL チャネル別]**」に変更します。

   ![](assets/image2014-9-17-18-3a36-3a59.png)

1. 「**[!UICONTROL X 軸]**」ドロップダウンを使用して、横軸の指標を選択します。まず、**[!UICONTROL プログラムコスト]**&#x200B;から始めましょう。

   ![](assets/image2014-9-17-18-3a37-3a7.png)

1. **[!UICONTROL Y 軸]**&#x200B;ドロップダウンを使用して、縦軸の指標を選択します。ここでは、「**[!UICONTROL （FT）パイプラインの作成]**」を行います。

   ![](assets/image2014-9-17-18-3a37-3a50.png)

   >[!NOTE]
   >
   >プログラムアナライザーで選択できる指標の多くは、ファーストタッチ（FT）計算とマルチタッチ（MT）計算で利用できます。[FT と MT のアトリビューションの違い](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md)を理解することが重要です。

1. 「**[!UICONTROL Y 軸]**」ドロップダウンを使用して、「**[!UICONTROL （MT）パイプライン作成]**」を選択します。

   ![](assets/image2014-9-17-18-3a39-3a5.png)

   このマルチタッチのアトリビューションを見ると、展示会やオンライン広告のチャネルより、ウェビナーのチャネルのほうが、作成されたパイプラインに対する影響が大きく、コストが低いことがわかります。

   次に、さらに 2 つのディメンションを追加します。

1. 「**[!UICONTROL バブルサイズ]**」ドロップダウンを使用して、「**[!UICONTROL 新しい名前]**」などのように、追加の測定を選択します。

   ![](assets/image2014-9-17-18-3a39-3a36.png)

1. グラフの変化を確認してください。

   ![](assets/image2014-9-17-18-3a39-3a55.png)

   「**[!UICONTROL 新しい名前]**」で測定すると、ウェビナーチャネルが縮小するのがわかります。メンバーは多くても、新しいリードの創出という点では、展示会のチャネルより効果が小さいと結論付けることができるでしょう。

1. 最後に、「カラー」ドロップダウンを使用して、4 つ目のディメンションを追加します。「**[!UICONTROL （FT）獲得した売上高]**」を選択します。

   ![](assets/image2014-9-17-18-3a41-3a7.png)

1. グラフのカラーの変化を確認します。

   ![](assets/image2014-9-17-18-3a41-3a19.png)

   色から、ファーストタッチアトリビューションで測定される、最も緑色のバブルである展示会チャネルが、売上高の獲得に最も大きく影響を与えていることがわかります。

1. ここで、カラー指標を「**[!UICONTROL （MT）獲得した売上高]**」に変更すると、オンライン広告チャネルが最も緑色になり、ウェビナーや展示会チャネルよりも&#x200B;_多く_&#x200B;売上高に影響したことがわかります。

   ![](assets/image2014-9-17-18-3a41-3a40.png)

この例では、ファーストタッチで作成されたパイプラインで測定した場合、展示会のチャネルが、最もコストが高く（最も右寄り）、最も成功している（Y 軸上で最も上）ことがわかります。次に、作成された各チャネルのパイプラインをマルチタッチのアトリビューションによって測定する場合を考えましょう。

>[!TIP]
>
>以上の手順の例では、作成されたパイプラインに基づいて効果を測定します。[!UICONTROL Y 軸]ドロップダウンを使用して、「[!UICONTROL 新しい名前]」、「[!UICONTROL メンバー]」、「[!UICONTROL 成功別コスト]」など、チャネルの効果を測定する他の方法を選択します。

>[!MORELIKETHIS]
>
>* [[!UICONTROL プログラムアナライザー]](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/explore-program-and-channel-details-with-the-program-analyzer.md)を使用したプログラムおよびチャネルの詳細の調査
>* [[!UICONTROL プログラムアナライザー]](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/compare-program-effectiveness-with-the-program-analyzer.md)を使用したプログラムの効果の比較
