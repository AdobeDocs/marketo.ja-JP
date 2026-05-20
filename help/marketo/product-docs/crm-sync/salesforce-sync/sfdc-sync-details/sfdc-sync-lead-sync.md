---
unique-page-id: 2953455
description: SalesforceとMarketo間のリードシンクの仕組みについて説明します。 双方向の同期を理解し、Marketoからリードを作成し、検証ルールを尊重します。
title: SFDC 同期 - リードの同期
exl-id: cf38e091-7344-4b95-b9e1-77eda751c4a9
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/zqztwtX4Xe08Df-v1aTxhRi-cB2CZALctr3kaFNrT7s
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: c5f60233-d5ea-4453-a799-0ad258b4d399
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 242
ht-degree: 84%

---

# SFDC 同期：リードの同期 {#sfdc-sync-lead-sync}

Marketoは、[!DNL Salesforce] データベースから同期します。 同期して 5 分待機し、その後また同期するという処理を 一日中、毎日繰り返しおこなっています。 ここでは、Marketo が [!DNL Salesforce] のリードをどのように扱っているかを詳しく説明します。

## 同期の方向 {#sync-direction}

リード（顧客）とコンタクトの同期は双方向です。 [!DNL Salesforce] または Marketo のレコードに変更を加えると、更新内容が両方のシステムに反映されます。

## 両方のシステムで変更が同時に行われた場合 {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Marketo が優先されます。 このようなデータの衝突が起こることは稀です。

## Marketo を使用して [!DNL Salesforce] でリードを作成することはできますか？ {#can-i-create-a-lead-in-salesforce-using-marketo}

はい、「[人物を SFDC に同期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)」フローアクションを使用します。 リードが存在しない場合、[!DNL Salesforce] にリードが作成されます。

## Marketo の人物を手動で [!DNL Salesforce] のリードと同期させることはできますか？ {#can-i-manually-force-a-sync-of-a-person-in-marketo-to-a-lead-in-salesforce}

[顧客を SFDC に同期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}フローアクションを使用して、リアルタイムで同期できます。

## すべての標準フィールドの Marketo への同期 {#does-every-single-standard-field-sync-to-marketo}

すべての標準フィールドが有用というわけではなく、すべて同期されるわけではありません。 カスタムフィールドはすべて同期に含めることができます。

>[!NOTE]
>
>Marketoは、[!DNL Salesforce] 同期ユーザがアクセスできるフィールドのみを同期します。

## Marketo は [!DNL Salesforce] の検証ルールを遵守しますか？ {#will-marketo-respect-the-salesforce-validation-rules}

はい。 データ形式が正しくない場合や、必須フィールドの情報が見つからない場合は、同期が失敗します。 この場合、Marketo はリードのアクティビティログに結果を記録します。
