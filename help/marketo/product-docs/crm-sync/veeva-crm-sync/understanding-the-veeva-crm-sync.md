---
description: Marketo Engageと Veeva の間で Veeva CRM 同期がどのように機能するかを説明します。 同期を実行して、人物アカウントやカスタムオブジェクトなど、同期された内容を確認します。
title: ' [!DNL Veeva]  CRM 同期について'
exl-id: 99ade106-7f32-40e8-8b9a-2b1d0e769b9c
feature: Veeva CRM
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 89%

---

# [!DNL Veeva] CRM 同期について {#understanding-the-veeva-crm-sync}

簡単な手順で Adobe Marketo Engage と [!DNL Veeva] CRM 間の同期を簡単に実行できます。

## 同期の仕組み {#how-the-sync-works}

Marketo Engage は、毎日、常に [!DNL Veeva] CRM と同期します。各同期はいくらか時間がかかり、5 分間一時停止してから再び開始します。

>[!NOTE]
>
>最初の同期には、Marketo Engage が [!DNL Veeva] からデータベース全体をコピーするので、数時間から数日かかる場合があります。その後、各同期には、通常、数分（場合によっては数秒）かかり、変更されたデータのみが同期されます。

![](assets/understanding-the-veeva-sync-1.png)

[!DNL Veeva] と Marketo Engage の同期は、個人取引先オブジェクトの取引先責任者フィールドに対してのみ双方向です。この場合、[!DNL Veeva] または Marketo Engage で変更を加えるたびに、更新内容が両方のシステムに反映されます。その他のすべての同期は、[!DNL Veeva] から Marketo Engage に対してのみです。詳しくは、次のリンクをクリックしてください。

## Marketo Engage と [!DNL Veeva] の間で同期されるもの {#what-is-synced-between-marketo-engage-and-veeva}

* [個人取引先](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/person-account-sync-faq.md){target="_blank"}
* ユーザ
* [呼び出しおよび呼び出しキーオブジェクト](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
* [カスタムオブジェクト](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/custom-object-sync.md){target="_blank"}

## 留意事項 {#things-to-know}

* [ [!DNL Veeva]](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"} 用に Marketo で入力した資格情報は、データの同期に使用されます。その資格情報でアクセスできるデータのみが含まれます。

* [!DNL Veeva] CRM は force.com に基づいており、Marketo Engage のプラットフォームによるリッチエクスペリエンスが、この同期に継承されます。

* Veeva CRM には、リード、取引先責任者、アカウント、ビジネスアカウント、商談、キャンペーン、アクティビティが表示されます。ただし、Marketo Engage との同期ではサポートされていません。
