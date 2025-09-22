---
unique-page-id: 3571844
description: Microsoft Dynamics 同期 - 商談の同期 - Marketo ドキュメント - 製品ドキュメント
title: Microsoft Dynamics 同期 - 商談の同期
exl-id: dcb72f28-c980-4183-8473-a1e5ad0c8d3c
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 100%

---

# [!DNL Microsoft Dynamics] 同期：商談の同期 {#microsoft-dynamics-sync-opportunity-sync}

Marketo と [!DNL Dynamics] の同期は非常に強力です。以下に、商談の同期に関するすべての詳細を示します。

## 2 つのシステム間での商談の詳細の同期方法 {#how-are-opportunity-details-kept-in-sync-between-the-two-systems}

商談の同期は、[!DNL Dynamics] から Marketo への一方向です。[!DNL Dynamics] で商談に変更を加えると、更新内容が Marketo に反映されます。

## Marketo を使用した [!DNL Dynamics] の商談の作成 {#can-i-create-an-opportunity-in-dynamics-using-marketo}

Marketo ではなく、[!DNL Dynamics] で商談を作成する必要があります。商談は自動的に Marketo に同期されます。

## Marketo に同期されるフィールド {#what-fields-will-sync-to-marketo}

設定の際に、[同期するフィールドを選択](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"}できます。

## アカウント／取引先責任者を商談に関連付ける方法 {#how-is-an-account-contact-associated-with-an-opportunity}

アカウント／取引先責任者を商談に関連付けるには、次の 2 つの方法があります。

* 商談を作成する際に、取引先責任者（取引先責任者向けのフォーム上のルックアップフィールド）やアカウント（アカウント向けのフォーム上のルックアップフィールド）を設定できます。どちらの場合も、これらの値は Dynamics の「見込み客（customerid）」フィールドに保存されます。このフィールドは、商談フォームには表示されませんが、設定から追加できます。このフィールドには、取引先責任者またはアカウントのいずれか 1 つの値のみを含めることができます。Marketo では、次を行います。

   * 取引先責任者の値が設定され、アカウントが空のままになっている場合、Marketo では `opportunitycontactrole` を作成し、商談のアカウントを取引先責任者のアカウントに設定します。取引先責任者にアカウントがない場合、このフィールドは空のままになります。
   * アカウントの値が設定され、取引先責任者が空のままになっている場合、Marketo では商談のアカウントをこのアカウントにのみ設定します。
   * 両方の値が設定されている場合、Dynamics では customerid の値としてアカウントを選択するので、動作は上記と同じになります。

* 関係者を通じて：Dynamics は接続を使用して、商談作成ページから関係者を通じて商談を取引先責任者に接続します。このために、新しい関係者ごとに `opportunitycontactrole` レコードを作成します。
