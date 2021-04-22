---
unique-page-id: 6094890
description: リリースノート — 2015年2月 —Marketoドキュメント — 製品ドキュメント
title: リリースノート — 2015年2月
exl-id: a7ce88dc-a4d2-4ccb-9fe5-61130334d24d
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 21%

---

# リリースノート：2015年2月{#release-notes-february}

2015年2月リリースには次の機能が含まれています。 Marketo版で利用可能な機能を確認してください。 リリース後は、各機能の詳細記事へのリンクを必ず戻して参照してください。 ドラムロール…

## マーケティング自動化の強化{#marketing-automation-enhancements}

**[スマートキャンペーンの移動](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/move-a-smart-campaign.md)**

朗報です!ドラッグアンドドロップまたはツリー内の移動機能を使ってプログラムからスマートキャンペーンが移動できるようになりました。

**[Dynamics 2015 （オンライン）](https://docs.marketo.com/display/docs/microsoft+dynamics+2013+on-premises)**  — サポート！

**HTTPS証明書の変更**

Marketoは、顧客データおよびSaaSサービスの機密性と完全性を保護するため、SaaS業界のベストプラクティスに従っています。

次のドメインでは、現在使用されているセキュリティプロトコル（SHA-1およびSSL）を、より安全なバージョン(SHA-2(a.k. SHA-256)およびTLS)に置き換えます。

* [marketo.net](https://marketo.net) （暗号化されたMunchkinトラフィック）

* [marketo.com](https://marketo.com) （メインのSaaSアプリケーション）

これは、このリリース後間もなく発生します。 2015年12月まで、SHA-1プロトコルは[mktoapi.com](https://mktoapi.com)ドメインで一時的にサポートされ、レガシーシステムやアプリケーションの所有者がSHA-2互換でシステムを更新できるようになります。

**セキュアマンチキン**

SSL3のサポートを削除します。 古いWebブラウザーのサポートを維持するため、SSL3を今まで維持してきましたが、2015年には、これらのブラウザーからの大量のWebトラフィックは見られなくなりました。 これは、セキュリティで保護されたページでMunchkinを使用した場合にのみ影響し、2月のリリース後はゆっくり展開します。

## リアルタイムパーソナライゼーションの機能強化{#real-time-personalization-enhancements}

**[キャンペーンのターゲットURL](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/adding-a-target-url-to-a-web-campaign.md)**

「ターゲットURLの追加」を使って、リアルタイムキャンペーンを表示したいページを選択してください。この機能は、すべてのキャンペーンの種類(Dialog、In Zone、Widgets)で機能しますが、選択したターゲットURLのみのゾーンIDでキャンペーンがレンダリングされるゾーン内キャンペーンでは特に有用です。 ターゲットの異なるWebページへの複数のURLの追加をサポートします。

![](assets/image2015-2-19-11-3a0-3a30.png)

**アカウントベースターゲットへの国と都道府県の追加**

ネームドアカウントリストに国と都道府県が追加できます。特定のロケーションからのキーアカウントを絞りこめます。
