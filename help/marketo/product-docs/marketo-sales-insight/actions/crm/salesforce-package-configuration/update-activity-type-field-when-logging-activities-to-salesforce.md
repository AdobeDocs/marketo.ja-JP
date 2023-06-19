---
description: アクティビティを Salesforce にログ記録する際のアクティビティタイプフィールドの更新 — Marketo Docs — 製品ドキュメント
title: アクティビティを Salesforce にログ記録する際のアクティビティタイプフィールドの更新
exl-id: f65d7d97-ec65-4210-9381-02be788498f9
source-git-commit: 02354356949aef7aa8836d4753ec538b7819a65a
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 17%

---

# アクティビティを Salesforce にログ記録する際のアクティビティタイプフィールドの更新 {#update-activity-type-field-when-logging-activities-to-salesforce}

アクションは、メールと通話アクティビティを Salesforce に自動的に同期して、レポートに使用し、アクティビティ履歴の可視性を高めることができます。 アクティビティをログに記録する場合は、記録するアクティビティの種類に応じて、「アクティビティタイプ」フィールドが適切に「 E メール」、「呼び出し」、「返信」に更新されていることを確認します。

>[!NOTE]
>
>BCC 経由での電子メールのログは、タスクタイプの選択リストを参照せず、代わりに、BCC アドレスを通じて Salesforce に配信されるので、タイプフィールドに「電子メール」と自動的に入力します。

## 留意事項 {#things-to-know}

* タスクの種類を更新するには、Salesforce との接続が必要です。
* Task Type の選択リストでデフォルトの Type 値が選択されていないはずです。
* 呼び出し、返信、電子メールは、すべてタスクタイプの選択リストに存在する必要があります（大文字/小文字の区別が必要です）。
* Salesforce のトリガー（[ タスクの種類 ] フィールドを更新するワークフロー）が、この処理を妨げる可能性があります。

## セットアップ {#setup}

まず、適切な選択リスト値が設定されていることを確認します。選択リストに変更を加えるには、Salesforce 管理者の支援が必要です。

まず、タスクタイプ選択リスト（E メール、呼び出し、返信から）に不足している値を確認します。 これを確認し、アクティビティタイプの選択リストを変更するには、Salesforce 管理者の支援が必要になる場合があります。 これらの変更を行うには、Salesforce 管理者は以下の手順に従うことができます。

### Salesforce Lightning 内 {#salesforce-lightning}

1. に移動します。 [Salesforce.com](https://salesforce.com){target="_blank"}.
1. 右上隅の歯車アイコンをクリックし、「 **設定** > **オブジェクトマネージャ**.
1. [ クイック検索 ] ボックスに&quot;task&quot;と入力します。
1. 左側のパネルで、 **フィールドと関係**.
1. フィールドラベルをクリック **タイプ**.
1. [ タスクタイプ選択リストの値 ] で、 **新規**.
1. 欠落している Task Type Picklist 値の名前を入力します (&quot;Email, &quot;Call&quot;, &quot;Reply&quot;)。
1. 「**保存**」をクリックします。

### Salesforce Classic 内 {#salesforce-classic}

1. に移動します。 [Salesforce.com](https://salesforce.com){target="_blank"}.
1. クリック **設定** > **ビルド** > **カスタマイズ** > **アクティビティ** > **タスクフィールド**.
1. 「**タイプ**」をクリックします。
1. [ タスクタイプ選択リストの値 ] で、 **新規**.
1. 欠落している Task Type Picklist 値の名前を入力します (&quot;Email, &quot;Call&quot;, &quot;Reply&quot;)。
1. 「**保存**」をクリックします。

これで、「タイプ」フィールドが表示され、ログに記録された E メール、呼び出し、返信の対応する値が入力されます。 これらの値は、 _not_ は、Sales Insight Actions リマインダータスクに対して設定されます。

>[!NOTE]
>
>値として「返信」が表示されない場合は、「**新規**」をクリックして返信を追加します。Salesforce では、「返信」は標準値ではありません。

>[!MORELIKETHIS]
>
>* [セールスアクティビティ属性の Salesforce へのログ](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}
>* [Salesforce アクティビティ詳細のカスタマイズの設定](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md){target="_blank"}
>* [セールス活動を Salesforce に同期](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md){target="_blank"}
