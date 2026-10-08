---
description: EnterpriseまたはUnlimitedの最後の手順で、MarketoとSalesforceを連携する方法について説明します。 Marketo Adminで、sync ユーザーセキュリティトークンを取得し、資格情報を設定します。
title: ステップ 3/3 - MarketoとSalesforceを接続する（Enterprise/Unlimited）
hide: true
hidefromtoc: 'yes'
feature: Salesforce Integration
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
subfeature_v2:
  - id: edcca97f-2314-445f-9a79-3ac30a2a9c27
    internal-label: Salesforce integration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '123'
ht-degree: 70%
---
# 手順 3 / 3：Marketo と Salesforce の接続（Enterprise／Unlimited） {#step-of-connect-marketo-and-salesforce-enterprise-unlimited}

この記事では、設定済みの Salesforce インスタンスと同期するように Marketo を設定します。

>[!PREREQUISITES]
>
>* [手順 1／3：Marketo フィールドの Salesforce への追加（Enterprise／Unlimited）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md){target="_blank"}
>* [手順 2 / 3：Marketo 用の Salesforce ユーザの作成（Enterprise／Unlimited）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"}

## 同期ユーザーセキュリティトークンの取得 {#retrieve-sync-user-security-token}

>[!TIP]
>
>セキュリティトークンを既に取得済みの場合は、「同期ユーザー資格情報の設定」に直接進んでください。事前準備ができているのは素晴らしいことです。

1. Marketo 同期ユーザーで Salesforce にログインし、同期ユーザーの名前をクリックしてから、「**[!UICONTROL マイ設定]**」をクリックします。
