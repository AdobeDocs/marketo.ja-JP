---
unique-page-id: 6094890
description: リリースノート - 2015年2月 - Marketo ドキュメント - 製品ドキュメント
title: リリースノート - 2015年2月
exl-id: a7ce88dc-a4d2-4ccb-9fe5-61130334d24d
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 35%

---

# リリースノート：2015年2月 {#release-notes-february}

2015年2月リリースには、次の機能が含まれています。お客様のご契約により、制限やオプションの契約が必要なものがあります。詳細は担当の営業にお問い合わせください。リリース後は、各機能に関する詳細な記事へのリンクを必ずご確認ください。ドラムロール…

## マーケティングの自動化の強化 {#marketing-automation-enhancements}

**[スマートキャンペーンの移動](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/move-a-smart-campaign.md)**

朗報です!ドラッグアンドドロップまたはツリー内の移動機能を使ってプログラムからスマートキャンペーンが移動できるようになりました。

**[Dynamics 2015（オンライン）](https://docs.marketo.com/display/docs/microsoft+dynamics+2013+on-premises)**  — サポート対象

**HTTPS証明書の変更**

Marketoは、顧客データおよびSaaSサービスの機密性と整合性を保護するため、SaaS業界のベストプラクティスに従っています

およびは、次のドメインで、現在使用されているセキュリティプロトコル（SHA-1およびSSL）を、よりセキュアなバージョン(SHA-2(a.k.a. SHA-256)およびTLS)に置き換えます。

* [marketo.net](https://marketo.net) （暗号化されたMunchkinトラフィック）

* [marketo.com](https://marketo.com) （メインのSaaSアプリケーション）

この問題は、このリリースの直後に発生します。 SHA-1プロトコルは、レガシーシステムおよびアプリケーションの所有者がSHA-2互換性を使用してシステムを更新できるように、2015年12月まで[mktoapi.com](https://mktoapi.com)ドメインで一時的にサポートされます。

**セキュアマンチキン**

SSL3のサポートは削除されます。 以前のWebブラウザーのサポートを維持するために、これまでSSL3を維持してきましたが、2015年には、これらのブラウザーからの大量のWebトラフィックは見られなくなりました。 これは、セキュリティで保護されたページで使用した場合にのみMunchkinに影響し、2月のリリース以降は徐々に展開されます。

## リアルタイムパーソナライゼーションの機能強化 {#real-time-personalization-enhancements}

**[キャンペーンのTarget URL](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/adding-a-target-url-to-a-web-campaign.md)**

「ターゲットURLの追加」を使って、リアルタイムキャンペーンを表示したいページを選択してください。この機能は、すべてのキャンペーンタイプ（ダイアログ、ゾーン、ウィジェット）で機能しますが、選択したターゲットURLのみのゾーンIDでキャンペーンがレンダリングされるゾーン内キャンペーンに特に役立ちます。 異なるWebページをターゲットにする複数のURLの追加をサポートします。

![](assets/image2015-2-19-11-3a0-3a30.png)

**アカウントベースターゲットへの国と都道府県の追加**

ネームドアカウントリストに国と都道府県が追加できます。特定のロケーションからのキーアカウントを絞りこめます。
