---
description: セールスアクティビティとアクティビティフィールドが Salesforce に同期されないのはなぜですか？ - Marketo ドキュメント - 製品ドキュメント
title: セールスアクティビティとアクティビティフィールドが Salesforce に同期されないのはなぜですか？
source-git-commit: c50f0f08914076a440026fb368bf38763b282bbf
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 1%

---

# セールスアクティビティとアクティビティフィールドが Salesforce に同期されないのはなぜですか？ {#why-arent-my-sales-activities-and-activity-fields-syncing-to-salesforce}

**Salesforce に同期されたメールまたは通話アクティビティが表示されません。**

* Salesforce に必ず接続してください。 各ユーザーは、電子メールと Salesforce への呼び出しをログに記録するための接続が必要です。
* が設定されていることを確認します。 [Salesforce 同期設定](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md){target="_blank"}.
* メールは、Salesforce ID に基づいてレコード検索をプライマリ参照とし、メールアドレスをセカンダリとして実行します。 担当者レコードに Salesforce ID とメールアドレスがリンクされていることを、 [アクション Web アプリ](https://toutapp.com/next#command_center){target="_blank"}.
* 呼び出しでは、Salesforce ID に基づくレコード参照のみ実行されます。 アクション内の担当者レコードに Salesforce ID が存在しない場合、呼び出しはログに記録されません。 担当者レコードに Salesforce ID がリンクされていることを、 [アクション Web アプリ](https://toutapp.com/next#command_center){target="_blank"}.

**Salesforce 更新にアクティビティフィールドが表示されません。**

電子メールが表示されない場合 [アクティビティ属性フィールド](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"} Salesforce で更新した場合、チームのフィールドアクセシビリティの制限が原因の可能性があります。 Salesforce フィールドレベルのセキュリティにより、Salesforce 管理者は、ユーザーが表示可能で編集可能な情報に制限を設けることができます。 アクションユーザーがこれらのフィールドを表示および編集するアクセス権を持っていない場合、アクションアクティビティの同期は、これらのフィールドの更新に失敗します。

* Salesforce 管理者と連携して、これらのセキュリティ設定が [アクション Salesforce アクティビティフィールド](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}.
* Salesforce 管理者の場合は、「セキュリティコントロール」タブの「フィールドアクセシビリティ」が表示されます。 アクションが操作する主なオブジェクトは次のとおりです。リード、連絡先、アカウント、商談、タスク/アクティビティ。

>[!NOTE]
>
>リード、連絡先、アカウント、商談の各オブジェクトに関連付けられたフィールドは、Sales Insight Salesforce パッケージと共にインストールされます。 次に関連するフィールド： [タスク/アクティビティレコードタイプを作成する必要があります](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"} Salesforce 管理者によって
