---
unique-page-id: 45416698
description: リリースノート — 20年7月21日 —Marketoドキュメント — 製品ドキュメント
title: リリースノート — 2010年7月
exl-id: 3c9b1f1d-961c-4bf8-8b99-37b483230506
translation-type: tm+mt
source-git-commit: d44f5e6f3fb24a25678e4d15ee4c6361b658556b
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 1%

---

# リリースノート：20日{#release-notes-july}

2007年7月21日リリースには、次の機能が含まれています。 Marketo版で利用可能な機能を確認してください。

>[!AVAILABILITY]
>
>現在のパッケージに応じて、星(![(star)](assets/yellow-star.png))を含む項目は、値のアドオンの購入が必要になる場合があります。 詳しくは、Marketo Engageの担当者にお問い合わせください。

**_四半期別_** リリース次の機能が2020 **年7月31日にリリースされます**。

## 管理 {#administration}

* **[Field Managementの「使用者」エクスポート](/help/marketo/product-docs/administration/field-management/export-used-by-data-for-a-field.md)**:管理者は、選択したフィールドの「使用者」アセットリンクをすべてCSVファイルに書き出せるようになりました。この機能強化は、管理者と非管理者の両方が、未使用のフィールドをクリーンアップするのに役立ちます。 また、アセットを新しいブラウザータブまたはブラウザーウィンドウで開くことができるようになりました。

## アカウントベースドマーケティング {#account-based-marketing}

![（星形）](assets/yellow-star.png)

* **アカウントプロファイルのUIが更新されました**:合理化された手順を1つの画面で行うことで、アカウントプロファイルでのターゲットアカウントリストの作成を簡単にします。

<br> 

**_四半期全体でリリース_**

次の機能は、四半期に属さないサイクルで提供され、今後数か月間にわたってリリースされます。

* **Formsサービス**:より強力なフォームフィールド構文の検証と、ランディングページ機能用の新しいセキュリティで保護されたドメインで一般的なボットパターンをブロックする機能が導入されています。ボットパターンをブロックすると、スパムフォームの送信を減らし、データベースの品質を向上させることができます。

>[!NOTE]
>
>強化されたフォームフィールド構文の検証の完全な展開は、2021年1月のリリース後まで延期されました。

* **Asset API URI Size Limit**:「_method」パラメーターを削除する前に、Uniform Resource Identifier(URI)のサイズ制限が8 KBから65 KBに増えています。長いクエリ文字列を実行する場合、このサイズ制限の増加によって、データの受け渡しがより容易になります。 「_method」パラメーターの削除は、今後のセキュリティアップグレードの一環です。

## Sales Insight {#sales-insight}

![（星形）](assets/yellow-star.png)

* **[非ネイティブSalesforce CRM統合](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md) （ベータ版）を使用するお客様向けのSales Insightの有効化**:ネイティブ以外のSalesforce CRM統合を使用するMarketo Engageのお客様は、Sales Insightを使用して、最も関与のあるリードやオポチュニティをセールスチームが理解し、優先順位を付け、やり取りを支援し、スマートな販売と迅速な取引を可能にします。

## セールスコネクト {#sales-connect}

![（星形）](assets/yellow-star.png)

* **[販売呼び出しに対する二者パーティの同意の強化：](/help/marketo/product-docs/marketo-sales-connect/phone/two-party-consent-settings.md)** 管理者が通話記録の設定をより詳細に制御できるようになりました。[双方の同意法に準拠していることを確認しながら、通話](/help/marketo/product-docs/marketo-sales-connect/phone/enable-call-recording.md) 記録を有効にします。録音中の呼び出しの通知を自動化し、呼び出しの前に再生されるオーディオクリップをアクティブにします。

<br> 

## お知らせと廃止{#announcements-deprecations}

* **アセットAPI &quot;_method&quot;パラメータの削除**:2020年9月以降、Asset APIエンドポイントで、URIの長さ制限を回避するために、POSTの本文にクエリパラメーターを渡すために「_method」を使用できなくなります。このパラメーターを必要とする要求に対応するために、アセットAPIのURI制限が8 KBから65 KBに増えます。
* **[Munchkin Associate Lead](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**:このリリースのMunchkin JavaScript Clientバージョン159では、Munchkin Associate Leadメソッドの廃止を開始します。呼び出すと、今後のリリースでメソッドが削除されることを示す警告が表示されます。 メソッドを削除すると、メソッドは機能しなくなり、使用の試みは失敗します。 この方法を最近使用したMarketo Engageのお客様には、その旨が個別に通知されます。
* **Internet Explorerのサポート**:前述のとおり、Internet Explorer 11のMarketo Engageサポートは2020年7月31日に終了 **します**。Google Chrome、Mozilla Firefox、Apple Safari、およびMicrosoft Edgeは引き続きサポートされます。
* **Skyのデフォルトエクスペリエンス**:管理者またはユーザーがMarketo Skyをデフォルトのエクスペリエンスとして設定するオプションは、プライマリユーザーエクスペリエンスの更新に備えて、このリリースで削除されます。主要なエクスペリエンスの更新に関する詳細は、今年中に予定されていますが、7月中に提供されます。 Marketo Skyをデフォルトのエクスペリエンスとして設定したユーザー、またはMarketo Skyへのアクセス権を付与されたユーザーは、マイMarketoホームページのタイルからMarketo Skyに引き続きアクセスできます。
* **EdgeHTML （Chromium以外の） Microsoft Edgeのサポート**:Marketo Engageは、2020年末にMicrosoft EdgeのEdgeHTMLバージョンをサポートしなくなります。2021年1月1日より、アドビは最新バージョンのChromium Edgeのみをサポートします。
