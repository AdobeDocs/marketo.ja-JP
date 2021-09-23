---
unique-page-id: 17727823
description: リリースノート - 19年冬 - Marketo ドキュメント - 製品ドキュメント
title: リリースノート - 19年冬
exl-id: 0cb3b3a1-472e-41d4-84f4-47f06e65017c
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '1109'
ht-degree: 6%

---

# リリースノート：19年冬 {#release-notes-winter}

19年冬リリースには、次の機能が含まれています。お客様のご契約により、制限やオプションの契約が必要なものがあります。詳細は担当の営業にお問い合わせください。

各機能の詳細な記事がある場合は、タイトルリンクをクリックして表示してください。

>[!NOTE]
>
>Facebookでカスタムオーディエンスの統合を活用するには、Business Managerアカウントが必要になりました。 facebook LaunchPointサービス&#x200B;*をBusiness Managerアカウントに関連付ける必要があります。関連付けないと、2019年1月14日&#x200B;**以降、統合が機能しなくなります。*** Business Managerアカウントを設定するには、[Facebookのヘルプ](https://www.facebook.com/business/help/1710077379203657)を参照してください。

>[!NOTE]
>
>Microsoftは、すべてのオンラインユーザーに対して、最新バージョンのMicrosoft Dynamicsへのアップグレードを求めています。 MarketoインスタンスをDynamics Onlineと統合する場合は、統合が引き続き機能するように、[Marketoソリューションの最新バージョン](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md)を&#x200B;**2019年1月31日より前に**&#x200B;アップグレードする必要があります。

>[!NOTE]
>
>Marketoは、GoToWebセミナーのOAuthバージョンを1.0から2.0にアップグレードしています。OAuth 1.0のサポートは、2019年1月に廃止されます。 GoToWebセミナーをご利用のお客様は、統合が引き続き機能するよう、**2019年1月31日(PT)までに（管理領域で）LaunchPointを通じてログインを再認証する必要があります。**&#x200B;詳しくは、[コミュニティページ](https://nation.marketo.com/docs/DOC-6739-gotowebinar-authentication-change-take-action-before-1312019)を参照してください。

## 主要プラットフォームの機能拡張 {#core-platform-enhancements}

**[Marketo Eメール用のEメールCC](/help/marketo/product-docs/email-marketing/general/email-cc.md)**

Marketo を通じて送信するメールは、受信者あたり 5 件までの CC アドレスを含めることができます。

**API**

* **Asset APIのマルチブランディングドメインのサポート：** APIとUIで同じ結果が得られます。
* **アセットAPIの電子メールCCサポート**:APIを使用してEメールをコピー、承認、処理するユーザーは、UI設定と同等の性能を維持します。

