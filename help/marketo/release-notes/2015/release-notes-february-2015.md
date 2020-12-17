---
unique-page-id: 6094890
description: リリースノート — 2015年2月 — Marketto Docs — 製品ドキュメント
title: リリースノート — 2015年2月
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '336'
ht-degree: 0%

---


# リリースノート：2015年2月{#release-notes-february}

2015年2月リリースには次の機能が含まれています。 Marketing Editionで機能が利用できるかどうかを確認してください。 リリース後は、各機能の詳細記事へのリンクを必ず戻して参照してください。 ドラムロール…

## マーケティング自動化の強化{#marketing-automation-enhancements}

** [スマートキャンペーンを移動](../../product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/move-a-smart-campaign.md)**

喜べ！ ツリーのドラッグ&amp;ドロップまたは移動機能を使用して、プログラムの内外でスマートキャンペーンを移動できるようになりました。

** [Dynamics 2015 （オンライン）](http://docs.marketo.com/display/docs/microsoft+dynamics+2013+on-premises) ** — サポート！

**HTTPS証明書の変更**

顧客データおよびSaaSサービスの機密性と完全性を保護するため、MarketoはSaaS業界のベストプラクティスに従っています。

次のドメインでは、現在使用されているセキュリティプロトコル（SHA-1およびSSL）を、より安全なバージョン(SHA-2(a.k. SHA-256)およびTLS)に置き換えます。

`·` [marketo.net](http://marketo.net) （暗号化されたMunchkinトラフィック）

`·` [marketo.com](http://marketo.com) （メインのSaaSアプリケーション）

これは、このリリース後間もなく発生します。 2015年12月まで、SHA-1プロトコルは[mktoapi.com](http://mktoapi.com)ドメインで一時的にサポートされ、レガシーシステムやアプリケーションの所有者がSHA-2互換でシステムを更新できるようになります。

**セキュアマンチキン**

SSL3のサポートを削除します。 以前のWebブラウザーのサポートを維持するため、SSL3を今まで維持してきましたが、2015年には、これらのブラウザーからの大量のWebトラフィックは見られなくなりました。 これは、セキュリティで保護されたページでMunchkinを使用した場合にのみ影響し、2月のリリース後はゆっくり展開します。

## リアルタイムパーソナライゼーションの機能強化{#real-time-personalization-enhancements}

** [キャンペーンのターゲットURL](../../product-docs/web-personalization/working-with-web-campaigns/adding-a-target-url-to-a-web-campaign.md)**

「ターゲットURL」を使用して、リアルタイムキャンペーンに表示するページ追加を選択します。 この機能は、すべてのキャンペーンの種類(Dialog、In Zone、Widgets)で機能しますが、選択したターゲットURLのみのゾーンIDでキャンペーンがレンダリングされるゾーン内キャンペーンでは特に有用です。 ターゲットの異なるWebページへの複数のURLの追加をサポートします。

![](assets/image2015-2-19-11-3a0-3a30.png)

** [国と州がアカウントベースのターゲティングに追加](https://docs.marketo.com/display/DOCS/View+a+Named+Account+List)**

国および州を指定されたアカウントリストに追加できるようになりました。 特定の場所のターゲットキーアカウント見込み客。
