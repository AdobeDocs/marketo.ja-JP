---
unique-page-id: 2953457
description: SFDC 同期 - 取引先責任者の同期 - Marketo ドキュメント - 製品ドキュメント
title: SFDC 同期 - 取引先責任者の同期
exl-id: 537bbc95-9233-4454-892e-81f962cf729d
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 73%

---

# SFDC 同期：取引先責任者の同期 {#sfdc-sync-contact-sync}

Marketoがデータベース全体を [!DNL Salesforce] と同期することをご存知ですか？ 同期し、5分待ってから、毎日、再び同期します。Marketoでの [!DNL Salesforce] ーザーの連絡先の具体的な取り扱い方法に関する詳細を以下に示します。

## 同期の方向 {#sync-direction}

取引先責任者の同期は、双方向です。[!DNL Salesforce] またはMarketoのいずれかの連絡先に変更を加えると、その変更は両方のシステムに反映されます。

## 両方のシステムで変更が同時に行われた場合はどうなりますか。 {#what-if-changes-are-made-in-both-systems-at-the-same-time}

私たちは親切だし、[!DNL Salesforce] に勝たせましょう。 このようなデータの競合が発生することは、ほとんどありません。

## 人物の Marketo の取引先責任者への変換 {#can-i-convert-a-person-into-a-contact-in-marketo}

**[顧客を変換](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md){target="_blank"}**&#x200B;フローアクションを使用することで実現できます。

>[!CAUTION]
>
>Marketo で人物をコンバージョンすると、[!DNL Salesforce] で新しいアカウントと商談が作成されます。アカウントを複製しない場合は、[!DNL Salesforce] を使用して変換します。

## 手動での取引先責任者の同期の強制 {#can-i-manually-force-a-sync-of-a-contact}

**[顧客を SFDC に同期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}**&#x200B;フローアクションを使用して、リアルタイムで同期できます。

## すべての標準フィールドの Marketo への同期 {#does-every-single-standard-field-sync-to-marketo}

すべての標準フィールドが有用というわけではなく、すべて同期されるわけではありません。カスタムフィールドはすべて同期に含めることができます。

>[!NOTE]
>
>Marketo は、Marketo 同期ユーザがアクセスできるフィールドのみを同期します。

## Marketoは [!DNL Salesforce] の検証ルールを尊重しますか？ {#will-marketo-respect-the-salesforce-validation-rules}

検証ルールが尊重され、競合が発生した場合、結果がリードのアクティビティログに記録されます。
