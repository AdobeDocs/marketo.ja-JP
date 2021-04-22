---
unique-page-id: 2953469
description: SFDC同期 —キャンペーン同期 —Marketoドキュメント — 製品ドキュメント
title: SFDC同期 —キャンペーン同期
exl-id: 62435e00-9c59-4dee-a9b7-ccf1d1f41b78
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 5%

---

# SFDC同期：キャンペーン同期{#sfdc-sync-campaign-sync}

Marketoプログラムは、Salesforceキャンペーンと同期できます。 この機能の概要を次に示します。

## なぜMarketoプログラムをSalesforceキャンペーンと同期する必要があるのですか。{#why-should-i-sync-marketo-programs-with-salesforce-campaigns}

* Marketoプログラムの強力な機能を使う。
* MarketoプログラムとSalesforceキャンペーンの間で、メンバーとそのステータスを同期させる。
* MarketoおよびSalesforceのレポート機能をタップします。

## MarketoのプログラムとSalesforceのキャンペーンは、どのように同期されますか。{#how-is-a-marketo-program-and-a-salesforce-campaign-synced}

Marketoでは、プログラムとSalesforceキャンペーンの間の1対1のマッピングを作成するオプションがあります。

![](assets/image2015-7-8-9-3a43-3a8.png)

Marketoの&#x200B;**[チャネル](/help/marketo/product-docs/administration/tags/create-a-program-channel.md)**&#x200B;と&#x200B;**[キャンペーンコスト](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-period-costs.md)**&#x200B;は、**期間タイプ**&#x200B;と&#x200B;**実費**&#x200B;としてSalesforceと同期する。 この同期は、MarketoからSalesforceへの&#x200B;**一方向**&#x200B;です。

Marketo **プログラムメンバー**&#x200B;とその&#x200B;**[進行状態](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)**&#x200B;は、**Salesforceキャンペーンメンバー**&#x200B;と&#x200B;**キャンペーンメンバー像**&#x200B;との同期を保つ。 これは&#x200B;**双方向の同期**&#x200B;なので、MarketoまたはSalesforceで行った変更は両方のシステムに反映されます。

>[!NOTE]
>
>MarketoプログラムにSalesforceに存在しない会員がいる場合、Marketoは、Salesforceでその会員をリードとして作成します。

## キャンペーンに関連するトリガー/フィルターは何か。{#what-are-the-triggers-filters-related-to-campaigns}

トリガー:

* SFDC キャンペーンに追加済み
* SFDC キャンペーンから削除済み
* SFDC キャンペーンでステータスが変更されています

フィルター:

* SFDC キャンベーンのメンバー

## SFDCキャンペーンにMarketo人を追加できますか。{#can-i-add-marketo-people-to-my-sfdc-campaign}

はい、[からSFDCへのキャンペーンフロー追加アクション](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/add-to-sfdc-campaign.md)を使用します。 この人がSalesforceに存在しない場合、MarketoはSalesforceで作成し、キャンペーンに追加します。

## Marketoを使用してSFDCキャンペーンからメンバーを削除できますか。{#can-i-remove-members-from-my-sfdc-campaign-using-marketo}

はい、[SFDCキャンペーンフローから削除](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/remove-from-sfdc-campaign.md)を使用します。

## Marketoを使用してキャンペーンメンバーのステータスを変更できますか？{#can-i-change-campaign-member-status-using-marketo}

はい、SFDCキャンペーンフローアクション](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md)の[ステータスの変更を使用します。

## 自分のSalesforceキャンペーンが見えないのはなぜですか。{#why-cant-i-see-any-of-my-salesforce-campaigns}

次の項目を確認できます。

1. [キャンペーン同期が有効](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md)であることを確認します。
1. [Marketo同期ユーザー](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)がSalesforceの[マーケティングユーザー](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md)であることを確認します。

>[!NOTE]
>
>SalesforceキャンペーンとマッピングされたMarketoプログラムに互換性のないプログラムステータスがある場合は、エラーメッセージが表示される場合があります。 同期](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-errors/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md)の前に、[プログラムのステータスに一致することをお勧めします。

>[!MORELIKETHIS]
>
>* [SFDCキャンペーンとプログラムの同期](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/sync-an-sfdc-campaign-with-a-program.md)
>* [プログラムメンバーシップについて](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)
>* [キャンペーン同期の有効化/無効化](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md)
>* [Marketo同期ユーザーをマーケティングユーザーにする](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md)

