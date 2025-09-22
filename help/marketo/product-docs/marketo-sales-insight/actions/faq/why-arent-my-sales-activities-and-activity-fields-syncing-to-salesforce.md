---
description: セールスアクティビティおよびアクティビティフィールドが Salesforce に同期されない理由- Marketo ドキュメント - 製品ドキュメント
title: セールスアクティビティおよびアクティビティフィールドが Salesforce に同期されない理由
exl-id: 5da855f2-18c6-456a-9e5d-ef4499596b3c
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 87%

---

# セールスアクティビティおよびアクティビティフィールドが Salesforce に同期されない理由 {#why-arent-my-sales-activities-and-activity-fields-syncing-to-salesforce}

**Salesforce に同期されたメールまたは電話アクティビティが表示されません。**

* Salesforce に接続していることを確認してください。各ユーザーは、メールおよび電話を Salesforce に記録するために接続している必要があります。
* [Salesforce 同期設定](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md){target="_blank"}が設定されていることを確認してください。
* メールは、プライマリルックアップとしての Salesforce ID およびセカンダリとしてのメールアドレスに基づいてレコードルックアップを行います。[ アクション web アプリ ](https://toutapp.com/next#command_center){target="_blank"} で、人物レコードにSalesforce ID とメールアドレスのリンクがあることを確認できます。
* 電話は、Salesforce ID のみに基づいてレコードルックアップを行います。Actions の人物レコードに Salesforce ID が存在しない場合、電話は記録されません。[ アクション web アプリ ](https://toutapp.com/next#command_center){target="_blank"} で、人物レコードにSalesforce ID がリンクされていることを確認できます。

**Salesforce アップデートにアクティビティフィールドが表示されません。**

Salesforce にメール[アクティビティ属性フィールド](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}アップデートが表示されない場合、チームのフィールドアクセシビリティの制限が原因である可能性があります。Salesforce のフィールドレベルセキュリティにより、Salesforce 管理者は、ユーザーが表示および編集可能な情報に制限を設けることができます。Actions ユーザーがこれらのフィールドを表示および編集するアクセス権を持っていない場合、Actions アクティビティ同期は、これらのフィールドの更新に失敗します。

* Salesforce 管理者と連携して、これらのセキュリティ設定が [Actions Salesforce Activity フィールド](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}に干渉しないようにします。
* Salesforce 管理者には、「セキュリティコントロール」タブに「フィールドアクセシビリティ」が表示されます。Actions がやり取りするメインオブジェクトは、リード、連絡先、アカウント、商談、タスク／アクティビティです。

>[!NOTE]
>
>リード、連絡先、アカウントおよび商談オブジェクトに関連付けられたフィールドは、Sales Insight Salesforce パッケージと共にインストールされます。[タスク／アクティビティレコードタイプに関連付けられたフィールドは、Salesforce 管理者によって作成される必要があります](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}。
