---
unique-page-id: 12983280
description: リリースノート — 17年秋 — Marketto Docs — 製品ドキュメント
title: リリースノート — 17年秋
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 0%

---


# リリースノート：秋17 {#release-notes-fall}

2017年秋のリリースには、次の機能が含まれています。 Marketing Editionで機能が使用できるかどうかを確認します。

タイトルリンクをクリックすると、各機能に関する表示の詳細記事が表示されます。 注意：このリリースに含まれる一部の機能には、関連記事がありません。 トピックに複数のサブ見出しが含まれる場合は、そこにリンクが配置されます。

## システムの信頼性 {#system-reliability}

優れた配列決定、不一致の減少、マンチキンの安定性の向上など、Marketoの中核インフラストラクチャに対してさらに改善を行っています。

## SFDC同期のパフォーマンス {#sfdc-sync-performance}

MarketoとSalesforceの豊富で高速な同期を利用できます。 アカウントまたはリードで一括更新を必要とするデータの変更は、バックログを避けるために並列キューに分割できます。 また、イベントとタスクの同期が最大50%高速化されました。

## Analyticsのパフォーマンス改善 {#analytics-performance-improvements}

最近のインフラストラクチャの強化オファーにより、Marketorのレポートおよび分析ツール内でアップタイムと安定性が向上し、アドホックレポートをより迅速に作成できるようになりました。

## [受信者タイムゾーン](https://docs.marketo.com/x/_xvG) {#recipient-time-zone}

この新機能により、ローカルタイムゾーンに従って電子メールを保持し、配信できるようになりました。 電子メールおよびエンゲージメントのプログラムは、受信者のタイムゾーンに配信されるように設定でき、複数のプログラムを作成する必要がなくなります。1回送信すると、Marketorはローカルの正しい時間まで電子メールを自動的に保持します。 電子メール指標を上昇させ、ローカルの慣行を観察し、グローバルに単一のプログラムを使用して時間を節約します。

![](assets/image2017-11-29-8-3a45-3a47.png)

>[!NOTE]
>
>電子メールおよびエンゲージメントプログラムで受信者のタイムゾーンをまだ有効にできない場合は、パニックに陥らないでください。 この機能は、すべてのお客様に対して徐々に有効になっています。

## [セグメント別サンプル電子メールの確認](https://docs.marketo.com/x/2IER) {#review-sample-emails-by-segment}

Marketorには、レビュー用にサンプル電子メールを送信する際に、セグメントを選択する新しいオプションが追加されました。 リードが属するセグメントを手動で判断する必要がなくなり、動的なコンテンツを含む電子メールを様々なセグメントに簡単に送信できるようになりました。

## [LinkedInのリードジェネレーションに関するカスタム質問](https://docs.marketo.com/x/ngLG) {#linkedin-lead-gen-custom-questions}

LinkedInのリードジェネレーションフォームをカスタマイズして、カスタムのリード属性を収集します。 1つのフォームにつき最大3つのカスタム質問を尋ねたり、1行のテキスト入力または複数選択の質問から選択したり、Marketorのリードフィールドにマッピングしたりできるようになりました。

## [Slack統合](../../product-docs/administration/additional-integrations/add-slack-as-a-launchpoint-service.md) {#slack-integration}

新しいSlack統合の一環として、次の2つの機能をリリースしました。

* システム通知：現在のキャンペーンのステータスや、直ちに対処する必要のある問題に関するアラートなど、Marketorインスタンスの重要なイベントに関するSlack通知を取得します。
* 興味深い瞬間：Marketon Insightが営業アカウントから既知の個人によってトリガーされた場合、リードの所有者にはSlackを介して通知できます。 通知には、リード情報と営業アカウントに関する詳細が含まれます。

## ABMの強化 {#abm-enhancements}

**連絡先のないアカウント [を表示](https://docs.marketo.com/x/fKCt)**

Marketto ABMは、連絡先のないCRMアカウントを同期して表示するようになりました。 事前の販売またはマーケティング履歴のない新しいアカウントを含め、後続のリードをアカウントに照合して進行状況を追跡します。

## ContentAnalytics`<sup>AI </sup>`{#contentai-analytics}

** [新しいABMアカウントリストフィルタ](https://docs.marketo.com/x/1BPG) **

ABMアカウントリスト全体でコンテンツの表示と比較を行い、既存のコンテンツを最適化します。 コンテンツ`<sup>AI</sup>` :

* 閲覧されたコンテンツのトップ
* トップコンバージョンコンテンツ
* マーケティングアクティビティ向けのAIベースの推奨コンテンツ

## ウェブパーソナライゼーションの強化 {#web-personalization-enhancements}

** [Tokens for Webキャンペーン](https://docs.marketo.com/x/SwJI)**

Webキャンペーンー内でトークンを使用できるようになりました。 トークンを利用して、パーソナライズされたメッセージやコンテンツを配信し、Webキャンペーンーへの関与を増やします。

![](assets/image2017-11-16-11-3a25-3a7.png)

** [Design StudioイメージをWebキャンペーンエディターに表示](https://docs.marketo.com/x/SwJI)**

クリエイティブなアセットや画像をMarketor内の複数のチャネルで再利用することで、時間を節約できます。

![](assets/image2017-11-16-11-3a26-3a10.png)

## 統合  {#integration}

** [電子メールプレビューAPI](https://developers.marketo.com/rest-api/assets/emails/)**

Marketoの外部で電子メールをリモートプレビューできるようになり、電子メールコンテンツローカライゼーションのプロセスが簡素化され、エラーが減少します。

** [Replace HTML API](https://developers.marketo.com/rest-api/assets/emails/)**

開発者は、電子メールアセットのHTMLコンテンツをリモートで更新でき、単一のシステム内でアセットを管理できるようになります。
