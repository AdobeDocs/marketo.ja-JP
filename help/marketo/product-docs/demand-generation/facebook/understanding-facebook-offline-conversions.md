---
unique-page-id: 11383945
description: Facebookのオフラインコンバージョンと、Marketoとの連携について説明します。 コンバージョンデータがどのように広告パフォーマンスを向上させるかを理解します。
title: Facebook オフラインコンバージョンについて
exl-id: e0995ebc-47fb-4f10-b767-4fe9f572b2d2
feature: Integrations
TQID: https://experienceleague.adobe.com/22t2foTWN-7xooxnnXuyk1l10kI-H4-gq0LbwbWSlns
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 241
ht-degree: 80%

---

# [!DNL Facebook] オフラインコンバージョンについて {#understanding-facebook-offline-conversions}

Facebook リード広告キャンペーンは、リードを生成し、マーケティングキャンペーンで使用するために Marketo に送信します。 ただし、オフラインのコンバージョンを可視化しないと、[!DNL Facebook]広告主はどの広告が最も効果的かを知ることができません。 次に例を示します。

>[!NOTE]
>
>**例**
>
>[!UICONTROL Facebook リード広告]では 3 つの広告が実行されます。
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
>オフラインコンバージョンがないと、広告主はおそらく広告 3 にさらに投資するでしょう。 オフラインコンバージョンデータを使用すると、広告主は広告 1 に投資する可能性が高くなります。

[Facebook オフラインコンバージョンを設定](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md)して、オフラインの広告パフォーマンスを [!DNL Facebook] に送信できます。

1. [[!DNL Facebook] [!UICONTROL LaunchPoint]統合](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-facebook-custom-audiences-as-a-launchpoint-service.md)が最新であることを確認します。
1. 収益サイクルモデルのステージを、[!DNL Facebook] のオフラインコンバージョンステージにマッピングします。
1. [!DNL Facebook] リードが [!DNL Facebook] リード広告から生成され、マッピングされたステージに到達すると、Marketo は、安全で自動化された API を使用して、オフラインコンバージョンデータを 1 日に数回 [!DNL Facebook] に送信します。 データが [!DNL Facebook] Ads Manager レポートに表示されます。

>[!MORELIKETHIS]
>
>[&#x200B; [!DNL Facebook]  オフラインコンバージョンの設定](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md)
