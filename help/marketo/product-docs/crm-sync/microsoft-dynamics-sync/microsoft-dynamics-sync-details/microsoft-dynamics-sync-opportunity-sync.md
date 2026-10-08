---
unique-page-id: 3571844
description: Microsoft DynamicsからMarketoへの商談シンクの仕組みについて説明します。 一方向の同期と、機会が連絡先やリードにどのように関連付けられるかを把握します。
title: Microsoft Dynamics 同期 - 商談の同期
exl-id: dcb72f28-c980-4183-8473-a1e5ad0c8d3c
feature: Microsoft Dynamics
TQID: 'https://experienceleague.adobe.com/vDSWrvMSvAa2-XSn6A-lcZYaoWRjrtKwsLo1fJvPAkg'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
subfeature_v2:
  - id: d5c7388a-594e-4d15-9b39-98d6ce479e8b
    internal-label: Microsoft Dynamics
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 83%
---
# [!DNL Microsoft Dynamics] 同期：商談の同期 {#microsoft-dynamics-sync-opportunity-sync}

Marketoから[!DNL Dynamics]への同期は強力です。 以下に、商談の同期に関するすべての詳細を示します。

## 2 つのシステム間で商談の詳細はどのように同期されますか？ {#how-are-opportunity-details-kept-in-sync-between-the-two-systems}

商談の同期は、[!DNL Dynamics] から Marketo への一方向です。 [!DNL Dynamics] で商談に変更を加えると、更新内容が Marketo に反映されます。

## Marketo を使用した [!DNL Dynamics] の商談の作成 {#can-i-create-an-opportunity-in-dynamics-using-marketo}

Marketo ではなく、[!DNL Dynamics] で商談を作成する必要があります。商談は自動的に Marketo に同期されます。

## Marketo に同期されるフィールド {#what-fields-will-sync-to-marketo}

設定の際に、[同期するフィールドを選択](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"}できます。

## アカウント／取引先責任者はどのように商談に関連付けられますか？ {#how-is-an-account-contact-associated-with-an-opportunity}

取引先責任者／アカウントを商談に関連付ける方法は、次の 2 通りあります。

* 商談を作成する際に、取引先責任者（取引先責任者向けのフォーム上のルックアップフィールド）および／またはアカウント（アカウント向けのフォーム上のルックアップフィールド）を設定できます。 どちらの場合も、これらの値は Dynamics の「見込み顧客（customerid）」フィールドに保存されます。 このフィールドは、商談フォームには表示されませんが、設定から追加できます。 このフィールドには、取引先責任者またはアカウントのいずれか 1 つの値のみを含めることができます。 Marketo では、次を行います。

  * 取引先責任者の値が設定され、アカウントが空のままになっている場合、Marketo では `opportunitycontactrole` を作成し、商談のアカウントを取引先責任者のアカウントに設定します。 連絡先にアカウントがない場合、このフィールドは空のままになります。
  * アカウントの値が設定され、取引先責任者が空のままになっている場合、Marketo は商談のアカウントとしてこのアカウントのみを設定します。
  * 両方の値が設定されている場合、Dynamics は customerid の値としてアカウントを選択するため、動作は上記と同じになります。

* 関係者を通じて：Dynamics は接続を使用して、商談作成ページから関係者を通じて商談を取引先責任者に接続します。 このために、新しい関係者ごとに`opportunitycontactrole` レコードが作成されます。
