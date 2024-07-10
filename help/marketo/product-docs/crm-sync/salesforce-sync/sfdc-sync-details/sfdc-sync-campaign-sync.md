---
unique-page-id: 2953469
description: SFDC の同期 - キャンペーンの同期 - Marketo ドキュメント - 製品ドキュメント
title: SFDC の同期 - キャンペーンの同期
exl-id: 62435e00-9c59-4dee-a9b7-ccf1d1f41b78
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: ht
source-wordcount: '377'
ht-degree: 100%

---

# SFDC 同期：キャンペーンの同期 {#sfdc-sync-campaign-sync}

Marketo Engageプログラムは、Salesforce キャンペーンと同期できます。この機能の概要を次に示します。

## Marketo プログラムを Salesforce キャンペーンと同期する理由 {#why-should-i-sync-marketo-programs-with-salesforce-campaigns}

* Marketo Program の強力な機能を使用する。
* Marketo プログラムと Salesforce キャンペーンの間で、メンバーとステータスの同期を維持する。
* Marketo と Salesforce のレポート機能を使用する。

## Marketo プログラムと Salesforce キャンペーンが同期される方法 {#how-is-a-marketo-program-and-a-salesforce-campaign-synced}

Marketo では、プログラムと Salesforce キャンペーンの間に 1 対 1 のマッピングを作成するオプションがあります。

![](assets/image2015-7-8-9-3a43-3a8.png)

Marketo の&#x200B;**[チャネル](/help/marketo/product-docs/administration/tags/create-a-program-channel.md){target="_blank"}**&#x200B;と&#x200B;**[期間原価](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-period-costs.md){target="_blank"}**&#x200B;は、**種別**&#x200B;および&#x200B;**キャンペーンの実費**&#x200B;として Salesforce に同期されます。 この同期は Marketo から Salesforce への&#x200B;**一方向**&#x200B;です。

Marketo の&#x200B;**プログラムメンバー**&#x200B;と&#x200B;**[進行状況のステータス](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md){target="_blank"}**&#x200B;は、**Salesforce キャンペーンメンバー**&#x200B;と&#x200B;**キャンペーンメンバーステータス**&#x200B;に同期されます。これは、**双方向同期**&#x200B;であるため、Marketo または Salesforce でおこなわれた変更は両方のシステムに反映されます。

>[!NOTE]
>
>Marketo プログラムに Salesforce に存在しないメンバーがいる場合、Marketo はそれらのメンバーを Salesforce 内のリードとして作成します。

## Campaign に関連するトリガー／フィルターは何ですか。 {#what-are-the-triggers-filters-related-to-campaigns}

トリガー：

* SFDC キャンペーンに追加
* SFDC キャンペーンから削除
* SFDC キャンペーンでのステータス変更

フィルター：

* SFDC キャンペーンのメンバー

## SFDC キャンペーンに Marketo 担当者を追加できますか？ {#can-i-add-marketo-people-to-my-sfdc-campaign}

はい。[SFDC キャンペーンに追加](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/add-to-sfdc-campaign.md){target="_blank"}フローアクションを使用します。この人物が Salesforce に存在しない場合、Marketo は Salesforce で作成し、キャンペーンに追加します。

## Marketo を使用して SFDC キャンペーンからメンバーを削除できますか？ {#can-i-remove-members-from-my-sfdc-campaign-using-marketo}

はい。[SFDC キャンペーンから削除](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/remove-from-sfdc-campaign.md){target="_blank"}フローアクションを使用します。

## Marketo を使用してキャンペーンメンバーのステータスを変更できますか？ {#can-i-change-campaign-member-status-using-marketo}

はい。[SFDC キャンペーンのステータス変更](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md){target="_blank"}フローアクションを使用します。

## Salesforce キャンペーンが表示されないのはなぜですか？ {#why-cant-i-see-any-of-my-salesforce-campaigns}

次の点を確認してください。

1. [キャンペーンの同期が有効](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md){target="_blank"}になっていることを確認します。
1. [Marketo 同期ユーザー](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"}が、Salesforce で[マーケティングユーザー](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md){target="_blank"}になっていることを確認します。

>[!NOTE]
>
>Salesforce キャンペーンとマッピングされた Marketo プログラムに互換性のないプログラムステータスがある場合、エラーメッセージが表示されることがあります。[同期前にプログラムステータスを一致させる](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md){target="_blank"}ことがお勧めです。

>[!MORELIKETHIS]
>
>* [SFDC キャンペーンとプログラムの同期](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/sync-an-sfdc-campaign-with-a-program.md){target="_blank"}
>* [プログラムメンバーシップについて](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md){target="_blank"}
>* [キャンペーン同期の有効化／無効化](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md){target="_blank"}
>* [Marketo 同期ユーザーをマーケティングユーザーにする](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md){target="_blank"}
