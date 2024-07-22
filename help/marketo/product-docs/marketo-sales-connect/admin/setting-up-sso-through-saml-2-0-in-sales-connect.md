---
unique-page-id: 14352405
description: Sales Connect で SAML 2.0 を使用した SSO の設定 — Marketo ドキュメント — 製品ドキュメント
title: Sales Connect で SAML 2.0 を使用した SSO の設定
exl-id: aab80626-d6d1-4194-9733-09c90c0b49a6
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 100%

---

# Sales Connect で SAML 2.0 を使用した SSO の設定 {#setting-up-sso-through-saml-in-sales-connect}

SAML 2.0 仕様で SSO をサポートしています。ただし、現時点では、どのプロバイダーとの直接統合もおこなっていません。この設定を取得するには、SSO プロバイダーから情報を収集する必要があります。

>[!NOTE]
>
>これは、**Marketo Sales Connect** ユーザーにのみ適用されます。Sales Connect をお持ちでなく詳細をお知りになりたい場合は、アドビアカウントチーム（担当のアカウントマネージャー）にお問い合わせください。

## 要件 {#requirements}

* SSO アカウント
* Marketo Sales Connect サブスクリプション
* SSO アカウントからの metadata.xml（イシュー URL、検証用のエンドポイント、公開鍵）

## セットアップ {#setup}

チームの SSO インスタンスの metadata.xml には、発行者 URL、検証用のエンドポイント、および公開鍵が含まれている必要があります。

また、会社の SSO アカウントを一意のドメインにするには、SSO の場所も必要です。例えば、`toutapp.pingidentity.com` または類似のサブドメインが必要です。このタイプの一意の識別子がないと、ダッシュボードから SAML を設定できなくなります。

One Login と Okta で、URL を割り当てる際に、一意の識別子を提供できない場合があります。Okta または One Login を使用している場合、One Login はダッシュボードボタンから設定できません。[web アプリケーション](https://toutapp.com/login)の「シングルサインオン」ボタンからは設定できます。

この情報を入手したら、アドビのエンジニアリングチームと協力して、お客様のサブスクリプション用にこれを設定します。
