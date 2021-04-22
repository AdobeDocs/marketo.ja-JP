---
unique-page-id: 17727823
description: リリースノート — Winter 19 -Marketoドキュメント — 製品ドキュメント
title: リリースノート — Winter '19
exl-id: 0cb3b3a1-472e-41d4-84f4-47f06e65017c
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '1109'
ht-degree: 3%

---

# リリースノート：冬&#39;19 {#release-notes-winter}

Winter 19リリースには、次の機能が含まれています。 Marketo版で利用可能な機能を確認してください。

タイトルリンクをクリックすると、各機能の表示の詳細記事が表示されます（ある場合）。

>[!NOTE]
>
>現在、facebookでは、カスタムオーディエンス統合を利用するためにBusiness Managerアカウントが必要です。 facebookLaunchPointサービス&#x200B;*をBusiness Managerアカウントに関連付ける必要があります*。関連付けが行われないと、2019年1月14日&#x200B;**以降、統合は機能しなくなります。** Business Managerアカウントを設定するには、[Facebookのヘルプ](https://www.facebook.com/business/help/1710077379203657)を参照してください。

>[!NOTE]
>
>Microsoftは、すべてのオンラインユーザーに対して、最新バージョンのMicrosoft Dynamicsへのアップグレードを要求しています。 MarketoインスタンスをDynamics Onlineと統合する場合、統合が引き続き機能するように、**2019年1月31日**&#x200B;の前に、Marketoソリューション](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md)の最新バージョンに[アップグレードする必要があります。

>[!NOTE]
>
>Marketoは、GoToWebinarのOAuthバージョンを1.0から2.0にアップグレードしています。OAuth 1.0のサポートは2019年1月に廃止されます。 GoToWebセミナーのお客様は、統合が引き続き機能するように、LaunchPoint（管理領域の）を使用して&#x200B;**2019年1月31日**&#x200B;までに再認証する必要があります。 詳しくは、[コミュニティページ](https://nation.marketo.com/docs/DOC-6739-gotowebinar-authentication-change-take-action-before-1312019)を参照してください。

## 主要プラットフォームの機能拡張 {#core-platform-enhancements}

**[Marketo電子メール用電子メールCC](/help/marketo/product-docs/email-marketing/general/email-cc.md)**

Marketo を通じて送信するメールは、受信者あたり 5 件までの CC アドレスを含めることができます。

**API**

* **アセットAPIのマルチブランドドメインのサポート：アセットの** 承認と複製は、APIとUIで同じ結果になります。
* **Asset APIの電子メールCCサポート**:APIを使用した電子メールの複製、承認、および処理を行うユーザーは、UI設定と同一性を維持します。

