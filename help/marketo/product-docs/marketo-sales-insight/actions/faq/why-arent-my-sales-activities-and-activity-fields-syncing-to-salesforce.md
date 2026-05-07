---
description: セールスアクティビティとフィールドがSalesforceに同期されない場合のトラブルシューティング。 APIのロギング、カスタムフィールド、権限を確認します。
title: セールスアクティビティおよびアクティビティフィールドが Salesforce に同期されない理由
exl-id: 5da855f2-18c6-456a-9e5d-ef4499596b3c
source-git-commit: 240b78561db11e169188698880d4707a5c1f64de
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 68%

---

# セールスアクティビティおよびアクティビティフィールドが Salesforce に同期されない理由 {#why-arent-my-sales-activities-and-activity-fields-syncing-to-salesforce}

**Salesforce に同期されたメールまたは電話アクティビティが表示されません。**

* Salesforceに接続していることを確認します。 各ユーザーは、メールおよび電話を Salesforce に記録するために接続している必要があります。
* [Salesforce 同期設定](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md){target="_blank"}が設定されていることを確認してください。
* メールは、プライマリルックアップとしての Salesforce ID およびセカンダリとしてのメールアドレスに基づいてレコードルックアップを行います。 個人レコードにSalesforce IDとメールアドレスがリンクされていることを、[ アクション web アプリ ](https://toutapp.com/next#command_center){target="_blank"}で確認できます。
* 電話は、Salesforce ID のみに基づいてレコードルックアップを行います。 Actions の人物レコードに Salesforce ID が存在しない場合、電話は記録されません。 個人レコードにSalesforce IDがリンクされていることを、[ アクション web アプリ ](https://toutapp.com/next#command_center){target="_blank"}で確認できます。

**Salesforce アップデートにアクティビティフィールドが表示されません。**

Salesforceでメール [ アクティビティ属性フィールド ](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}の更新が表示されない場合は、チームのフィールドアクセシビリティが制限されている可能性があります。 Salesforce のフィールドレベルセキュリティにより、Salesforce 管理者は、ユーザーが表示および編集可能な情報に制限を設けることができます。 Actions ユーザーがこれらのフィールドを表示および編集するアクセス権を持っていない場合、Actions アクティビティ同期は、これらのフィールドの更新に失敗します。

* Salesforce 管理者と連携して、これらのセキュリティ設定が [Actions Salesforce Activity フィールド](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}に干渉しないようにします。
* Salesforce管理者の場合は、「セキュリティコントロール」タブでフィールドアクセシビリティを確認できます。 Actions がやり取りするメインオブジェクトは、リード、連絡先、アカウント、商談、タスク／アクティビティです。

>[!NOTE]
>
>リード、取引先責任者、アカウントおよび商談オブジェクトに関連付けられたフィールドは、セールスインサイトSalesforce パッケージと共にインストールされます。 [タスク／アクティビティレコードタイプに関連付けられたフィールドは、Salesforce 管理者によって作成される必要があります](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}。
