---
unique-page-id: 3571848
description: Microsoft Dynamics 同期 - リード同期 - Marketo ドキュメント - 製品ドキュメント
title: Microsoft Dynamics 同期 - リード同期
exl-id: ea04a039-32f7-41f9-85fb-18df8e236390
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 100%

---

# [!DNL Microsoft Dynamics] 同期：リード同期 {#microsoft-dynamics-sync-lead-sync}

Marketo と [!DNL Dynamics] の同期は非常に強力です。詳細は次のとおりです。

## 2 つのシステム間で詳細を同期させる方法 {#how-are-details-kept-in-sync-between-the-two-systems}

同期は双方向です。[!DNL Dynamics] でリードに、または Marketo で人物に変更を加えると、更新内容が両方のシステムに反映されます。

>[!NOTE]
>
>削除は常に両方向に自動的に同期するわけではありません。[リードまたは連絡先の削除](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/deleting-a-lead-or-contact.md){target="_blank"}を参照してください。

## 両方のシステムの同じフィールドに変更が同時に加えられた場合はどうなりますか？（データの競合） {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

まれなことですが、人物（リード）では Marketo が、取引先責任者では [!DNL Dynamics] が優先されます。これは、人物についてはマーケティング部門が権限を持ち、取引先責任者についてはセールス（CRM）部門が公式な記録システムを持っていると考えているからです。

## Marketo を使用して [!DNL Dynamics] でリードを作成できますか？ {#can-i-create-a-lead-in-dynamics-using-marketo}

はい、[[!UICONTROL 人物を Microsoft に同期]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md)フローアクションを使用します。リードが存在しない場合、[!DNL Dynamics] にリードが作成されます。リードが存在する場合、フローステップは何も実行しません。

>[!NOTE]
>
>「[!UICONTROL 人物を Microsoft に同期]」フローアクション（トリガーキャンペーン内のみ）を使用すると、[!DNL Dynamics] でリード／取引先責任者がリアルタイムで作成されます。

## Marketo の人物を手動で [!DNL Dynamics] のリードと同期させることはできますか？ {#can-i-manually-force-a-sync-of-a-person-from-marketo-to-a-lead-in-dynamics}

いいえ、Marketo と [!DNL Dynamics] の間で更新を同期するには、自動バックグラウンド同期が唯一の方法です。[[!UICONTROL リードを Microsoft に同期]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md)フローアクションは、リードの同期を強制しません。

## Marketo と同期するフィールド {#what-fields-will-sync-to-marketo}

設定の際に、[同期するフィールドを選択](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"}できます。

## Marketo は [!DNL Dynamics] の検証ルールを遵守しますか？ {#will-marketo-respect-the-dynamics-validation-rules}

はい。データ形式が正しくない場合や、必須のフィールド情報が見つからない場合は、同期が失敗します。この場合、Marketo はユーザーのアクティビティログに結果を記録します。
