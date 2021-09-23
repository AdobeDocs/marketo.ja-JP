---
unique-page-id: 13795395
description: リリースノート - 18年冬 - Marketo ドキュメント - 製品ドキュメント
title: リリースノート - 18年冬
exl-id: f08bdc91-86d3-4ea2-a74a-1398ed525bbb
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 18%

---

# リリースノート：18年冬 {#release-notes-winter}

18年冬リリースには、次の機能が含まれています。お客様のご契約により、制限やオプションの契約が必要なものがあります。詳細は担当の営業にお問い合わせください。

各機能の詳細な記事を表示するには、タイトルリンクをクリックしてください。**注意**:このリリースに含まれる機能の一部には、関連記事がありません。トピックに複数のサブ見出しが含まれる場合、リンクはそこに配置されます。

## キャンペーンのパフォーマンスとスループットの強化 {#campaign-performance-and-throughput-enhancements}

Marketoは、アドビのビッグデータアーキテクチャを活用して、トリガーキャンペーンのスループットを向上し、Webアクティビティの処理を改善し、オーディエンスのアクションにすばやく反応できるようにしています。

## MarketoのSalesforce CRM統合の機能強化 {#enhancements-to-marketo-s-salesforce-crm-integration}

Salesforce CRM統合には、次の2つの機能強化があります。

* [特定のCRM同](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications/notification-types.md) 期エラー（資格情報の期限切れ、APIの制限に達した、など）に関するMarketo管理者の通知

* [リード割り当て時にリー](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/turn-off-email-notifications-to-lead-owner.md) ド所有者への電子メール通知を無効にする機能

これらの改善は、2018年以降に公開される予定です。

## [Marketo パフォーマンスインサイト](/help/marketo/product-docs/reporting/performance-insights/performance-insights-overview.md) {#marketo-performance-insights}

>[!AVAILABILITY]
>
>パフォーマンスインサイトは、アドオン製品です。 見積もりについては、Marketoカスタマーサクセスマネージャーまたはアカウント担当者にお問い合わせください。

アトリビューション分析、インタラクティブなビジュアライゼーション、詳細データテーブルを使用して、キャンペーンとチャネルがビジネス結果に与える影響を調べます。

![](assets/image2018-2-5-7-3a55-3a46.png)

## アカウントベースのマーケティングの強化 {#account-based-marketing-enhancements}

**[ABM階層](/help/marketo/product-docs/target-account-management/target/named-accounts/tam-hierarchies.md)**

SalesforceまたはMicrosoft Dynamicsを使用するABMのお客様の場合、ABMはCRMで確立された親子関係を自動的に継承（および表示）するようになりました。 これらの関係は、ロールアップレポートとキャンペーンの実行の両方で使用できます。

## メールマーケティング {#email-marketing}

**[動的メールスクリプト](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md)**

Velocity のスクリプト記述が、動的コンテンツを使用するメールでサポートされました。速度とセグメント化ベースの動的コンテンツを組み合わせて、パーソナライズされたEメールを作成します。

**受信者タイムゾーン**

* **[毎月の育成サイクル](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)**:月次サイクルでプログラムの育成スケジュールを設定する機能を追加しました。

* **[配信を停止](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/abort-delivery-of-email-programs-scheduled-with-recipient-time-zone.md)**:残りの送信を中間実行で停止できるようになりました。

## 広告ネットワーク統合 {#ad-network-integrations}

**[Google カスタマーマッチ統合](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-google-customer-match-as-a-launchpoint-service.md)**

この統合により、Google AdWordsを使用してターゲット設定するMarketoオーディエンスをGoogleに送信し、YouTube、検索およびGmail全体でオーディエンスを再ターゲット化できます。

**[linkedIn Matched Audiences APIの機能強化](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-linkedin-matched-audiences-as-a-launchpoint-service.md)**

新しいLinkedIn APIにより、複数のLinkedIn Campaign ManagerアカウントにまたがってMarketoデータベース内のユーザーを再ターゲット化できるようになりました。

## Web パーソナライゼーション {#web-personalization}

**Webパーソナライゼーション用の日本語データソース**

Marketoでは、Web訪問者の識別（リバースIPルックアップ）や、日本からの訪問者のパーソナライゼーションを向上させるために、Webパーソナライゼーション用の日本語データソースを追加しています。 組織名は日本語で表示されます。

**[静的リストを使用したウェブセグメントの作成](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-segment-using-a-static-list.md)**

Webパーソナライゼーションで、マーケティングアクティビティ(MLM)で定義された静的リストに含まれる既知のWeb訪問者に対して、コンテンツをパーソナライズできるようになりました。 この機能強化により、チャネル間の静的リストにマーケティングし、Webサイト上のパーソナライズされたコンテンツを使用して、これらのリストの人をターゲットに設定できるようになりました。

## ContentAI {#contentai}

**予測アルゴリズムの改善**

Marketoで最適化されたContentAIアルゴリズムを通じて推奨されるコンテンツは、ランダムなコンテンツの最大2倍のクリック数を生成します。

## 統合 {#integration}

**[キャンペーン API の有効化/無効化](https://developers.marketo.com/rest-api/assets/campaigns/)**

この新しいAPIを使用すると、トリガーキャンペーンをリモートでアクティブ化および非アクティブ化でき、完全に自動化されたプログラムテンプレートを作成できます。 プログラムテンプレートを1回作成し、クローン作成、マーケティングコラテラルの更新を自動化し、スマートキャンペーンの有効化/スケジュール設定を自動化します。

## ToutApp {#toutapp}

**配信停止の更新**

2018年3月1日以降、[ToutApp.com](https://ToutApp.com)から（およびSalesforceの「Email with Tout」ボタンを使用して）送信されるすべての電子メールに、下部に登録解除リンクが追加されます。

**ライブフィードの更新**

「エンゲージメント」タブと「タスク」タブのルックアンドフィールを更新し、セールスメンバーがライブフィードから直接顧客のアクティビティに対応しやすく、迅速に対応できるようにしました。

**担当者詳細ビューの更新**

改善された人物詳細表示(PDV)では、ToutとSalesforce CRMの連絡先詳細を統合し、連絡先の包括的な表示を提供します。