**[Munchkin v155（ベータ版）](https://developers.marketo.com/javascript-api/lead-tracking/configuration/)**

* **APIのみのモード**:ユーザーは、Marketoの自動追跡に依存する代わりに、単一ページのWebアプリで、Webページの訪問を記録するタイミングを明示的に呼び出すことで、データベースのメンバーを追跡するタイミングと方法を決定できるようになりました。
* **オプトアウト管理**:オプトアウトcookieドメインをMunchkin追跡cookieドメインと一致させることで、オプトアウトを簡単に管理できます。
* **Domain-Level Decider Parameter**:2文字のドメイン(例：&quot;  [website.io](https://website.io)&quot;)は、追加のセットアップ要件なしに、自動的にMarketoで追跡されます。

## Marketo セールスエンゲージ {#marketo-sales-engage}

* **Salesforceカスタムプロファイル**:Sales Engageは、無制限のカスタムプロファイルをサポートするようになりました。

* **Salesforceのカスタマイズ**:重要でないカスタムアクティビティのフィールドを削除すると、CRMプラットフォームにSales Engageをより効率的に設定できます。
* **Email Service**:Microsoft Outlookに（[電子メール接続]タブのOffice365またはOn-Prem経由で）接続することで、配信品質と、返信追跡機能、スケジュール済みの電子メール機能、およびバルク電子メール機能が向上しました。
* **新しい管理設定**:Sales Engageインスタンスを最適化する2つの管理ページが追加されました。

   * _チーム_ 管理では、管理者が購読やチームを編集できるようにすることで、シームレスなアカウント設定プロセスをサポートしています。
   * _Salesforce管理者_ 設定シェルプチームは、SFDC同期を以前に比べて迅速かつ容易に設定します。

* **OWA Plugin for Windows**:1つのアドインを1つ追加すると、Windows Office 365のすべてのクライアントがSales Engageでサポートされ、Outlookでライブフィードを使用できます。新しいプラグインがMicrosoft Storeで入手できます。
* **アクティビティプッシャー**:販売を同期してコアMarketoプラットフォームに関与させ、リアルタイムのマーケティングインサイトを活用します。

## Marketo Sky {#marketo-sky}

>[!NOTE]
>
>Marketo Skyリリースは、より頻繁に行われます。 第4四半期前半には、以下の機能および機能強化がリリースされる予定です。 詳細と更新情報については、[Skyのドキュメント](https://help.marketo.com/)を参照してください。

* **デフォルトエクスペリエンス**（オプション）:Marketoのユーザーは、管理者からアクセス権を与えられた場合、Marketo Skyをデフォルトのエクスペリエンスとして設定できます。

* **私のMarketo**:重要な情報、通知、最も頻繁に訪問される領域へのリンクを提供するウィジェットを追加して、エクスペリエンスをカスタマイズします。

* **Design Studioリスト表示と詳細ページ**:電子メール、ランディングページ、フォームのフィルタリングおよび検索が可能なリスト表示により、組織と正確性のレベルを高めます。アセットの詳細ページには、アセットが使用されているプログラム、使用されているスニペットの数など、各アセットに関する主な情報が表示されます。

* **グローバル検索**:Marketoは、プラットフォーム全体で、より高速でより強力なグローバル検索機能をオファーします。検索クエリは、アクセス可能なすべてのワークスペースに対して実行でき、アセット（アクティブとアーカイブの両方）、ラベル、キャンペーン、プログラムを検索できるようになりました。 検索結果はオーバーレイを介して提供され、各結果にはアセットの居住地を指定するファイルの場所のトレールが含まれます。

* **ユーザーインターフェイスの強化**:新しいアイコン、モデル、ボタン、および新しいカラーパレットに加え、ブランドの刷新を反映し、Marketo Skyをより魅力的で機能的にします。

* **電子メールプログラムのユーザビリティの強化**:従来のMarketoリード管理プラットフォームと新しいMarketo Skyエクスペリエンスの間で、電子メールプログラム機能の統一に向けて、引き続き努力していきます。
* **ウェビナーを使用するイベントプログラム**:ウェビナーイベントプログラムは、Marketo Skyで利用できるようになりました(注意：このリリースではGoToWebinarのみサポートされ、時間の経過とともに確立される統合が追加されます)。

## アカウントベースドマーケティング {#account-based-marketing}

**[ABM Personaベースのセグメント化とフィルタリング](/help/marketo/product-docs/target-account-management/using-personas.md)**

名前付きアカウント内の特定の個人に合わせてABMキャンペーンをパーソナライズします。 ABM Persona機能は、リードのセグメント化に基づいてデフォルトの役職を作成し、追加のパーソナルセグメントを設定できます。

## アナリティクス {#analytics}

**Bizible**

* **カスタムの計算フィールド**:任意のBizible属性を使用して、ダッシュボードのレポートとセグメント化に使用できるカスタムフィールドを作成します。

* **SOC II Type II認定**:セキュリティとプライバシーに関する新しい認定は、今年の初めからType I認定に基づいて行われます。

## ウェブパーソナライゼーション {#web-personalization}

**[アカウント設定にサブドメインを追加](/help/marketo/product-docs/web-personalization/getting-started/workspaces-in-web-personalization.md)**

ドメインとサブドメインをより効率的に管理するために、ユーザーはRTPアカウント設定にサブドメインを追加できるようになりました。

## Marketoモバイルエンゲージメント(MME) {#marketo-mobile-engagement-mme}

**Android向けMMEソフトウェア開発キット(SDK)の更新**

Android向けSDKは、より柔軟性と新しいエンジニアリング機能を備えた、よりモダンで安定性と拡張性の高いフレームワークに更新されました。 Androidアプリの開発者は、Googleの[Firebase Cloud Messaging](https://firebase.google.com/docs/cloud-messaging/)(FCM)をこの新しいSDKで直接使用できるようになりました。

* [開発者向けの手順](https://developers.marketo.com/mobile/installation/#android_adding_fcm_to_your_application)
* [開発者向けFAQ](https://developers.marketo.com/mobile/installation/#android_fcm_faq)

>[!NOTE]
>
>アプリ開発者&#x200B;**は、2019年3月31日までに新しいバージョンに更新する必要があります。** 2019年3月31日までにSDKを更新しない場合、この日以降にアプリをダウンロードした新規ユーザーは、最新バージョンのSDKに更新するまでプッシュ通知を受信できません。 SDKの更新では、現在のモバイルアプリユーザーが新しいバージョンのアプリを再ダウンロードする必要はありません。

## 追加の更新{#additional-updates}

**拡張可能なウェビナープラットフォーム**

製品リリースに加えて、パートナーチームは、ウェビナープロバイダーがMarketoとの連携を構築し維持できる新しいフレームワークに取り組み、ソリューションの更新と強化に柔軟性を提供し、マーケティング担当者が選択した統合を最大限に活用できるようにしています。

アドビは、プロバイダとの新しいプラットフォームをケースバイケースで展開する予定です。 詳しくは、[プログラムの詳細](https://www.marketo.com/why-marketo/partners/technology/)を参照するか、Marketoの担当者にお問い合わせください。
