---
unique-page-id: 14352405
description: Sales Connect -Marketoドキュメント — 製品ドキュメントでのSAML 2.0を介したSSOの設定
title: Sales ConnectでのSAML 2.0を使用したSSOの設定
exl-id: aab80626-d6d1-4194-9733-09c90c0b49a6
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---

# Sales Connect {#setting-up-sso-through-saml-in-sales-connect}でのSAML 2.0を介したSSOの設定

SAML 2.0仕様を通じてSSOをサポートします。 現時点では、プロバイダーとの直接統合はありません。 この設定を取得するには、SSOプロバイダーから情報をいくつか収集する必要があります。

>[!NOTE]
>
>これは、**Marketo・セールス・コネクト**&#x200B;のお客様にのみ当てはまります。 Sales Connectをお持ちでなく、詳細をご希望の場合は、カスタマーサクセスマネージャーにお問い合わせください。

## 要件 {#requirements}

* SSOアカウント
* Marketoセールスコネクト購読
* SSOアカウントからのMetadata.xml（問題URL、検証のエンドポイント、および公開鍵）

## セットアップ {#setup}

チームのSSOインスタンスのmetadata.xmlには、発行者URL、検証のエンドポイント、および公開鍵を含める必要があります。

また、会社のSSOアカウントのSSOの場所を一意のドメインにする必要があります。 例えば、`toutapp.pingidentity.com`などの一意のサブドメインが必要です。 このタイプの一意の識別子がないと、ダッシュボードからSAMLを設定できません。

1つのログインとOktaは、URLの割り当て時に必ずしも一意の識別子を提供しない場合があります。 Oktaまたは1回のログインを使用している場合は、ダッシュボードボタンから1回のログインを設定できないことを意味します。 [Webアプリケーション](https://toutapp.com/login)の「シングルサインオン」ボタンから、この設定を引き続き行うことができます。

この情報を入手したら、エンジニアリングチームと協力して、お客様の購読に合わせてこの設定を行います。
