---
unique-page-id: 3571844
description: Microsoft Dynamics 同期 - 商談の同期 - Marketo ドキュメント - 製品ドキュメント
title: Microsoft Dynamics 同期 - 商談の同期
exl-id: dcb72f28-c980-4183-8473-a1e5ad0c8d3c
feature: Microsoft Dynamics
source-git-commit: 9a130e0b2ec84b638adf37188b65b565b090fe1b
workflow-type: tm+mt
source-wordcount: '311'
ht-degree: 29%

---

# Microsoft Dynamics 同期：商談の同期 {#microsoft-dynamics-sync-opportunity-sync}

Marketo Engageから Dynamics への同期は非常に強力です。 オポチュニティ同期の詳細はすべて次のとおりです。

## 2 つのシステム間での商談の詳細の同期方法 {#how-are-opportunity-details-kept-in-sync-between-the-two-systems}

商談の同期は、Dynamics から Marketo への一方向です。Dynamics で商談に変更を加えると、更新内容が Marketo に反映されます。

## Marketo を使用した Dynamics の商談の作成 {#can-i-create-an-opportunity-in-dynamics-using-marketo}

Marketo ではなく、Dynamics で商談を作成する必要があります。商談は自動的に Marketo に同期されます。

## Marketo に同期されるフィールド {#what-fields-will-sync-to-marketo}

設定の際に、[同期するフィールドを選択](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"}できます。

## アカウント/連絡先は商談にどのように関連付けられていますか？ {#how-is-an-account-contact-associated-with-an-opportunity}

連絡先/アカウントは、次の 2 つの方法で商談に関連付けることができます。

* オポチュニティを作成する際に、連絡先（連絡先のフォーム上の参照フィールド）やアカウント（連絡先のフォーム上の参照フィールド）を設定できます。 どちらの場合も、これらの値は、Dynamics の「潜在的な顧客 (customerid) 」フィールドに格納されます。 このフィールドは商談フォームには表示されませんが、設定から追加できます。 このフィールドには、連絡先またはアカウントの値を 1 つだけ含めることができます。 Marketoは次の操作を実行します。

   * 連絡先の値が設定され、アカウントが空のままの場合、Marketoは `opportunitycontactrole` また、商談のアカウントを連絡先のアカウントに設定します。 連絡先にアカウントがない場合、このフィールドは空のままです。
   * アカウントの値が設定され、連絡先が空の場合、Marketoはオポチュニティ上のアカウントをこのアカウントに対してのみ設定します。
   * 両方の値が設定されている場合、Dynamics は customerid の値としてアカウントを選択するので、動作は上記と同じになります。


* 関係者を通じて： Dynamics は接続を使用して、オポチュニティ作成ページから関係者を通じて連絡する機会を結び付けます。 このために、 `opportunitycontactrole` 新規の関係者全員に対する記録
