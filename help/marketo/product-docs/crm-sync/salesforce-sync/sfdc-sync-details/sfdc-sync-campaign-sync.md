---
unique-page-id: 2953469
description: SFDC同期 —キャンペーン同期 — Marketto Docs — 製品ドキュメント
title: SFDC同期 —キャンペーン同期
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---


# SFDC同期：キャンペーン同期{#sfdc-sync-campaign-sync}

Marketorプログラムは、Salesforceキャンペーンと同期できます。 この機能の概要を次に示します。

## MarketorプログラムとSalesforceキャンペーンを同期する必要があるのはなぜですか。{#why-should-i-sync-marketo-programs-with-salesforce-campaigns}

* マーケティングプログラムの強力な機能を使用します。
* MarketorプログラムとSalesforceキャンペーンの間で、メンバーとそのステータスを同期させます。
* MarketoとSalesforceのレポート機能をタップします。

## MarketoプログラムとSalesforceキャンペーンは、どのように同期されますか。{#how-is-a-marketo-program-and-a-salesforce-campaign-synced}

Marketoでは、プログラムとSalesforceキャンペーンの間の1対1のマッピングを作成するオプションがあります。

![](assets/image2015-7-8-9-3a43-3a8.png)

Marketoの&#x200B;**[チャネル](/help/marketo/product-docs/administration/tags/create-a-program-channel.md)**&#x200B;と&#x200B;**[キャンペーンコスト](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-period-costs.md)**&#x200B;は、**期間タイプ**&#x200B;と&#x200B;**実際のコスト**&#x200B;としてSalesforceと同期します。 この同期は、MarketoからSalesforceへの&#x200B;**1方向**&#x200B;です。

**プログラムメンバー**&#x200B;と&#x200B;**[進行状況](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)**&#x200B;は、**Salesforceキャンペーンメンバー**&#x200B;と&#x200B;**キャンペーンメンバー像**&#x200B;と同期している。 これは&#x200B;**双方向の同期**&#x200B;なので、MarketoまたはSalesforceで行った変更は両方のシステムに反映されます。

>[!NOTE]
>
>MarketoプログラムにSalesforceに存在しないメンバーが存在する場合、MarketoはSalesforceのリードとしてそれらのメンバーを作成します。

## キャンペーンに関連するトリガー/フィルターは何か。{#what-are-the-triggers-filters-related-to-campaigns}

トリガー:

* SFDCキャンペーンに追加
* SFDCキャンペーンから削除
* SFDCキャンペーンでステータスが変更された場合

フィルター:

* SFDCキャンペーンのメンバー

## SFDCキャンペーンにマーケティング担当者を追加できますか。{#can-i-add-marketo-people-to-my-sfdc-campaign}

はい、[からSFDCへのキャンペーンフロー追加アクション](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/add-to-sfdc-campaign.md)を使用します。 この人物がSalesforceに存在しない場合、MarketorはSalesforceで作成し、キャンペーンに追加します。

## Marketoを使用してSFDCキャンペーンからメンバーを削除できますか。{#can-i-remove-members-from-my-sfdc-campaign-using-marketo}

はい、[SFDCキャンペーンフローから削除](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/remove-from-sfdc-campaign.md)を使用します。

## Marketoを使用してキャンペーンのメンバーステータスを変更できますか。{#can-i-change-campaign-member-status-using-marketo}

はい、SFDCキャンペーンフローアクション](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md)の[ステータスの変更を使用します。

## 自分のSalesforceキャンペーンが見えないのはなぜですか。{#why-cant-i-see-any-of-my-salesforce-campaigns}

次の項目を確認できます。

1. [キャンペーン同期が有効](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md)であることを確認します。
1. [Marketo Sync User](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)がSalesforceの[マーケティングユーザー](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md)であることを確認します。

>[!NOTE]
>
>SalesforceキャンペーンとマッピングされたMarketoプログラムに互換性のないプログラムステータスがある場合は、エラーメッセージが表示される場合があります。 同期](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-errors/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md)の前に、[プログラムのステータスに一致することをお勧めします。

>[!MORELIKETHIS]
>
>* [SFDCキャンペーンとプログラムの同期](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/sync-an-sfdc-campaign-with-a-program.md)
>* [プログラムメンバーシップについて](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)
>* [キャンペーン同期の有効化/無効化](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md)
>* [マーケティングユーザーの同期をマーケティングユーザーにする](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md)

