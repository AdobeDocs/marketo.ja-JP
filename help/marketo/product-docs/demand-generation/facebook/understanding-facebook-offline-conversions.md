---
unique-page-id: 11383945
description: Facebook オフラインコンバージョンについて — Marketo ドキュメント — 製品ドキュメント
title: Facebook オフラインコンバージョンについて
exl-id: e0995ebc-47fb-4f10-b767-4fe9f572b2d2
feature: Integrations
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 57%

---

# [!DNL Facebook] オフラインコンバージョンについて {#understanding-facebook-offline-conversions}

Facebook リード広告キャンペーンは、リードを生成し、マーケティングキャンペーンで使用するために Marketo に送信します。ただし、オフラインコンバージョンを可視化しないと、[!DNL Facebook] の広告主はどの広告が最も効果的かを知ることができません。 次に例を示します。

>[!NOTE]
>
>**例**
>
>[!UICONTROL Facebook リード広告 ] は 3 つの広告を実行します。
>
>* 広告 1 が 20 リードを生成
>* 広告 2 が 30 リードを生成
>* 広告 3 が 50 リードを生成
>
>これらの数だけから、広告 3 が最も効果的に見えます。
>
>しかし、Marketo 側のデータを見ると、別の話が展開します。
>
>* 広告 1 が 10 件の売上を生成
>* 広告 3 が 2 件の売上を生成
>
>つまり、広告 1 は、リードが少ないにもかかわらず、50% の成功率を示し、広告 3 はまったく効果がなかったということです。
>
>オフラインコンバージョンがないと、広告主はおそらく広告 3 にさらに投資するでしょう。オフラインコンバージョンデータを使用すると、広告主は広告 1 に投資する可能性が高くなります。

[Facebook オフラインコンバージョンを設定 ](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md) して、オフライン広告パフォーマンスを [!DNL Facebook] に送信できます。

1. [[!DNL Facebook] [!UICONTROL LaunchPoint] 統合 ](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-facebook-custom-audiences-as-a-launchpoint-service.md) が最新であることを確認します。
1. 収益サイクルモデルのステージを、[!DNL Facebook] のオフラインコンバージョンステージにマッピングします。
1. [!DNL Facebook] リードが [!DNL Facebook] リード広告から生成され、マッピングされたステージに到達すると、Marketoは、安全な自動 API を使用して、オフラインコンバージョンデータを 1 日に数回 [!DNL Facebook] に送り返します。 データは、[!DNL Facebook] 広告マネージャーレポートに表示されます。

>[!MORELIKETHIS]
>
>[ 設定  [!DNL Facebook]  オフラインコンバージョン ](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md)
