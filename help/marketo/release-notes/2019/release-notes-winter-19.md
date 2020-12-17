---
unique-page-id: 17727823
description: リリースノート — Winter 19 - Marketto Docs — 製品ドキュメント
title: リリースノート — Winter '19
translation-type: tm+mt
source-git-commit: dc20aede0894a09e6c0bcd3d1580859b5fecb5f1
workflow-type: tm+mt
source-wordcount: '1112'
ht-degree: 0%

---


# リリースノート：冬&#39;19 {#release-notes-winter}

Winter 19リリースには、次の機能が含まれています。 Marketing Editionで機能が使用できるかどうかを確認します。

タイトルリンクをクリックすると、各機能の表示の詳細記事が表示されます（ある場合）。

>[!NOTE]
>
>Facebookでは、カスタムオーディエンスの統合を活用するために、Business Managerアカウントが必要になりました。 Facebook LaunchPointサービス&#x200B;*をBusiness Managerアカウントに関連付ける必要があります*。関連付けが行われないと、2019年1月14日&#x200B;**以降、統合は機能しなくなります。** Business Managerアカウントを設定するには、[Facebookのヘルプ](https://www.facebook.com/business/help/1710077379203657)を参照してください。

>[!NOTE]
>
>Microsoftは、すべてのオンラインユーザーに対して、最新バージョンのMicrosoft Dynamicsへのアップグレードを要求しています。 MarketoインスタンスをDynamics Onlineと統合する場合、統合が引き続き機能するように、**2019年1月31日**&#x200B;の前に、Marketo Solutionの最新バージョン](../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution/upgrade-the-marketo-solution-for-microsoft-dynamics.md)に[アップグレードする必要があります。

>[!NOTE]
>
>Marketoは、GoToWebinarのOAuthバージョンを1.0から2.0にアップグレードしています。OAuth 1.0のサポートは2019年1月に廃止されます。 GoToWebセミナーのお客様は、統合が引き続き機能するように、LaunchPoint（管理領域の）を使用して&#x200B;**2019年1月31日**&#x200B;までに再認証する必要があります。 詳しくは、[コミュニティページ](https://nation.marketo.com/docs/DOC-6739-gotowebinar-authentication-change-take-action-before-1312019)を参照してください。

## コアプラットフォームの強化{#core-platform-enhancements}

** [Marketto Emails](../../product-docs/email-marketing/general/email-cc.md)の電子メールCC**

受信者1人あたり最大5つのCCアドレスを、マーケティング担当者経由で送信される電子メールに含めます。

**API**

* **アセットAPIのマルチブランドドメインのサポート：アセットの** 承認と複製は、APIとUIで同じ結果になります。
* **Asset APIの電子メールCCサポート**:APIを使用した電子メールの複製、承認、および処理を行うユーザーは、UI設定と同一性を維持します。

