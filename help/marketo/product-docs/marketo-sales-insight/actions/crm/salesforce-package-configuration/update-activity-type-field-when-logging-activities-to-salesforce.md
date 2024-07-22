---
description: Salesforce にアクティビティを記録する際のアクティビティタイプフィールドの更新 - Marketo ドキュメント - 製品ドキュメント
title: Salesforce にアクティビティを記録する際のアクティビティタイプフィールドの更新
exl-id: 800323cb-2b99-42f1-ae30-0f87a9a1b4be
source-git-commit: c16081143588ebc0793f5b6e2630b58348e27124
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 100%

---

# Salesforce にアクティビティを記録する際のアクティビティタイプフィールドの更新 {#update-activity-type-field-when-logging-activities-to-salesforce}

Actions は、レポートに使用したりアクティビティ履歴の視認性を高めたりするために、メールおよび電話アクティビティを Salesforce に自動的に同期できます。アクティビティのログを記録する際に、記録されるアクティビティのタイプに応じて、「アクティビティのタイプ」フィールドが、メール、電話または返信に対して適切に更新されていることを確認してください。

>[!NOTE]
>
>BCC によってメールをログに記録する場合、BCC アドレスを通じて Salesforce に配信されるので、「タスクタイプ」ピックリストは参照されず、代わりに、タイプフィールドには自動的に「メール」が入力されます。

## 留意事項 {#things-to-know}

* Salesforce との接続は、「タスクタイプ」を更新するために必要です。
* 「タスクタイプ」ピックリストで、デフォルトのタイプ値が選択されていない必要があります。
* 「電話（Call）」、「返信（Reply）」、「メール（Email）」がすべて「タスクタイプ」ピックリストに存在する必要があります（大文字と小文字を区別する）。
* 「タスクタイプ」フィールドを更新する Salesforce のワークフローまたはトリガーは、このプロセスに干渉する可能性があります。

## セットアップ {#setup}

まず、適切な選択リスト値が設定されていることを確認します。選択リストに変更を加えるには、Salesforce 管理者の支援が必要です。

まず、「タスクタイプ」ピックリストで見つからない値を確認します（メール、電話、返信のうち）。これを確認したり、「アクティビティのタイプ」ピックリストに変更を加えるには、Salesforce 管理者の支援が必要になる可能性があります。これらの変更を加えるために、Salesforce 管理者は以下の手順に従うことができます。

### Salesforce Lightning では {#salesforce-lightning}

1. [Salesforce.com](https://salesforce.com){target="_blank"} に移動します。
1. 右上隅にある歯車アイコンをクリックして、**設定**／**オブジェクトマネージャー**&#x200B;を選択します。
1. 「クイック検索」ボックスに「タスク」と入力します。
1. 左側のパネルで、「**フィールドと関係**」をクリックします。
1. フィールドラベル「**タイプ**」をクリックします。
1. 「タスクタイプピックリストの値」で、「**新規**」をクリックします。
1. 見つからない「タスクタイプ」ピックリスト値の名前を入力します（「メール」、「電話」、「返信」）。
1. 「**保存**」をクリックします。

### Salesforce Classic では {#salesforce-classic}

1. [Salesforce.com](https://salesforce.com){target="_blank"} に移動します。
1. **設定**／**ビルド**／**カスタマイズ**／**アクティビティ**／**タスクフィールド**&#x200B;をクリックします。
1. 「**タイプ**」をクリックします。
1. 「タスクタイプピックリストの値」で、「**新規**」をクリックします。
1. 見つからない「タスクタイプ」ピックリスト値の名前を入力します（「メール」、「電話」、「返信」）。
1. 「**保存**」をクリックします。

これで、「タイプ」フィールドに、ログに記録されたメール、電話、返信の対応する値が表示されます。これらの値は、Sales Insight Actions リマインダータスクには&#x200B;_設定されません_。

>[!NOTE]
>
>値として「返信」が表示されない場合は、「**新規**」をクリックして返信を追加します。Salesforce では、「返信」は標準値ではありません。

>[!MORELIKETHIS]
>
>* [セールスアクティビティ属性の Salesforce へのログ](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}
>* [Salesforce アクティビティの詳細のカスタマイズの設定](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md){target="_blank"}
>* [セールスアクティビティの Salesforce への同期](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md){target="_blank"}
