---
unique-page-id: 4719312
description: 選択リスト値追加の削除 —Marketoドキュメント — 製品ドキュメント
title: Picklist値追加/Remove Picklist Values
exl-id: f1230c43-10cb-47ff-89d7-9f835b034db0
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---

# 追加/Remove Picklist Values {#add-remove-picklist-values}

Salesforceでの選択リスト値の追加と削除について知っておくべきことを以下に示します。

## 選択リスト値の追加{#adding-picklist-values}

1. Salesforceにpicklistフィールドタイプに値が追加されると、[通知](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications.md)が送信され、これがどのフォームに影響を与えるかがわかります。

   ![](assets/image2015-1-21-14-3a4-3a7.png)

1. フォームエディターに移動し、[提案のリストに追加の値](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md)を追加します。

## 選択リスト値の削除{#remove-picklist-values}

Salesforceのフィールドからpicklist値が削除された場合、このフィールドをホストするすべてのフォームから、この値を手動で削除する必要があります。

>[!NOTE]
>
>Salesforceのリードフィールドと連絡先フィールドの値が異なる場合、共通の値はMarketoで使用できます。

Salesforceのリードフィールドと連絡先フィールドの値が異なる場合：

1. SFDCに値を追加すると、ピックリストに通知が送信されます。
1. 通知は、その通知がどこで使用されたかを示します。 これで、この新しい値を必要に応じてフォーム上のオプションとして追加できます。

SFDCリードの選択リストの値がSFDC担当者の選択リストと異なる場合は、フォームのデフォルト値オプションとして共通の値が使用されます。

選択リストから値を削除する場合は、フォームからオプションとして手動で値を削除する必要があります。
