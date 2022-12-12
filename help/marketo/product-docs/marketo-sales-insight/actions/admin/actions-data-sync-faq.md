---
description: アクションデータ同期に関する FAQ - Marketo ドキュメント - 製品ドキュメント
title: アクションデータ同期に関する FAQ
exl-id: bb213d50-be22-492d-b74c-b8cfb834b2ca
source-git-commit: fbeb28b1b89fb329a4b45fb01dbad7df939ddc0c
workflow-type: ht
source-wordcount: '1050'
ht-degree: 100%

---

# アクションデータ同期に関する FAQ {#actions-data-sync-faq}

Sales Insight Actions のデータ統合フィールド同期を使用すると、Marketo Engage データベースから Sales Insight Actions データベースに個人情報を取り込むことができます。

これにより、Sales Insight Actions web アプリで最新の人物データを提供し、Marketo の対応する人物レコードと Salesforce のリード／取引先責任者／アカウント／商談レコードの一意の ID を収集できるので、レコードをログデータに正しく参照できます。

この同期は、Marketo Engage の「管理」セクションの「Sales Insight Actions 設定」タブで有効にできます。詳しくは、[データ同期の開始](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.md#initiate-data-sync)を参照してください。

![](assets/actions-data-sync-faq-1.png)

上の図は、人物アクティビティとタスクデータがシステム間でどのように同期されるのかを示しています。注意事項：

* 人物レコードは、Marketo Engage から Sales Insight Actions に同期され、Marketo Engage が Sales Insight Actions の人物データの信頼できる情報源となります。
* Marketo Engage と Sales Insight Actions どちらにも、Salesforce への配信停止ステータスの収集と同期を行う[仕組みがあります](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md)。
* 配信停止ステータスはセールスのアクションから Marketo Engage に同期されませんが、[Marketo 配信停止チェック](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md)を使用して販売者にメールの送信を許可する前に、人物の Marketo 配信停止ステータスを確認するように Sales Insight Actions を設定できます。

データ統合同期の仕組みに関するよくある質問を以下に示します。

## Sales Insight Actions に同期されるリード／取引先責任者は何ですか？ {#what-lead-contacts-are-synced}

![](assets/actions-data-sync-faq-2.png)

セールス所有者が割り当てられているリードと取引先責任者が、セールスのアクションに同期されます。

リード／取引先責任者に Salesforce 内のセールス所有者が存在するかどうかを確認するには、存在する標準所有者フィールドを確認します。

セールス所有者は、Marketo 同期ユーザや、特定の Salesforce またはセールスユーザである必要はありません。必要なのは、Salesforce のリード所有者と取引先責任者所有者フィールドにユーザがリストされていることだけです。これにより、リードとして識別して Sales Insight Actions に同期できます。同期するフィールドが更新されると、Sales Insight Actions でも検出され、更新されます。

## Sales Insight スマートグリッドに表示されるアクティビティデータは、どこから入手されるのですか？ {#where-does-the-activity-data-get-sourced-from}

![](assets/actions-data-sync-faq-3.png)

メール、電話、注目のアクション、web などのアクティビティデータは、すべて Marketo Engage のデータベースから取得されます。セールスユーザが Sales Insight スマートグリッドを読み込むたびに、Marketo Engage インスタンスに対してデータを取得するリクエストが行われます。

![](assets/actions-data-sync-faq-4.png)

すべてのアクティビティデータを Marketo Engage から取得できるように、Sales Insight Actions はすべてのアクティビティデータを Marketo Engage に同期します。

## 人物レコードに関連するどのフィールドが、Marketo Engage から Sales Insight Actions に同期されるのですか？ {#what-fields-sync}

Marketo Engage から Sales Insight Actions に同期するフィールドは 11 個あります。

* 名
* 姓
* Salesforce 取引先責任者 ID
* Salesforce リード ID
* Salesforce アカウント ID
* Salesforce 商談 ID
* Marketo ID
* 会社
* 職位
* メール
* 電話番号
* Linkedin URL
* ソース

## Marketo Engage と Sales Insight Actions の間で同期するフィールドは設定可能ですか？ {#are-the-fields-that-sync-configurable}

Sales Insight Actions に同期する Marketo Engage フィールドの設定は使用できず、フィールドをマッピングする機能も使用できません。Marketo からの同期では、標準の Marketo フィールドが、セールスアクションのインスタンスの標準フィールドに自動的にマッピングされます。

## Sales Insight Actions に独自のデータベースがあるのはなぜですか？ {#why-does-actions-have-its-own-database}

Sales Insight Actions には、個人およびアクティビティデータベースを備えた専用の web アプリケーションがあり、セールスチーム向けに構築および設計して最適化したワークスペースが提供されます。これにより、セールス管理者と販売者は、マーケティングオペレーションスペシャリスト向けに最適化された、プライマリ Marketo Engage ワークスペースにアクセスや権限を付与することなく、エンゲージメント戦略を構築し、管理するスペースを確保できます。

## 重複はどのように処理されますか？ {#how-are-duplicates-handled}

セールスアクションのデータベースは、Marketo Engage データベースに存在する条件を満たした人物（セールス所有者を持つリード／取引先責任者）の複製になります。つまり、Marketo で同じメールアドレスを持つ 2 つのレコードが作成された場合、セールスアクションで重複レコードが作成されます。

## 初期同期が完了するまでにどのくらい時間がかかりますか？ {#how-long-initial-sync}

すべてのセールスリードデータを新しい Sales Insight Actions インスタンスに同期する最初のプロセスでは、通常、1～2 分ごとに約 1,000 件の人物が処理されます。これは単なる推定であり、状況によって異なる場合があります。

初期同期が実行され、すべてのセールスリードが Sales Insight Actions web アプリインスタンスに入力されると、同期されるサポート対象フィールドの 1 つが更新されるたびに増分同期が実行されます。

## Sales Insight Actions ユーザは Actions web アプリから人物データを編集できますか？ {#can-actions-users-edit-people-data}

いいえ。Actions web アプリのユーザも管理者も Actions で人物レコードを作成および編集する機能を使用できません。人物の作成と編集は、Salesforce または Marketo Engage で行う必要があります。Sales Insight Actions は、新しいデータを継続的に同期することで、Marketo を人物データの信頼できる情報源として使用します。したがって、Marketo のワークフローからまたは Salesforce から同期した人物が Marketo で更新または作成されると、その更新が Sales Insight Actions web アプリデータベースに渡されます。

## セールスアクティビティは Marketo に記録されますか？ {#do-sales-activities-log-to-marketo}

はい、セールスエンゲージメントアクティビティは、ネイティブアクティビティとして Marketo に記録されます。また、これらのアクティビティには、セールスアクティビティ属性に基づいてリードをターゲット設定するための制約と共に使用できるネイティブフィルターも含まれます。

![](assets/actions-data-sync-faq-5.png)

以下に、Marketo に記録されるアクティビティのリストを示します。

* セールスメールを送信
* セールスメール開封
* セールスメールクリック
* セールスメールに返信
* セールスメールバウンス
* セールス電話受信
* セールスキャンペーンに追加
* セールスキャンペーンから削除

## セールスアクティビティは Salesforce に記録されますか？ {#do-sales-activities-log-to-salesforce}

はい、セールスエンゲージメントアクティビティは、ネイティブタスクとして Salesforce に記録されます。これらのタスクを Salesforce レポートで使用して、セールスアクティビティを追跡するチームダッシュボードを強化できます。

Sales Insight Actions を使用すると、管理者は、Salesforce にログに記録するセールスアクティビティを設定できます。これらのアクティビティには、メール、電話、開封リマインダータスクが含まれます。

![](assets/actions-data-sync-faq-6.png)

上の図は、Salesforce にログに記録される情報を示しています。メールや電話などのアクティビティは、Salesforce に[一方向同期](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md)で記録されます。[配信停止](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md)および[リマインダータスク](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md)は双方向同期で最新の状態に保たれます。これらの各データ同期は、Sales Insight Actions web アプリインターフェイスから設定できます。

>[!MORELIKETHIS]
>
>* [Salesforce との配信停止の同期](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md)
>* [Marketo 配信停止チェック](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md)
>* [Salesforce 同期設定](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md)
>* [Salesforce とのリマインダータスク同期](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md)
>* [データ同期の開始](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.md#initiate-data-sync)

