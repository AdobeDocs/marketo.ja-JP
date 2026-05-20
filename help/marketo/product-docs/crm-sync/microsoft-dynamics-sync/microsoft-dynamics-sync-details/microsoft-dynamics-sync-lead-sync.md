---
unique-page-id: 3571848
description: Microsoft DynamicsとMarketo間のリードシンクの仕組みについて説明します。 Microsoftに個人を同期することで、双方向の同期を把握し、リードを作成できます。
title: Microsoft Dynamics 同期 - リード同期
exl-id: ea04a039-32f7-41f9-85fb-18df8e236390
feature: Microsoft Dynamics
TQID: https://experienceleague.adobe.com/BB-28aHosrt72difKAr7vgYqdI8a9ts0aOSnbWJzbw8
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 309
ht-degree: 79%

---

# [!DNL Microsoft Dynamics] 同期：リード同期 {#microsoft-dynamics-sync-lead-sync}

Marketoから[!DNL Dynamics]への同期は強力です。 詳細は次のとおりです。

## 2 つのシステム間で詳細を同期させる方法 {#how-are-details-kept-in-sync-between-the-two-systems}

同期は双方向です。 [!DNL Dynamics] でリードに、または Marketo で人物に変更を加えると、更新内容が両方のシステムに反映されます。

>[!NOTE]
>
>削除は常に両方向に自動的に同期するわけではありません。 [リードまたは連絡先の削除](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/deleting-a-lead-or-contact.md){target="_blank"}を参照してください。

## 両方のシステムの同じフィールドに同時に変更が加えられた場合の動作 （データの競合） {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

まれなことですが、人物（リード）では Marketo が、取引先責任者では [!DNL Dynamics] が優先されます。 これは、マーケティング部門が個人の権威と考えられているのに対し、コンタクト先の正式な記録システムはセールス（CRM）部門に属しているためです。

## Marketo を使用して [!DNL Dynamics] でリードを作成できますか？ {#can-i-create-a-lead-in-dynamics-using-marketo}

はい、[[!UICONTROL 人物を Microsoft に同期]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md)フローアクションを使用します。 この操作により、リードが存在しない場合は[!DNL Dynamics]にリードが作成されます。 リードが存在する場合、フローステップは何も実行しません。

>[!NOTE]
>
>「[!UICONTROL 人物を Microsoft に同期]」フローアクション（トリガーキャンペーン内のみ）を使用すると、[!DNL Dynamics] でリード／取引先責任者がリアルタイムで作成されます。

## Marketo の人物を手動で [!DNL Dynamics] のリードと同期させることはできますか？ {#can-i-manually-force-a-sync-of-a-person-from-marketo-to-a-lead-in-dynamics}

いいえ、Marketo と [!DNL Dynamics] の間で更新を同期するには、自動バックグラウンド同期が唯一の方法です。 [[!UICONTROL リードを Microsoft に同期]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md)フローアクションは、リードの同期を強制しません。

## Marketo に同期されるフィールド {#what-fields-will-sync-to-marketo}

設定の際に、[同期するフィールドを選択](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"}できます。

## Marketo は [!DNL Dynamics] の検証ルールを遵守しますか？ {#will-marketo-respect-the-dynamics-validation-rules}

はい。 データ形式が正しくない場合や、必須フィールドの情報が見つからない場合は、同期が失敗します。 この場合、Marketo はユーザーのアクティビティログに結果を記録します。
