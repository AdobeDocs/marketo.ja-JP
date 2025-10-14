---
description: ' [!DNL Veeva] CRM 同期について – Marketo ドキュメント – 製品ドキュメント'
title: ' [!DNL Veeva] CRM 同期について'
exl-id: 99ade106-7f32-40e8-8b9a-2b1d0e769b9c
feature: Veeva CRM
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 28%

---

# [!DNL Veeva] CRM 同期について {#understanding-the-veeva-crm-sync}

いくつかの簡単な手順で、Adobe Marketo Engageと [!DNL Veeva] CRM の間の同期を簡単に実行できます。

## 同期の仕組み {#how-the-sync-works}

Marketo Engageは [!DNL Veeva] CRM と毎日同期されます。 各同期はいくらか時間がかかり、5 分間一時停止してから再び開始します。

>[!NOTE]
>
>Marketo Engageが [!DNL Veeva] からデータベース全体をコピーしているので、最初の同期には数時間または数日かかる場合があります。 その後、各同期には、通常、数分（場合によっては数秒）かかり、変更されたデータのみが同期されます。

![](assets/understanding-the-veeva-sync-1.png)

[!DNL Veeva] とMarketo Engageの同期は、人物アカウントオブジェクトの連絡先フィールドに対してのみ双方向です。 このような場合、[!DNL Veeva] またはMarketo Engageで変更を加えるたびに、その変更が両方のシステムに反映されます。 その他の同期はすべて [!DNL Veeva] からMarketo Engageへの同期のみです。 詳しくは、次のリンクをクリックしてください。

## Marketo Engageと [!DNL Veeva] の間で同期されるもの {#what-is-synced-between-marketo-engage-and-veeva}

* [&#x200B; 人物アカウント &#x200B;](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/person-account-sync-faq.md){target="_blank"}
* ユーザ
* [Call および Call Key オブジェクト &#x200B;](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
* [カスタムオブジェクト](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/custom-object-sync.md){target="_blank"}

## 留意事項 {#things-to-know}

* [Marketo Engageに入力する資格情報  [!DNL Veeva]](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"} は、データの同期に使用されます。 その資格情報でアクセスできるデータのみが含まれます。

* CRM[!DNL Veeva]force.comに基づいており、Marketo Engageとプラットフォームの間で行われた豊富なエクスペリエンスがこの同期に継承されます。

* Veeva CRM には、リード、連絡先、アカウント、ビジネスアカウント、オポチュニティ、キャンペーンおよびアクティビティが表示されます。 ただし、Marketo Engage との同期ではサポートされていません。
