---
unique-page-id: 2953469
description: SFDC同期 —キャンペーン同期 — Marketto Docs — 製品ドキュメント
title: SFDC同期 —キャンペーン同期
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 0%

---


# SFDC同期：キャンペーン同期 {#sfdc-sync-campaign-sync}

Marketorプログラムは、Salesforceキャンペーンと同期できます。 この機能の概要を次に示します。

## MarketorプログラムとSalesforceキャンペーンを同期する必要があるのはなぜですか。 {#why-should-i-sync-marketo-programs-with-salesforce-campaigns}

* マーケティングプログラムの強力な機能を使用します。
* MarketorプログラムとSalesforceキャンペーンの間で、メンバーとそのステータスを同期させます。
* MarketoとSalesforceのレポート機能をタップします。

## MarketoプログラムとSalesforceキャンペーンは、どのように同期されますか。 {#how-is-a-marketo-program-and-a-salesforce-campaign-synced}

Marketoでは、プログラムとSalesforceキャンペーンの間の1対1のマッピングを作成するオプションがあります。

![](assets/image2015-7-8-9-3a43-3a8.png)

** [チャネル](../../../../product-docs/administration/tags/create-a-program-channel.md) および** **期間コスト [Marketoは、Salesforceに対して、キャンペーンタイプとしての](../../../../product-docs/core-marketo-concepts/programs/working-with-programs/understanding-period-costs.md)** 期間コストMarkettoと、実際のコストSalesとして同期 ********&#x200B;します。 この同期は、MarketoからSalesforce **への** 1つの方法です。

Marketo **プログラムメンバー** とその** [進行状態](../../../../product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)**は、Salesforceキャンペーンメンバーおよび **キャンペーンメンバー像と同期され******&#x200B;ます。 これは **双方向の** 同期です **。したがって**、MarketoまたはSalesforceで行った変更は両方のシステムに反映されます。

>[!NOTE]
>
>MarketoプログラムにSalesforceに存在しないメンバーが存在する場合、MarketoはSalesforceのリードとしてそれらのメンバーを作成します。

## キャンペーンに関連するトリガー/フィルターは何ですか。 {#what-are-the-triggers-filters-related-to-campaigns}

トリガー：

* SFDCキャンペーンに追加
* SFDCキャンペーンから削除
* SFDCキャンペーンでステータスが変更された場合

フィルター:

* SFDCキャンペーンのメンバー

## SFDCキャンペーンにマーケティング担当者を追加できますか。 {#can-i-add-marketo-people-to-my-sfdc-campaign}

はい、 [SFDCへのキャンペーンフローアクション](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/add-to-sfdc-campaign.md)を追加使用します。 この人物がSalesforceに存在しない場合、MarketorはSalesforceで作成し、キャンペーンに追加します。

## Marketoを使用してSFDCキャンペーンからメンバーを削除できますか。 {#can-i-remove-members-from-my-sfdc-campaign-using-marketo}

はい、 [SFDCキャンペーンフローからの](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/remove-from-sfdc-campaign.md)削除アクションを使用します。

## Marketoを使用してキャンペーンのメンバーステータスを変更できますか。 {#can-i-change-campaign-member-status-using-marketo}

はい、SFDCキャンペーンフローアクションの [変更ステータスを使用し](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md)ます。

## 自分のSalesforceキャンペーンが見えないのはなぜですか。 {#why-cant-i-see-any-of-my-salesforce-campaigns}

次の項目を確認できます。

1. [キャンペーンの同期が有効になっていることを確認します](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md)。
1. Salesforceの [マーケティングユーザー](../../../../product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) (Marketto Sync User [](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md) )であることを確認します。

>[!NOTE]
>
>SalesforceキャンペーンとマッピングされたMarketoプログラムに互換性のないプログラムステータスがある場合は、エラーメッセージが表示される場合があります。 同期の前に、プログラムのステータスを [一致させることをお勧めします](sfdc-errors/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md)。

>[!NOTE]
>
>**関連記事**
>
>* [SFDCキャンペーンとプログラムの同期](../../../../product-docs/core-marketo-concepts/programs/working-with-programs/sync-an-sfdc-campaign-with-a-program.md)
>* [プログラムメンバーシップについて](../../../../product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)
>* [キャンペーン同期の有効化/無効化](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md)
>* [マーケティングユーザーの同期をマーケティングユーザーにする](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md)

>



