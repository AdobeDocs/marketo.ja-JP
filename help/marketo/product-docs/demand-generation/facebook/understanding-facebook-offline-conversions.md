---
unique-page-id: 11383945
description: Facebook オフラインコンバージョンについて — Marketo ドキュメント — 製品ドキュメント
title: Facebook オフラインコンバージョンについて
exl-id: e0995ebc-47fb-4f10-b767-4fe9f572b2d2
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '222'
ht-degree: 100%

---

# Facebook オフラインコンバージョンについて {#understanding-facebook-offline-conversions}

Facebook リード広告キャンペーンは、リードを生成し、マーケティングキャンペーンで使用するために Marketo に送信します。ただし、オフラインコンバージョンを視認できない場合、Facebook の広告主は、最も効果的な広告を把握できません。次に例を示します。

>[!NOTE]
>
>**例**
>
>Facebook リード広告では 3 つの広告が実行されます。
>
>* 広告 1 が 20 リードを生成
>* 広告 2 が 30 リードを生成
>* 広告 3 が 50 リードを生成

>
>
これらの数だけから、広告 3 が最も効果的に見えます。
>
>しかし、Marketo 側のデータを見ると、別の話が展開します。
>
>* 広告 1 が 10 件の売上を生成
>* 広告 3 が 2 件の売上を生成

>
>
つまり、広告 1 は、リードが少ないにもかかわらず、50% の成功率を示し、広告 3 はまったく効果がなかったということです。
>
>オフラインコンバージョンがないと、広告主はおそらく広告 3 にさらに投資するでしょう。オフラインコンバージョンデータを使用すると、広告主は広告 1 に投資する可能性が高くなります。

[Facebook Offline Conversions](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md) を設定して、オフラインの広告パフォーマンスを Facebook に送信できます。

1. [Facebook LaunchPoint 統合](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-facebook-custom-audiences-as-a-launchpoint-service.md)が最新であることを確認します。
1. 売上高サイクルモデルのステージを、Facebook のオフラインコンバージョンステージにマッピングします。
1. Facebook リードが Facebook リード広告から生成され、マッピングされたステージに到達すると、Marketo は、安全で自動化された API を使用して、オフラインコンバージョンデータを 1 日に数回 Facebook に送信します。データが Facebook Ads Manager レポートに表示されます。

>[!MORELIKETHIS]
>
>[Facebook オフラインコンバージョンの設定](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md)
