---
description: アクションデータ同期に関する FAQ - Marketo ドキュメント - 製品ドキュメント
title: アクションデータ同期に関する FAQ
feature: Sales Insight Actions
exl-id: bb213d50-be22-492d-b74c-b8cfb834b2ca
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '958'
ht-degree: 41%

---

# アクションデータ同期に関する FAQ {#actions-data-sync-faq}

[!DNL Sales Insight Actions] のデータ統合フィールド同期により、Marketo Engage データベースから [!DNL Sales Insight Actions] データベースに個人情報を取り込むことができます。

これにより、[!DNL Sales Insight Actions] web アプリに最新の人物データが提供され、Marketoの対応する人物レコードと [!DNL Salesforce] のリード/連絡先/アカウント/商談レコードの一意の ID を収集できるので、レコードをログデータから適切に参照できます。

この同期は、Marketo Engageの「管理者」セクションの「[!DNL Sales Insight Actions] 設定」タブで有効にすることができます。 詳しくは、[データ同期の開始](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.md#initiate-data-sync)を参照してください。

![](assets/actions-data-sync-faq-1.png)

上の図は、人物アクティビティとタスクデータがシステム間でどのように同期されるのかを示しています。注意事項：

* 人物レコードはMarketo Engageから [!DNL Sales Insight Actions] に同期されるので、Marketo Engageは [!DNL Sales Insight Actions] 人の人物データの情報源になります
* Marketo Engageと [!DNL Sales Insight Actions] の両方 [ には、登録解除ステータスを収集して ](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md) に同期するメカニズムが [!DNL Salesforce] あります）
* 登録解除ステータスは、セールスアクションとMarketo Engageが同期しま [!DNL Sales Insight Actions] んが、[Marketo登録解除チェック ](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md) 付きのメールをセラーが送信できるようにする前に、Marketoのユーザーの登録解除ステータスを確認するように設定できます。

データ統合同期の仕組みに関するよくある質問を以下に示します。

## どのリード/連絡先が [!DNL Sales Insight Actions] に同期されますか？ {#what-lead-contacts-are-synced}

![](assets/actions-data-sync-faq-2.png)

セールス所有者が割り当てられているリードと連絡先が、Sales Actions に同期されます。

存在する標準の所有者フィールドを調べることで、リード/連絡先に [!DNL Salesforce] の販売所有者がいるかどうかを確認できます。

営業オーナーは、Marketo sync user または特定の [!DNL Salesforce] ーザーや営業ユーザーである必要はありません。 必要なのは、[!DNL Salesforce] にリストされているリードオーナーおよびコンタクトオーナーのフィールドにユーザーが表示されることで、それをセールスリードとして識別して [!DNL Sales Insight Actions] に同期できます。 同期するフィールドへの更新も [!DNL Sales Insight Actions] で検出され、更新されます。

## Sales Insight スマートグリッドに表示されるアクティビティデータは、どこから入手されるのですか？ {#where-does-the-activity-data-get-sourced-from}

![](assets/actions-data-sync-faq-3.png)

メール、電話、注目のアクション、web などのアクティビティデータは、すべて Marketo Engage のデータベースから取得されます。セールスユーザーが Sales Insight スマートグリッドを読み込むたびに、Marketo Engage インスタンスに対してデータを取得するリクエストが行われます。

![](assets/actions-data-sync-faq-4.png)

すべてのアクティビティデータをMarketo Engageから取得できるように、[!DNL Sales Insight Actions] ではすべてのアクティビティデータをMarketo Engageに同期します。

## 人物レコードに関連するフィールドで、Marketo Engageから [!DNL Sales Insight Actions] に同期されるものはどれですか？ {#what-fields-sync}

Marketo Engageから [!DNL Sales Insight Actions] に同期されるフィールドは 11 個あります。

* 名
* 姓
* [!DNL Salesforce] 連絡先 ID
* [!DNL Salesforce] リード ID
* [!DNL Salesforce] アカウント ID
* [!DNL Salesforce] オポチュニティ ID
* Marketo ID
* 会社
* 職位
* メール
* 電話番号
* [!DNL Linkedin] URL
* ソース

## Marketo Engageと [!DNL Sales Insight Actions] の間で同期されるフィールドは設定可能ですか。 {#are-the-fields-that-sync-configurable}

Marketo Engageのフィールドを [!DNL Sales Insight Actions] に同期するように設定することも、フィールドをマッピングする機能も使用できません。 Marketo からの同期では、標準の Marketo フィールドが、セールスアクションのインスタンスの標準フィールドに自動的にマッピングされます。

## [!DNL Sales Insight Actions] に独自のデータベースがあるのはなぜですか？ {#why-does-actions-have-its-own-database}

[!DNL Sales Insight Actions] には専用のユーザーとアクティビティデータベースを持つ独自の web アプリケーションがあり、販売チーム向けに構築および設計された最適化されたワークスペースを提供します。 これにより、セールス管理者と販売者は、マーケティングオペレーションスペシャリスト向けに最適化された、プライマリ Marketo Engage ワークスペースにアクセスや権限を付与することなく、エンゲージメント戦略を構築し、管理するスペースを確保できます。

## 重複はどのように処理されますか？ {#how-are-duplicates-handled}

Sales Actions データベースは、Marketo Engage データベースに存在する、条件を満たした人物（セールス所有者を持つリード／連絡先）のコピーになります。つまり、Marketo で同じメールアドレスを持つ 2 つのレコードが作成された場合、Sales Actions で重複レコードが作成されます。

## 初期同期が完了するまでにどのくらい時間がかかりますか？ {#how-long-initial-sync}

すべてのセールス・リード・データを新しい [!DNL Sales Insight Actions] インスタンスに同期する初期プロセスでは、通常、1～2 分ごとに約 1,000 人のスタッフが処理されます。 これは単なる推定であり、状況によって異なる場合があります。

最初の同期を実行し、すべての営業リードが [!DNL Sales Insight Actions] web アプリインスタンスに入力されると、同期されるサポート対象フィールドの 1 つに対して更新が行われるたびに増分同期が実行されます。

## ユーザー [!DNL Sales Insight Actions]Actions web アプリから人物データを編集できますか？ {#can-actions-users-edit-people-data}

いいえ。Actions web アプリのユーザーも管理者も Actions で人物レコードを作成および編集する機能を使用できません。ユーザーの作成と編集は、[!DNL Salesforce] またはMarketo Engageで行う必要があります。 [!DNL Sales Insight Actions] は、Marketoを人物データの信頼できるソースとして使用し、新しいデータを継続的に同期します。そのため、Marketoのワークフローから、または [!DNL Salesforce] から同期されて、Marketoで人物が更新または作成された場合、その更新は、[!DNL Sales Insight Actions] web アプリデータベースに渡されます。

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

## 営業活動は [!DNL Salesforce] に記録されますか？ {#do-sales-activities-log-to-salesforce}

はい、セールスエンゲージメントアクティビティは、ネイティブタスクとして [!DNL Salesforce] にログします。 その後、これらのタスクを [!DNL Salesforce] レポートで使用して、販売活動を追跡するチームダッシュボードを強化できます。

管理者 [!DNL Sales Insight Actions]、ログに記録するセールスアクティビティを設定で [!DNL Salesforce] ます。 これらのアクティビティには、メール、電話、開封リマインダータスクが含まれます。

![](assets/actions-data-sync-faq-6.png)

上の図は、[!DNL Salesforce] に記録される情報を示しています。 メールや電話などのアクティビティは、[!DNL Salesforce] に [ 一方向の同期 ](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md) で記録されます。 [登録解除](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md)および[リマインダータスク](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md)は双方向同期で最新の状態に保たれます。これらの各データ同期は、web アプリインターフェイスから設定 [!DNL Sales Insight Actions] きます。

>[!MORELIKETHIS]
>
>* [ 購読解除の同期  [!DNL Salesforce]](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md)
>* [Marketo 登録解除チェック](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md)
>* [[!DNL Salesforce] 同期設定](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md)
>* [ リマインダータスクの同期先  [!DNL Salesforce]](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md)
>* [データ同期の開始](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.md#initiate-data-sync)

