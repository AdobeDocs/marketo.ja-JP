---
unique-page-id: 11383945
description: facebookオフラインコンバージョンについて —Marketoドキュメント — 製品ドキュメント
title: facebookオフラインコンバージョンについて
exl-id: e0995ebc-47fb-4f10-b767-4fe9f572b2d2
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 0%

---

# facebookオフラインコンバージョンについて{#understanding-facebook-offline-conversions}

Facebookリード広告のキャンペーンはリードを生み出し、マーケティングキャンペーンで使用するためにMarketoに送ります。 ただし、オフラインコンバージョンが視認できない場合、Facebookの広告主はどの広告が最も効果的かを知ることができません。 次に例を示します。

>[!NOTE]
>
>**例**
>
>Facebookリード広告は3つの広告を掲載している。
>
>* 広告1は20のリードを生成
>* 広告2は30のリードを生成
>* 広告3は50のリードを生成

>
>
これらの数字だけから、広告3が最も効果的と思われます。
>
>しかし、Marketo側のデータを見ると、別の話が展開します。
>
>* 広告1は10件の売上を生み出す
>* 広告3は2つの売上を生み出す

>
>
つまり、広告1はリードを生み出す数が少ないにもかかわらず、成功率が50%で、広告3はほとんど効果がなかったということです。
>
>オフラインコンバージョンがない場合、広告主は広告3により多くの投資を行うでしょう。 オフラインコンバージョンデータを使用すると、広告主は広告1に投資する可能性が高くなります。

[Facebookオフラインコンバージョン](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md)を設定して、オフライン広告のパフォーマンスをFacebookに送信できます。

1. [FacebookLaunchPoint統合](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-facebook-custom-audiences-as-a-launchpoint-service.md)が最新の状態であることを確認してください。
1. 売上高サイクルモデルのステージをFacebookのオフラインコンバージョンステージにマッピングします。
1. facebookリード広告からFacebookリードが生成され、マッピングされたステージに到達すると、Marketoは安全な自動APIを介してオフラインコンバージョンデータを1日に数回Facebookに送り返します。 データは、Facebook広告マネージャーレポートに表示されます。

>[!MORELIKETHIS]
>
>[facebookオフラインコンバージョンの設定](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md)
