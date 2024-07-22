---
unique-page-id: 3571848
description: Microsoft Dynamics 同期 - リード同期 - Marketo ドキュメント - 製品ドキュメント
title: Microsoft Dynamics 同期 - リード同期
exl-id: ea04a039-32f7-41f9-85fb-18df8e236390
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 89%

---

# Microsoft Dynamics 同期：リード同期 {#microsoft-dynamics-sync-lead-sync}

DynamicsMarketo Engageは非常に強力です。 詳細は以下の通りです。

## 2 つのシステム間で詳細を同期させる方法 {#how-are-details-kept-in-sync-between-the-two-systems}

同期は双方向です。Dynamics のリードまたは Marketo のリードに変更を加えると、両方のシステムに更新が反映されます。

>[!NOTE]
>
>削除は常に両方向に自動的に同期するわけではありません。[リードまたは連絡先の削除](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/deleting-a-lead-or-contact.md){target="_blank"}を参照してください。

## 両方のシステムの同じフィールドに変更が同時に加えられた場合はどうなりますか？（データの競合） {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

これが起こることは稀ですが、リードの場合は Marketo の変更が反映され、連絡先の場合は Dynamics の変更が反映されます。これは、リードに対してはマーケティング部門が権限を持ち、連絡先の正式な記録はセールス（CRM）部門が持つという考えによるものです。

## Marketo を使用して Dynamics でリードを作成できますか？ {#can-i-create-a-lead-in-dynamics-using-marketo}

はい、[リードを Microsoft に同期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md){target="_blank"}フローアクションを使用します。リードが存在しない場合、Dynamics にリードが作成されます。リードが存在する場合、フローステップは何も実行しません。

>[!NOTE]
>
>「ユーザーをMicrosoftに同期」フローアクションを使用する場合（トリガーキャンペーンでのみ）、リード/連絡先は Dynamics でリアルタイムに作成されます。

## 手動で Marketo のリードを Dynamics のリードに同期させることはできますか？ {#can-i-manually-force-a-sync-of-a-person-from-marketo-to-a-lead-in-dynamics}

いいえ。自動バックグラウンド同期は、Marketo と Dynamics の間で更新を同期する唯一の方法です。[リードを Microsoft に同期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md){target="_blank"}フローアクションは、リードの同期を強制しません。

## Marketo と同期するフィールド {#what-fields-will-sync-to-marketo}

設定時に[同期するフィールドを選択](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"}できます。

## Marketo は Dynamics 検証ルールを遵守しますか？ {#will-marketo-respect-the-dynamics-validation-rules}

はい。データ形式が正しくない場合や、必須のフィールド情報が見つからない場合は、同期が失敗します。この場合、Marketo はユーザーのアクティビティログに結果を記録します。
