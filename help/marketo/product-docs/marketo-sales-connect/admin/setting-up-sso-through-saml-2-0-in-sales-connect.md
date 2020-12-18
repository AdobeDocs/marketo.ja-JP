---
unique-page-id: 14352405
description: Sales Connect - Marketto Docs - Product DocumentationでのSAML 2.0を介したSSOの設定
title: Sales ConnectでのSAML 2.0を使用したSSOの設定
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 0%

---


# Sales Connect {#setting-up-sso-through-saml-in-sales-connect}でのSAML 2.0を介したSSOの設定

SAML 2.0仕様を通じてSSOをサポートします。 現時点では、プロバイダーとの直接統合はありません。 この設定を取得するには、SSOプロバイダーから情報をいくつか収集する必要があります。

>[!NOTE]
>
>**Reminder**
>
>これは、**Marketo Sales Connect**&#x200B;のお客様にのみ適用されます。 Sales Connectをお持ちでなく、詳細をご希望の場合は、カスタマーサクセスマネージャーにお問い合わせください。

## 要件{#requirements}

* SSOアカウント
* Marketo Salesの接続購読
* SSOアカウントからのMetadata.xml（問題URL、検証のエンドポイント、および公開鍵）

## セットアップ{#setup}

チームのSSOインスタンスのmetadata.xmlには、発行者URL、検証のエンドポイント、および公開鍵を含める必要があります。

また、会社のSSOアカウントのSSOの場所を一意のドメインにする必要があります。 例えば、`require a unique subdomain`は「toutapp.pingidentity.com」などと似ています。 このタイプの一意の識別子がないと、ダッシュボードからSAMLを設定できません。

1つのログインとOktaは、URLの割り当て時に必ずしも一意の識別子を提供しない場合があります。 Oktaまたは1回のログインを使用している場合、ダッシュボードボタンから1回のログインを設定できないことを意味します。 [Webアプリケーション](http://toutapp.com/login)の「シングルサインオン」ボタンから、この設定を引き続き行うことができます。

この情報を入手したら、エンジニアリングチームと協力して、お客様の購読に合わせてこの設定を行います。
