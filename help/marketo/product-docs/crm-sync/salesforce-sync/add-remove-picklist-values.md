---
unique-page-id: 4719312
description: Picklist値の追加削除 — Marketto Docs — 製品ドキュメント
title: Picklist値追加/Remove Picklist Values
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
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
>Salesforceのリードフィールドと連絡先フィールドの値が異なる場合、共通の値がMarketoで使用できます。

Salesforceのリードフィールドと連絡先フィールドの値が異なる場合：

1. SFDCに値を追加すると、ピックリストに通知が送信されます。
1. 通知は、その通知がどこで使用されたかを示します。 これで、この新しい値を必要に応じてフォーム上のオプションとして追加できます。

SFDCリードの選択リストの値がSFDC担当者の選択リストと異なる場合は、フォームのデフォルト値オプションとして共通の値が使用されます。

選択リストから値を削除する場合は、フォームからオプションとして手動で値を削除する必要があります。