**[Munchkin v155（ベータ版）](https://developers.marketo.com/javascript-api/lead-tracking/configuration/)**

* **APIのみのモード**:Marketoの自動追跡に依存する代わりに、単一ページのWebアプリからWebページの訪問を記録するタイミングを明示的に呼び出すことで、データベースのメンバーを追跡するタイミングと方法を判断できるようになりました。
* **オプトアウト管理**:オプトアウトCookieドメインをMunchkinトラッキングCookieドメインと照合することで、オプトアウトを簡単に管理できます。
* **ドメインレベルのデシダーパラメーター**:2文字のドメイン(「  [webサイト.io](https://website.io) 」)は、追加の設定要件なしで、Marketoで自動的に追跡されます。

## Marketo セールスエンゲージ {#marketo-sales-engage}

* **Salesforceカスタムプロファイル**:Sales Engageが無制限のカスタムプロファイルをサポートするようになりました。

* **Salesforceのカスタマイズ**:重要でないカスタムアクティビティフィールドを削除することで、ユーザーは、CRMプラットフォームでのSales Engageをより効率的に設定できます。
* **Eメールサービス**:Microsoft Outlookに接続する（Office365または「Eメール接続」タブのオンプレミス）ことで、配信品質の向上に加え、返信トラッキング、スケジュール済みEメール機能の向上、および一括Eメール機能を利用できます。
* **新しい管理設定**:Sales Engageインスタンスを最適化するための2つの管理ページが追加されました。

   * _チーム管_ 理では、管理者が購読とチームを編集できるので、シームレスなアカウント設定プロセスがサポートされます。
   * _Salesforce Admin Settingshelpsチー_ ムは、SFDC同期を以前よりも高速かつ簡単に設定します。

* **Windows用OWAプラグイン**:1つのアドインで、すべてのWindows Office365クライアントがSales Engageでサポートされ、Outlookでライブフィードを使用できます。新しいプラグインは、Microsoftストアで入手できます。
* **アクティビティプッシャー**:販売の同期コアMarketoプラットフォームにエンゲージメントして、リアルタイムマーケティングの洞察を活用します。

## Marketo Sky {#marketo-sky}

>[!NOTE]
>
>Marketo Skyリリースは、より頻繁に発生します。 第1四半期の下旬に、次の機能および機能強化がリリースされる予定です。 詳細と更新については、[Skyのドキュメント](https://help.marketo.com/)を参照してください。

* **オプションのデフォルトエクスペリエンス**:Marketoユーザーは、Marketo Skyが管理者からアクセス権を付与されている場合、ユーザーをデフォルトエクスペリエンスとして設定できます。

* **Reigined My Marketo**:最も頻繁に訪問される領域に重要な情報、通知、リンクを提供するウィジェットを追加して、エクスペリエンスをカスタマイズします。

* **Design Studioリストビューと詳細ページ**:Eメール、ランディングページ、フォームのフィルタリング可能で検索可能なリスト表示で、組織と精度を向上させます。アセットの詳細ページには、アセットが使用するプログラム、使用するスニペットの数など、各アセットに関する重要な情報が表示されます。

* **グローバル検索**:Marketoは、プラットフォーム全体でより高速で堅牢なグローバル検索機能を提供します。検索クエリが、アクセス可能なすべてのワークスペースで実行され、アセット（アクティブとアーカイブの両方）、ラベル、キャンペーン、プログラムを検索できるようになりました。 検索結果はオーバーレイを介して提供され、各結果にはアセットの保存場所を指定するファイルの場所の追跡情報が含まれます。

* **ユーザーインターフェイスの改善**:新しいアイコン、モダル、ボタン、および新しいカラーパレットを追加し、ブランドの更新を反映し、Marketo Skyをさらに美しく機能させます。

* **電子メールプログラムのユーザビリティの強化**:アドビでは、従来のMarketoリード管理プラットフォームと新しいMarketo Sky体験との間で、引き続きEメールプログラムの機能を同等にしています。
* **イベントとウェビナーのプログラム**:イベントとウェビナーのプログラムがMarketo Skyで利用できるようになりました(注意：このリリースでは、GoToWebセミナーのみがサポートされます。これは、時間の経過と共にさらなる統合が確立されるものです)。

## アカウントベースドマーケティング {#account-based-marketing}

**[ABMのペルソナベースのセグメント化とフィルタリング](/help/marketo/product-docs/target-account-management/using-personas.md)**

名前付きアカウント内の特定のペルソナに合わせてABMキャンペーンをパーソナライズする。 ABMのペルソナ機能は、リードのセグメント化に基づいてデフォルトの役職を作成し、追加のペルソナのセグメント化を設定できます。

## アナリティクス {#analytics}

**Bizible**

* **カスタム計算フィールド**:任意のBizible属性を使用して、ダッシュボードのレポートとセグメント化に使用できるカスタムフィールドを作成します。

* **SOC II Type II認定**:新しいセキュリティとプライバシーの認定は、今年初めからType Iの認定に基づいて構築されます。

## Web パーソナライゼーション {#web-personalization}

**[アカウント設定にサブドメインを追加](/help/marketo/product-docs/web-personalization/getting-started/workspaces-in-web-personalization.md)**

ドメインとサブドメインをより効率的に管理するために、ユーザーは、RTPアカウント設定にサブドメインを追加できるようになりました。

## Marketo モバイルエンゲージメント（MME） {#marketo-mobile-engagement-mme}

**Android向けMMEソフトウェア開発キット(SDK)の更新**

Android向けSDKを、より柔軟性と新しいエンジニアリング機能を含む、より新しく、安定した、拡張性の高いフレームワークに更新しました。 Androidアプリ開発者は、この新しいSDKでGoogleの[Firebase Cloud Messaging](https://firebase.google.com/docs/cloud-messaging/)(FCM)を直接使用できるようになりました。

* [開発者向けの手順](https://developers.marketo.com/mobile/installation/#android_adding_fcm_to_your_application)
* [開発者向けFAQ](https://developers.marketo.com/mobile/installation/#android_fcm_faq)

>[!NOTE]
>
>アプリ開発者は、2019年3月31日より前に、新しいバージョンに&#x200B;**更新する必要があります。** 2019年3月31日までにSDKを更新しない場合、この日以降にアプリをダウンロードした新しいユーザーは、最新バージョンのSDKに更新するまでプッシュ通知を受け取れません。 SDKの更新では、現在のモバイルアプリユーザーが新しいバージョンのアプリを再ダウンロードする必要はありません。

## その他の更新 {#additional-updates}

**拡張可能なウェビナープラットフォーム**

アドビのパートナーチームは、製品リリースに加えて、WebセミナープロバイダーがMarketoとの独自の統合を構築および維持できる新しいフレームワークに取り組み、ソリューションの更新と強化を柔軟に提供しながら、マーケターが選択した統合を最大限に活用できます。

アドビでは、プロバイダーとの間で新しいプラットフォームをケースバイケースで展開する予定です。 詳しくは、[プログラムの詳細](https://www.marketo.com/why-marketo/partners/technology/)を参照するか、Marketoの担当者にお問い合わせください。
