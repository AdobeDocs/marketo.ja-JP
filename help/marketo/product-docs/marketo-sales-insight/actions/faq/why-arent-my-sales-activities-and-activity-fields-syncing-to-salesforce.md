---
description: セールスアクティビティおよびアクティビティフィールドが Salesforce に同期されない理由- Marketo ドキュメント - 製品ドキュメント
title: セールスアクティビティおよびアクティビティフィールドが Salesforce に同期されない理由
source-git-commit: c50f0f08914076a440026fb368bf38763b282bbf
workflow-type: ht
source-wordcount: '335'
ht-degree: 100%

---

# セールスアクティビティおよびアクティビティフィールドが Salesforce に同期されない理由 {#why-arent-my-sales-activities-and-activity-fields-syncing-to-salesforce}

**Salesforce に同期されたメールまたは電話アクティビティが表示されません。**

* Salesforce に接続していることを確認してください。各ユーザーは、メールおよび電話を Salesforce に記録するために接続している必要があります。
* [Salesforce 同期設定](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md){target="_blank"}が設定されていることを確認してください。
* メールは、プライマリルックアップとしての Salesforce ID およびセカンダリとしてのメールアドレスに基づいてレコードルックアップを行います。[Actions web アプリ](https://toutapp.com/next#command_center){target="_blank"}で、人物レコードに Salesforce ID およびメールアドレスがリンクされていることを確認できます。
* 電話は、Salesforce ID のみに基づいてレコードルックアップを行います。Actions の人物レコードに Salesforce ID が存在しない場合、電話は記録されません。[Actions web アプリ](https://toutapp.com/next#command_center){target="_blank"}で、人物レコードに Salesforce ID がリンクされていることを確認できます。

**Salesforce アップデートにアクティビティフィールドが表示されません。**

Salesforce にメール[アクティビティ属性フィールド](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}アップデートが表示されない場合、チームのフィールドアクセシビリティの制限が原因である可能性があります。Salesforce のフィールドレベルセキュリティにより、Salesforce 管理者は、ユーザーが表示および編集可能な情報に制限を設けることができます。Actions ユーザーがこれらのフィールドを表示および編集するアクセス権を持っていない場合、Actions アクティビティ同期は、これらのフィールドの更新に失敗します。

* Salesforce 管理者と連携して、これらのセキュリティ設定が [Actions Salesforce Activity フィールド](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}に干渉しないようにします。
* Salesforce 管理者には、「セキュリティコントロール」タブに「フィールドアクセシビリティ」が表示されます。Actions がやり取りするメインオブジェクトは、リード、連絡先、アカウント、商談、タスク／アクティビティです。

>[!NOTE]
>
>リード、連絡先、アカウントおよび商談オブジェクトに関連付けられたフィールドは、Sales Insight Salesforce パッケージと共にインストールされます。[タスク／アクティビティレコードタイプに関連付けられたフィールドは、Salesforce 管理者によって作成される必要があります](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}。
