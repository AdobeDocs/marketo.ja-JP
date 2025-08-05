---
unique-page-id: 3571844
description: Microsoft Dynamics 同期 - 商談の同期 - Marketo ドキュメント - 製品ドキュメント
title: Microsoft Dynamics 同期 - 商談の同期
exl-id: dcb72f28-c980-4183-8473-a1e5ad0c8d3c
feature: Microsoft Dynamics
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 15%

---

# [!DNL Microsoft Dynamics] Sync: Opportunity Sync {#microsoft-dynamics-sync-opportunity-sync}

Marketoから [!DNL Dynamics] 同期は非常に強力です。 以下に、商談の同期に関するすべての詳細を示します。

## 2 つのシステム間での商談の詳細の同期方法 {#how-are-opportunity-details-kept-in-sync-between-the-two-systems}

オポチュニティの同期は、Marketoに [!DNL Dynamics] する方法の 1 つです。 [!DNL Dynamics] でオポチュニティに変更を加えると、更新はMarketoに反映されます。

## Marketoを使用して [!DNL Dynamics] でオポチュニティを作成できますか？ {#can-i-create-an-opportunity-in-dynamics-using-marketo}

いいえ、[!DNL Dynamics] でオポチュニティを作成する必要があります。作成したオポチュニティはMarketoと自動的に同期されます。

## Marketo に同期されるフィールド {#what-fields-will-sync-to-marketo}

設定の際に、[同期するフィールドを選択](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"}できます。

## アカウント/連絡先はオポチュニティにどのように関連付けられますか？ {#how-is-an-account-contact-associated-with-an-opportunity}

連絡先/アカウントをオポチュニティに関連付けるには、次の 2 つの方法があります。

* オポチュニティを作成する際に、連絡先（連絡先に対するフォームのルックアップフィールド）やアカウント（アカウントに対するフォームのルックアップフィールド）を設定できます。 どちらの場合も、これらの値は Dynamics の「見込み顧客（customerid）」フィールドに保存されます。 このフィールドは商談フォームに表示されませんが、設定から追加できます。 このフィールドには、連絡先またはアカウントの値を 1 つだけ含めることができます。 Marketoは次の機能を実行します。

   * 連絡先の値が「」に設定されていてアカウントが空のままの場合、Marketoは `opportunitycontactrole` を作成し、オポチュニティに関するアカウントを連絡先のアカウントに設定します。 連絡先にアカウントがない場合、このフィールドは空白のままになります。
   * アカウントの値が「」に設定され、連絡先が空のままの場合、Marketoは、opportunity のアカウントをこのアカウントに設定するだけです。
   * 両方の値が設定されている場合、Dynamics では customerid の値として考慮が選択されるので、動作は上記と同じになります。

* 関係者を通して：Dynamics は接続を使用して、商談を作成ページから関係者を通じて連絡を取ります。 これにより、新しい関係者ごとに `opportunitycontactrole` レコードを作成します。
