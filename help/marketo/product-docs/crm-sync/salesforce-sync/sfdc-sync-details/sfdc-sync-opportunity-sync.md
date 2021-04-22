---
unique-page-id: 2953467
description: SFDC同期 — オポチュニティ同期 —Marketoドキュメント — 製品ドキュメント
title: SFDC同期 — オポチュニティ同期
exl-id: f8acc528-c631-43f0-8899-2f3c6fdabe9e
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 4%

---

# SFDC同期：オポチュニティの同期{#sfdc-sync-opportunity-sync}

## 2つのシステム間でオポチュニティの詳細を同期させる方法{#how-are-opportunity-details-kept-in-sync-between-the-two-systems}

同期は次の1つの方法で行われます。セールスフォースからMarketoまで Salesforceのオポチュニティに対する更新は、Marketoに同期されます。

>[!NOTE]
>
>Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)用にMarketoに入力した[資格情報は、データの同期に使用されます。 資格情報にアクセスできるデータのみが含まれます。

## オポチュニティの同期を開始できますか。{#can-i-initiate-an-opportunity-sync}

いや、できない。Salesforceのオポチュニティに対する変更は、自動的にMarketoに同期されます。

## MarketoはOpportunity Amountで複数の通貨をサポートしていますか。{#does-marketo-support-more-than-one-currency-in-the-opportunity-amount}

いいえ。Marketoは1つの通貨のみをサポートします。 オポチュニティの金額はSalesforceから同期されますが、通貨はMarketo購読の[デフォルトの通貨](/help/marketo/product-docs/administration/settings/set-default-location-settings-for-a-subscription.md#set-the-default-currency-settings-for-a-subscription)になります。

## Marketoは機会と連絡をどのように関連付けているか。{#how-does-marketo-associate-opportunities-and-contacts}

Marketoは、[Opportunity Contact Roles](https://help.salesforce.com/HTViewHelpDoc?id=contactroles.htm)を使用して、オポチュニティと連絡先を関連付けます。 連絡先ロールが割り当てられていないオポチュニティは、Marketoに同期されますが、誰にも属しません。 例えば、「Has Opportunity」フィルターは適用されません。

## 人の機会を全て見る方法は？{#how-can-i-see-all-the-opportunities-of-a-person}

オポチュニティのリストは、[個人の詳細](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md)ページの「**オポチュニティ情報**」タブで表示できます。

## オポチュニティに関連するトリガー/フィルターは何か。{#what-are-the-triggers-filters-related-to-opportunity}

トリガー:

* オポチュニティに追加
* オポチュニティから削除
* オポチュニティが更新されます

フィルター:

* 商談あり
* オポチュニティが更新されたか、オポチュニティが更新されませんでした
* オポチュニティに追加された/Opportunityに追加されなかった
* オポチュニティから削除されたか、オポチュニティから削除されませんでした
* 合計商談数
* 商談数
* 商談の合計収益予測

>[!TIP]
>
>フィルターとトリガーの制約事項を確認します。 そこには素晴らしい細部がたくさんある。
>
>Salesforceのオポチュニティオブジェクトに新しいフィールドを作成するだけで、それが自動的に制約になります。
