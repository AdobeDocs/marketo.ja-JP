---
unique-page-id: 11383945
description: Facebookオフラインコンバージョンについて — Marketto Docs — 製品ドキュメント
title: Facebookオフラインコンバージョンについて
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '224'
ht-degree: 0%

---


# Facebookオフラインコンバージョンについて {#understanding-facebook-offline-conversions}

Facebookのリード広告のキャンペーンは、リードを生成し、マーケティングキャンペーンで使用できるようにマーケティング担当者に送信します。 ただし、オフラインコンバージョンが表示されないと、Facebookの広告主はどの広告が最も効果的かを知ることができません。 次に例を示します。

>[!NOTE]
>
>**例**
>
>Facebookリード広告は3つの広告を実行します。
>
>* 広告1は20のリードを生成
>* 広告2は30のリードを生成
>* 広告3は50のリードを生成

>
>
これらの数字だけから、広告3が最も効果的と思われます。
>
>しかし、マーケット側のデータを見ると、別のストーリーが展開します。
>
>* 広告1は10件の売上を生み出す
>* 広告3は2つの売上を生み出す

>
>
つまり、広告1はリードを生み出す数が少ないにもかかわらず、成功率が50%で、広告3はほとんど効果がなかったということです。
>
>オフラインコンバージョンがない場合、広告主は広告3により多くの投資を行うでしょう。 オフラインコンバージョンデータを使用すると、広告主は広告1に投資する可能性が高くなります。

Facebookのオフラインコンバージョンを [設定して](set-up-facebook-offline-conversions.md) 、オフライン広告のパフォーマンスをFacebookに送信できます。

1. Facebook LaunchPoint統合が最新の [ものであることを確認します](../../../product-docs/demand-generation/ad-network-integrations/add-facebook-custom-audiences-as-a-launchpoint-service.md) 。
1. 売上高サイクルモデルのステージをFacebookのオフラインコンバージョンステージにマッピングします。
1. FacebookのリードがFacebookのリード広告から生成され、マッピングされたステージに到達すると、Marketorは、安全な自動APIを介してオフラインコンバージョンデータを1日に数回Facebookに送信します。 データがFacebook広告マネージャーレポートに表示されます。

>[!NOTE]
>
>**関連記事**
>
>* [Facebookオフラインコンバージョンの設定](set-up-facebook-offline-conversions.md)

>



