---
unique-page-id: 4719312
description: Salesforce ピックリストの値を追加および削除する方法と、それらがMarketoに与える影響について説明します。 通知からフォームに新しい値を追加し、必要に応じて手動で値を削除します。
title: 選択リスト値の追加／削除
exl-id: f1230c43-10cb-47ff-89d7-9f835b034db0
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/dKioXsrR-JTWPgJdoLx70Dw4M56G1X6kMLL1HEO5ZTM
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b0bb9048-d951-48d8-8232-45cf248a7e27
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 244
ht-degree: 85%

---

# 選択リスト値の追加／削除 {#add-remove-picklist-values}

次は、[!DNL Salesforce] で選択リストの値を追加および削除する方法について知っておく必要があることです。

## 選択リスト値の追加 {#adding-picklist-values}

1. Salesforce で選択リストフィールドタイプに値が追加された場合、影響を受けるフォームを特定した[通知](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications.md){target="_blank"}が届きます。

   ![](assets/image2015-1-21-14-3a4-3a7.png)

1. フォームエディターに移動し、洲推奨リストに[追加の値を追加](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md){target="_blank"}します。

## 選択リスト値の削除 {#remove-picklist-values}

[!DNL Salesforce] のフィールドから選択リスト値が削除された場合、このフィールドをホストするすべてのフォームからこの値を手動で削除する必要があります。

>[!NOTE]
>
>Salesforce のリードフィールドと取引先責任者フィールドの値が異なる場合、共通の値を Marketo Engage で使用できます。

[!DNL Salesforce] のリードフィールドと取引先責任者フィールドの値が異なる場合：

1. SFDC で選択リストに値を追加すると、通知が届きます。
1. 通知を使用すると、どこで使用されているかがわかります。 これで、この新しい値を必要に応じてフォーム上のオプションとして追加できます。

SFDC リードの選択リストの値が SFDC 連絡先の選択リストと異なる場合は、共通の値がフォームのデフォルト値オプションとして使用されます。

値を選択リストから削除する場合は、フォームからオプションとして手動で削除する必要があります。
