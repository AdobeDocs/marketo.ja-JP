---
unique-page-id: 3571886
description: 成功パス分析の使用 - Marketo ドキュメント - 製品ドキュメント
title: 成功パス分析の使用
exl-id: f816b7ac-a158-46bd-9d00-09ef4cc8b381
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 100%

---

# 成功パス分析の使用 {#using-the-success-path-analyzer}

成功パス分析を使用して、[収益サイクルモデル](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/understanding-revenue-models.md)のステージにおけるリードの流れ（量）と速度（日数で表したスピード）の両方を反映する特定の詳細を調査します。

>[!PREREQUISITES]
>
>[成功パス分析の作成](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/create-a-success-path-analyzer.md)

1. **[!UICONTROL 分析]**&#x200B;に移動し、「**成功パス分析**」を選択します。

   ![](assets/image2015-6-12-17-3a23-3a53.png)

   右側のグラフには、左側で選択したボタンのデータが反映されます。デフォルトでは、これは「**[!UICONTROL 残高]**」です。

1. 「**[!UICONTROL インフロー]**」をクリックして、選択した期間にステージに入った人数をグラフ化します。

   ![](assets/image2015-6-12-17-3a30-3a52.png)

   * 「**[!UICONTROL アウトフロー]**」をクリックして、ステージから離脱した人数をグラフ化します。
   * 「**[!UICONTROL コンバージョン率]**」をクリックして、このステージから次のステージへのコンバージョン率をグラフ化します。
   * 「**[!UICONTROL 平均時間]**」をクリックして、訪問者が次のステージに移るまでにこのステージに費やした時間を確認します。

1. **[!UICONTROL グラフのアクション]**／**[!UICONTROL 期間を比較]**&#x200B;をクリックして、データを同じ長さの異なる期間と比較します。

   ![](assets/image2015-6-12-17-3a39-3a15.png)

1. 比較期間の&#x200B;**[!UICONTROL 開始]**&#x200B;日を選択します。

   ![](assets/image2015-6-12-17-3a43-3a49.png)

   **[!UICONTROL 終了]**&#x200B;日は、元の期間の長さに合わせて自動的に設定されます。

1. 「**[!UICONTROL 比較]**」をクリックします。

   ![](assets/image2015-6-12-17-3a44-3a8.png)

1. グラフは、比較期間の重複するデータを緑色で更新します。

   ![](assets/image2015-6-12-17-3a46-3a16.png)

1. グラフの時間スケールを変更するには、**[!UICONTROL グラフの基準]**&#x200B;ボタンのいずれか（毎日（デフォルト）、毎週、毎月）をクリックします。

   ![](assets/image2015-6-12-17-3a46-3a55.png)

1. SLA （Service-Level Agreements）を使用するステージの場合、**[!UICONTROL グラフのアクション]**／**[!UICONTROL SLA 期限の表示]**&#x200B;をクリックして、指定した期間内に SLA ターゲットを逃したことのあるすべてのリードを表示します。

   ![](assets/image2015-6-12-17-3a49-3a23.png)

1. グラフが更新され、各ノードで発生した SLA の数が橙色で表示されます。

   ![](assets/image2015-6-12-17-3a50-3a16.png)

   橙色で表示されているリードは、SLA ステージに残っている場合と&#x200B;*残っていない*&#x200B;場合があります。

1. **[!UICONTROL グラフのアクション]**／**[!UICONTROL 期限切れ SLA の表示]**&#x200B;をクリックして、期限切れの SLA ターゲットを持ち、指定された期間の終わりにまだ SLA ステージにいるすべてのリードを表示します。

   ![](assets/image2015-6-12-17-3a51-3a39.png)

1. グラフが更新され、各ノードで期限切れになっている SLA の数が橙色で表示されます。

   ![](assets/image2015-6-12-17-3a52-3a17.png)

1. 特定のノード（日付）上のデータポイントの特定の詳細を読み取るには、バブルにマウスポインタを合わせます。

   ![](assets/image2015-6-12-17-3a52-3a49.png)

1. グラフを印刷するには、**[!UICONTROL グラフのアクション]**／**[!UICONTROL グラフを印刷]**&#x200B;をクリックします。

   ![](assets/image2015-6-12-17-3a53-3a34.png)

アナライザーは、モデル内の動きを理解するのに役立ちます。より進化するにつれ、マーケティング戦略を立てる上で非常に重要になります。
