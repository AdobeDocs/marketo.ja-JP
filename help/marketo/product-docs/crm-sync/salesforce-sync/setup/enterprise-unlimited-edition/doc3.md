---
description: エンタープライズまたは無制限の最後の手順で、MarketoとSalesforceを接続する方法について説明します。 同期ユーザーセキュリティトークンを取得し、Marketo Admin で資格情報を設定します。
title: 手順 3/3 - MarketoとSalesforceの接続（Enterprise/Unlimited）
hide: true
hidefromtoc: true
feature: Salesforce Integration
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '123'
ht-degree: 70%

---

# 手順 3 / 3：Marketo と Salesforce の接続（Enterprise／Unlimited） {#step-of-connect-marketo-and-salesforce-enterprise-unlimited}

この記事では、設定済みの Salesforce インスタンスと同期するように Marketo を設定します。

>[!PREREQUISITES]
>
>* [手順 1／3：Marketo フィールドの Salesforce への追加（Enterprise／Unlimited）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md){target="_blank"}
>* [手順 2 / 3：Marketo 用の Salesforce ユーザーの作成（Enterprise／Unlimited）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"}

## 同期ユーザーセキュリティトークンの取得 {#retrieve-sync-user-security-token}

>[!TIP]
>
>既にセキュリティトークンを持っている場合は、直接「同期ユーザー資格情報の設定」に進んで、準備を完了させます。

1. Marketo 同期ユーザで Salesforce にログインし、同期ユーザの名前をクリックしてから、「**[!UICONTROL マイ設定]**」をクリックします。
