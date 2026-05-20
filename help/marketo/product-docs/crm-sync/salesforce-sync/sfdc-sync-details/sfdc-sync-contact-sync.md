---
unique-page-id: 2953457
description: SalesforceとMarketo間の連絡先の同期の仕組みについて説明します。 双方向の同期を理解し、人物を連絡先に変換し、フローアクションとの強制的な同期を実現します。
title: SFDC 同期 - 取引先責任者の同期
exl-id: 537bbc95-9233-4454-892e-81f962cf729d
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/bddyM2G50v-Hgdy1oHw8xIPw1zij-2JvGSU7se3-UfI
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: c5f60233-d5ea-4453-a799-0ad258b4d399
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 243
ht-degree: 83%

---

# SFDC 同期：取引先責任者の同期 {#sfdc-sync-contact-sync}

Marketoは、データベース全体を[!DNL Salesforce]と同期します。 同期し、5 分待ってから、毎日、再び同期します。 ここでは、Marketo が [!DNL Salesforce] の取引先責任者をどのように扱っているかを詳しく説明します。

## 同期の方向 {#sync-direction}

取引先責任者の同期は、双方向です。 [!DNL Salesforce] または Marketo で取引先責任者に変更を加えると、更新内容が両方のシステムに反映されます。

## 両方のシステムで変更が同時に行われた場合 {#what-if-changes-are-made-in-both-systems-at-the-same-time}

[!DNL Salesforce] での変更を優先します。 このようなデータの衝突が起こることは稀です。

## 人物の Marketo の取引先責任者への変換 {#can-i-convert-a-person-into-a-contact-in-marketo}

**[顧客を変換](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md){target="_blank"}**&#x200B;フローアクションを使用することで実現できます。

>[!CAUTION]
>
>Marketo で人物をコンバージョンすると、[!DNL Salesforce] で新しいアカウントと商談が作成されます。 アカウントを重複させたくない場合は、[!DNL Salesforce] を使用して変換します。

## 手動での取引先責任者の同期の強制 {#can-i-manually-force-a-sync-of-a-contact}

**[顧客を SFDC に同期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}**&#x200B;フローアクションを使用して、リアルタイムで同期できます。

## すべての標準フィールドの Marketo への同期 {#does-every-single-standard-field-sync-to-marketo}

すべての標準フィールドが有用というわけではなく、すべて同期されるわけではありません。 カスタムフィールドはすべて同期に含めることができます。

>[!NOTE]
>
>Marketo は、Marketo 同期ユーザがアクセスできるフィールドのみを同期します。

## Marketo は [!DNL Salesforce] の検証ルールを遵守しますか？ {#will-marketo-respect-the-salesforce-validation-rules}

検証ルールが尊重され、競合が発生した場合、結果がリードのアクティビティログに記録されます。
