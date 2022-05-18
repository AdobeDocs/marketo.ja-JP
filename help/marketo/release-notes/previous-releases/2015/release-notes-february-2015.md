---
unique-page-id: 6094890
description: リリースノート - 2015 年 2 月 - Marketo ドキュメント - 製品ドキュメント
title: リリースノート - 2015 年 2 月
exl-id: a7ce88dc-a4d2-4ccb-9fe5-61130334d24d
source-git-commit: 6f15abf1fed69431b3bbe249c908b0f90a56d391
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 100%

---

# リリースノート：2015 年 2 月 {#release-notes-february}

2015 年 2 月リリースには、次の機能が含まれています。お客様のご契約により、制限やオプションの契約が必要なものがあります。詳細は担当の営業にお問い合わせください。リリース後は、各機能に関する詳細な記事へのリンクを必ずご確認ください。お待たせしました。

## マーケティング自動化の強化 {#marketing-automation-enhancements}

**[スマートキャンペーンの移動](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/move-a-smart-campaign.md)**

朗報です! ドラッグアンドドロップまたはツリー内の移動機能を使ってプログラムからスマートキャンペーンが移動できるようになりました。

**[Dynamics 2015（オンライン）](https://docs.marketo.com/display/docs/microsoft+dynamics+2013+on-premises)** — サポートされています。

**HTTPS 証明書の変更**

顧客データおよび SaaS サービスの機密性と整合性を保護するため、Marketo は SaaS 業界のベストプラクティスに従い、

次のドメインで、現在使用されているセキュリティプロトコル（SHA-1 および SSL）をより安全なバージョン（SHA-2（SHA-256）および TLS）に置き換えます。

* marketo.net（暗号化された Munchkin トラフィック）

* [marketo.com](https://marketo.com)（主な SaaS アプリケーション）

これは、このリリースの直後に発生します。SHA-1 プロトコルは、2015 年 12 月まで [mktoapi.com](https://mktoapi.com) のドメインで一時的にサポートされ、レガシーシステムおよびアプリケーションの所有者が SHA-2 互換でシステムを更新できるようにします。

**セキュア Munchkin**

SSL3 のサポートを削除します。古い web ブラウザーのサポートを維持するために、これまで SSL3 を維持してきましたが、2015 年には、これらのブラウザーからの大量の web トラフィックは見られなくなりました。これは、セキュアなページで使用した場合にのみ Munchkin に影響し、2 月のリリース以降はゆっくりと展開されます。

## リアルタイムパーソナライズ機能の強化 {#real-time-personalization-enhancements}

**[キャンペーンのターゲット URL](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/adding-a-target-url-to-a-web-campaign.md)**

「ターゲット URL を追加」を使って、リアルタイムキャンペーンを表示したいページを選択してください。この機能は、すべてのキャンペーンタイプ（ダイアログ、ゾーン内、ウィジェット）で機能しますが、選択したターゲット URL のみのゾーン ID でキャンペーンがレンダリングされるゾーン内キャンペーンで特に役立ちます。異なる web ページをターゲットにする複数の URL の追加をサポートします。

![](assets/image2015-2-19-11-3a0-3a30.png)

**アカウントベースターゲットへの国と都道府県の追加**

ネームドアカウントリストに国と都道府県が追加できます。特定のロケーションからのキーアカウントを絞りこめます。
