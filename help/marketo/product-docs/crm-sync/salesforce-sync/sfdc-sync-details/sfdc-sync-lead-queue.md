---
unique-page-id: 7516241
description: SFDC 同期 - リードキュー - Marketo ドキュメント - 製品ドキュメント
title: SFDC 同期 - リードキュー
exl-id: b3b5e14c-f914-429c-a4b9-6b535ad8e882
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '130'
ht-degree: 54%

---

# SFDC 同期：リードキュー {#sfdc-sync-lead-queue}

Marketoでは、リードの配信に役立つユーザーを [[!DNL Salesforce]  リードキュー ](https://help.salesforce.com/apex/HTViewHelpDoc?id=queues_overview.htm) に追加できます。 詳細は以下の通りです。

## Marketo のキューに個人を割り当てる方法 {#how-to-assign-a-person-to-a-queue-in-marketo}

次のいずれかのフロー・アクションを使用して、[!DNL Salesforce] のリード・キューに個人を割り当てることができます。

* [ ユーザーをSFDCに同期 ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}
* [ 所有者の変更 ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md){target="_blank"}

>[!NOTE]
>
>Marketo では、キューを作成または変更できません。

## 個人がキューに属する場合、リード所有者情報はどのように保存されますか？ {#how-is-lead-owner-information-stored-if-the-person-belongs-to-a-queue}

リードが [!DNL Salesforce] のキューに所有されている場合、リードが所有者に割り当てられるまで、これらの販売所有者フィールドは空のままになります。

* セールス所有者の名
* セールス所有者の姓
* セールス所有者の職位
* セールス所有者の電話番号
* セールス所有者のメールアドレス