** [Munchkin v155 （ベータ版）](http://developers.marketo.com/javascript-api/lead-tracking/configuration/)**

* **APIのみのモード**:ユーザーは、マーケティング担当者の自動追跡に依存する代わりに、単一ページのWebアプリで、Webページの訪問を記録するタイミングを明示的に呼び出すことで、データベースのメンバーを追跡するタイミングと方法を決定できるようになりました。
* **オプトアウト管理**:オプトアウトcookieドメインをMunchkin追跡cookieドメインと一致させることで、オプトアウトを簡単に管理できます。
* **Domain-Level Decider Parameter**:2文字のドメイン(例：&quot;  [webサイト.io](http://website.io)&quot;)は、追加のセットアップ要件なしに、Marketoで自動的に追跡されます。

## マーケティング担当営業{#marketo-sales-engage}

* **Salesforceカスタムプロファイル**:Sales Engageは、無制限のカスタムプロファイルをサポートするようになりました。

* **Salesforceのカスタマイズ**:重要でないカスタムアクティビティのフィールドを削除すると、CRMプラットフォームにSales Engageをより効率的に設定できます。
* **Email Service**:Microsoft Outlookに（[電子メール接続]タブのOffice365またはOn-Prem経由で）接続することで、配信品質と、返信追跡機能、スケジュール済みの電子メール機能、およびバルク電子メール機能が向上しました。
* **新しい管理設定**:Sales Engageインスタンスを最適化する2つの管理ページが追加されました。

   * *チーム* 管理では、管理者が購読やチームを編集できるようにすることで、シームレスなアカウント設定プロセスをサポートしています。
   * *Salesforce管理者* 設定シェルプチームは、SFDC同期を以前に比べて迅速かつ容易に設定します。

* **OWA Plugin for Windows**:1つのアドインを1つ追加すると、Windows Office 365のすべてのクライアントがSales Engageでサポートされ、Outlookでライブフィードを使用できます。新しいプラグインがMicrosoft Storeで入手できます。
* **アクティビティプッシャー**:販売を同期してコアマーケティングプラットフォームに関与させ、リアルタイムのマーケティングインサイトを活用します。

## Marketo Sky{#marketo-sky}

>[!NOTE]
>
>Marketo Skyリリースは、より頻繁に行われます。 第4四半期前半には、以下の機能および機能強化がリリースされる予定です。 詳細と更新情報については、[Skyのドキュメント](https://help.marketo.com/hc/en-us/articles/360012858573)を参照してください。

* **デフォルトエクスペリエンス**（オプション）:管理者からアクセス権が付与されている場合、マーケティング担当者は、Marketo Skyをデフォルトのエクスペリエンスとして設定できます。

* **マーケティング担当者**:重要な情報、通知、最も頻繁に訪問される領域へのリンクを提供するウィジェットを追加して、エクスペリエンスをカスタマイズします。

* **Design Studioリスト表示と詳細ページ**:電子メール、ランディングページ、フォームのフィルタリングおよび検索が可能なリスト表示により、組織と正確性のレベルを高めます。アセットの詳細ページには、アセットが使用されているプログラム、使用されているスニペットの数など、各アセットに関する主な情報が表示されます。

* **グローバル検索**:プラットフォーム全体で、オファーがより高速でより強力なグローバル検索機能を使用できるようになりました。検索クエリは、アクセス可能なすべてのワークスペースに対して実行でき、アセット（アクティブとアーカイブの両方）、ラベル、キャンペーン、プログラムを検索できるようになりました。 検索結果はオーバーレイを介して提供され、各結果にはアセットの居住地を指定するファイルの場所のトレールが含まれます。

* **ユーザーインターフェイスの強化**:新しいアイコン、モデル、ボタン、および新しいカラーパレットに加え、ブランドの刷新を反映し、Marketo Skyをより魅力的で機能的にします。

* **電子メールプログラムのユーザビリティの強化**:従来のMarketor Lead Managementプラットフォームと新しいMarketo Skyエクスペリエンスの間で、電子メールプログラム機能の統一に向けて、引き続き努力していきます。
* **ウェビナーを使用するイベントプログラム**:ウェビナーイベントプログラムは、Marketo Skyで利用できるようになりました(注意：このリリースではGoToWebinarのみサポートされ、時間の経過とともに確立される統合が追加されます)。

## アカウントベースのマーケティング{#account-based-marketing}

** [ABM Persona-Based Segmentation &amp; Filtering](../../product-docs/account-based-marketing/using-personas.md)**

名前付きアカウント内の特定の個人に合わせてABMキャンペーンをパーソナライズします。 ABM Persona機能は、リードのセグメント化に基づいてデフォルトの役職を作成し、追加のパーソナルセグメントを設定できます。

## 解析{#analytics}

**Bizible**

* **カスタムの計算フィールド**:任意のBizible属性を使用して、ダッシュボードのレポートとセグメント化に使用できるカスタムフィールドを作成します。

* **SOC II Type II認定**:セキュリティとプライバシーに関する新しい認定は、今年の初めからType I認定に基づいて行われます。

## Webパーソナライゼーション{#web-personalization}

**[アカウント設定の追加サブドメイン](/help/marketo/product-docs/web-personalization/getting-started/workspaces-in-web-personalization.md)**

ドメインとサブドメインをより効率的に管理するために、ユーザーはRTPアカウント設定にサブドメインを追加できるようになりました。

## Marketo Mobile Engagement(MME) {#marketo-mobile-engagement-mme}

**Android向けMMEソフトウェア開発キット(SDK)の更新**

Android向けSDKは、より柔軟性と新しいエンジニアリング機能を備えた、よりモダンで安定性と拡張性の高いフレームワークに更新されました。 Androidアプリの開発者は、Googleの[Firebase Cloud Messaging](http://firebase.google.com/docs/cloud-messaging/)(FCM)をこの新しいSDKで直接使用できるようになりました。

* [開発者向けの手順](http://developers.marketo.com/mobile/installation/#android_adding_fcm_to_your_application)
* [開発者向けFAQ](http://developers.marketo.com/mobile/installation/#android_fcm_faq)

>[!NOTE]
>
>アプリ開発者&#x200B;**は、2019年3月31日までに新しいバージョンに更新する必要があります。** 2019年3月31日までにSDKを更新しない場合、この日以降にアプリをダウンロードした新規ユーザーは、最新バージョンのSDKに更新するまでプッシュ通知を受信できません。 SDKの更新では、現在のモバイルアプリユーザーが新しいバージョンのアプリを再ダウンロードする必要はありません。

## 追加の更新{#additional-updates}

**拡張可能なウェビナープラットフォーム**

製品リリースに加えて、パートナーチームは、ウェビナープロバイダーがMarketorとの統合を構築し維持できる新しいフレームワークに取り組み、ソリューションの更新と強化の柔軟性を提供し、マーケティング担当者が選択した統合を最大限に活用できるようにしています。

アドビは、プロバイダとの新しいプラットフォームをケースバイケースで展開する予定です。 詳しくは、[プログラムの詳細](https://www.marketo.com/why-marketo/partners/technology/)を参照するか、Marketoの担当者にお問い合わせください。
