---
unique-page-id: 2953469
description: SFDC の同期 - キャンペーンの同期 - Marketo ドキュメント - 製品ドキュメント
title: SFDC の同期 - キャンペーンの同期
exl-id: 62435e00-9c59-4dee-a9b7-ccf1d1f41b78
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '360'
ht-degree: 44%

---

# SFDC 同期：キャンペーンの同期 {#sfdc-sync-campaign-sync}

Marketo プログラムは、[!DNL Salesforce] キャンペーンと同期できます。 この仕組みの概要を次に示します。

## Marketo プログラムを [!DNL Salesforce] キャンペーンと同期する必要があるのはなぜですか？ {#why-should-i-sync-marketo-programs-with-salesforce-campaigns}

* Marketo Program の強力な機能を使用する。
* Marketo プログラムと [!DNL Salesforce] Campaign の間でメンバーとそのステータスを同期させます。
* Marketoと [!DNL Salesforce] のレポート機能を利用する。

## Marketo プログラムと [!DNL Salesforce] キャンペーンはどのように同期されますか？ {#how-is-a-marketo-program-and-a-salesforce-campaign-synced}

Marketoでは、プログラムと [!DNL Salesforce] キャンペーンの間に 1 対 1 のマッピングを作成するオプションがあります。

![](assets/image2015-7-8-9-3a43-3a8.png)

Marketoの **[チャネル](/help/marketo/product-docs/administration/tags/create-a-program-channel.md)** と **[期間コスト](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-period-costs.md)** は、[!DNL Salesforce] キャンペーンタイプ **と** 実際のコスト **として** に同期されます。 この同期は、Marketoから **への** 一方向 [!DNL Salesforce] です。

Marketo **プログラムメンバー** とその **[進行ステータス](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)** は、**[!DNL Salesforce]キャンペーンメンバー** および **キャンペーンメンバーのステータス** と同期が保たれます。 これは **双方向同期** なので、Marketoまたは [!DNL Salesforce] のいずれかで行われた変更は、両方のシステムに反映されます。

>[!NOTE]
>
>Marketo プログラムのメンバーのうち、[!DNL Salesforce] に存在しないものが存在する場合、Marketoはそれらのメンバーを [!DNL Salesforce] でリードとして作成します。

## Campaign に関連するトリガー／フィルターは何ですか。 {#what-are-the-triggers-filters-related-to-campaigns}

トリガー：

* SFDC キャンペーンに追加
* SFDC キャンペーンから削除
* SFDC キャンペーンでのステータス変更

フィルター：

* SFDC キャンペーンのメンバー

## SFDC キャンペーンに Marketo 担当者を追加できますか？ {#can-i-add-marketo-people-to-my-sfdc-campaign}

はい。[SFDC キャンペーンに追加](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/add-to-sfdc-campaign.md)フローアクションを使用します。このユーザーが [!DNL Salesforce] に存在しない場合、Marketoは [!DNL Salesforce] でこのユーザーを作成して、キャンペーンに追加します。

## Marketo を使用して SFDC キャンペーンからメンバーを削除できますか？ {#can-i-remove-members-from-my-sfdc-campaign-using-marketo}

はい。[SFDC キャンペーンから削除](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/remove-from-sfdc-campaign.md){target="_blank"}フローアクションを使用します。

## Marketo を使用してキャンペーンメンバーのステータスを変更できますか？ {#can-i-change-campaign-member-status-using-marketo}

はい。[SFDC キャンペーンのステータス変更](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md){target="_blank"}フローアクションを使用します。

## [!DNL Salesforce] キャンペーンが表示されないのはなぜですか？ {#why-cant-i-see-any-of-my-salesforce-campaigns}

次の点を確認してください。

1. [キャンペーンの同期が有効](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md)になっていることを確認します。
1. [Marketo同期ユーザー ](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) が [ の ](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md) マーケティングユーザー [!DNL Salesforce] であることを確認します。

>[!NOTE]
>
>[!DNL Salesforce] キャンペーンとマッピングされたMarketo プログラムに互換性のないプログラムステータスがある場合、エラーメッセージが表示される場合があります。 [同期前にプログラムステータスを一致させる](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md)ことがお勧めです。

>[!MORELIKETHIS]
>
>* [SFDC キャンペーンとプログラムの同期](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/sync-an-sfdc-campaign-with-a-program.md){target="_blank"}
>* [プログラムメンバーシップについて](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md){target="_blank"}
>* [キャンペーン同期の有効化／無効化](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md){target="_blank"}
>* [Marketo 同期ユーザーをマーケティングユーザーにする](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md){target="_blank"}
