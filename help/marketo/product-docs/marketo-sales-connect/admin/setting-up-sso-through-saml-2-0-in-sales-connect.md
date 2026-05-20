---
unique-page-id: 14352405
description: Sales ConnectでSAML 2.0を使用してSSOを設定する方法について説明します。 SSO プロバイダーと一意のドメインの要件とセットアップ手順を確認します。
title: ' [!DNL Sales Connect] で SAML 2.0 を使用した SSO の設定'
exl-id: aab80626-d6d1-4194-9733-09c90c0b49a6
feature: Marketo Sales Connect
TQID: https://experienceleague.adobe.com/FLGacQUvOJFtKJ5O1PzWRmpk3Zm1KH1D-W3ATHSVRSA
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 270
ht-degree: 91%

---

# [!DNL Sales Connect] で SAML 2.0 を使用した SSO の設定 {#setting-up-sso-through-saml-in-sales-connect}

SAML 2.0 仕様で SSO をサポートしています。 ただし、現時点では、どのプロバイダーとの直接統合もおこなっていません。 この設定を取得するには、SSO プロバイダーから情報を収集する必要があります。

>[!NOTE]
>
>これは、**Marketo Sales Connect** ユーザーにのみ適用されます。 Sales Connect をお持ちでなく詳細をお知りになりたい場合は、アドビアカウントチーム（担当のアカウントマネージャー）にお問い合わせください。

## 要件 {#requirements}

* SSO アカウント
* Marketo Sales Connect サブスクリプション
* SSO アカウントからの metadata.xml（イシュー URL、検証用のエンドポイント、公開鍵）

## 設定 {#setup}

チームの SSO インスタンスの metadata.xml には、発行者 URL、検証用のエンドポイント、および公開鍵が含まれている必要があります。

また、会社の SSO アカウントを一意のドメインにするには、SSO の場所も必要です。 例えば、`toutapp.pingidentity.com` または類似のサブドメインが必要です。 このタイプの一意の識別子がないと、ダッシュボードから SAML を設定できなくなります。

One Login と Okta で、URL を割り当てる際に、一意の識別子を提供できない場合があります。 Okta または One Login を使用している場合、One Login はダッシュボードボタンから設定できません。 [web アプリケーション](https://toutapp.com/login)の「シングルサインオン」ボタンからは設定できます。

この情報を入手したら、アドビのエンジニアリングチームと協力して、お客様のサブスクリプション用にこれを設定します。
