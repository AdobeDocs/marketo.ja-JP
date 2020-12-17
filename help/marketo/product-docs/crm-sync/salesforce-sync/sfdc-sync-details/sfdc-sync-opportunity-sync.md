---
unique-page-id: 2953467
description: SFDC同期 — オポチュニティの同期 — Marketto Docs — 製品ドキュメント
title: SFDC同期 — オポチュニティ同期
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 0%

---


# SFDC同期：オポチュニティの同期{#sfdc-sync-opportunity-sync}

## 2つのシステム間でオポチュニティの詳細を同期させる方法{#how-are-opportunity-details-kept-in-sync-between-the-two-systems}

同期は次の1つの方法で行われます。SalesforceからMarketoへ Salesforceのオポチュニティに対する更新は、Marketoに同期されます。

>[!NOTE]
>
>Marketo for Salesforce](../../../../product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)に入力する[資格情報は、データの同期に使用されます。 資格情報にアクセスできるデータのみが含まれます。

## オポチュニティの同期を開始できますか。{#can-i-initiate-an-opportunity-sync}

いや、できない。Salesforceのオポチュニティに対する変更は、Marketoに自動的に同期されます。

## Opportunity Amountで複数の通貨がサポートされているか。{#does-marketo-support-more-than-one-currency-in-the-opportunity-amount}

いいえ。マーケティング担当者は1つの通貨のみをサポートしています。 オポチュニティの金額はSalesforceから同期されますが、通貨はMarketo購読の[デフォルトの通貨](https://docs.marketo.com/display/DOCS/Set+Default+Location+Settings+for+a+Subscription#SetDefaultLocationSettingsforaSubscription-SettheDefaultCurrencySettingsforaSubscription)になります。

## オポチュニティと連絡先を関連付ける方法{#how-does-marketo-associate-opportunities-and-contacts}

Marketorは、[Opportunity Contact Roles](https://help.salesforce.com/HTViewHelpDoc?id=contactroles.htm)を使用して、オポチュニティと連絡先を関連付けます。 連絡先の役割が割り当てられていないオポチュニティは、Marketorに同期されますが、誰にも属しません。 例えば、「Has Opportunity」フィルターは適用されません。

## 人の機会を全て見るにはどうすればいいですか。{#how-can-i-see-all-the-opportunities-of-a-person}

オポチュニティのリストは、[個人の詳細](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md)ページの「**オポチュニティ情報**」タブで表示できます。

## オポチュニティに関連するトリガー/フィルターは何か。{#what-are-the-triggers-filters-related-to-opportunity}

トリガー：

* オポチュニティに追加
* オポチュニティから削除
* オポチュニティが更新されます

フィルター:

* オポチュニティがある
* オポチュニティが更新されたか、オポチュニティが更新されませんでした
* オポチュニティに追加された/Opportunityに追加されなかった
* オポチュニティから削除されたか、オポチュニティから削除されませんでした
* 合計金額
* オプション数
* 合計利益予測売上高

>[!TIP]
>
>フィルターとトリガーの制約事項を確認します。 そこには素晴らしい細部がたくさんある。
>
>Salesforceのオポチュニティオブジェクトに新しいフィールドを作成するだけで、それが自動的に制約になります。

世界最高のセールスフォースの同期性を持つマーケット！