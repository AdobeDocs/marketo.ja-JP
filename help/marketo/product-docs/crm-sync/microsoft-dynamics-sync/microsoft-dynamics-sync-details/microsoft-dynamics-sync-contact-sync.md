---
unique-page-id: 3571833
description: Microsoft Dynamics 同期 - 連絡先の同期 - Marketo ドキュメント - 製品ドキュメント
title: Microsoft Dynamics 同期 - 連絡先の同期
exl-id: d4583ea0-2b52-415e-b28c-a8eafebeff64
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 87%

---

# Microsoft Dynamics 同期：連絡先の同期 {#microsoft-dynamics-sync-contact-sync}

Marketo Engageがデータベース全体を Dynamics と同期することを知っていましたか？ 同期した後、5 分待ってからまた同期するということを、1 日中、毎日繰り返しています。ここでは、Marketo が Dynamics の連絡先をどのように扱っているかを詳しく説明します。

## 2 つのシステム間での詳細の同期方法 {#how-are-details-kept-in-sync-between-the-two-systems}

連絡先の同期は、双方向です。Dynamics で連絡先に、または Marketo で人物に変更を加えると、更新内容が両方のシステムに反映されます。

## 両方のシステムの同じフィールドに同時に変更が加えられた場合の動作（データの競合） {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

めったにないことですが、人物では Marketo が、連絡先では Dynamics  が優先されます。これは、人物についてはマーケティング部門が権限を持ち、連絡先についてはセールス（CRM）部門が公式な記録システムを持っていると考えているからです。

## Marketo を使用した連絡先の作成 {#can-i-create-a-contact-using-marketo}

はい。[以下に手順を示します](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync/create-a-contact-in-microsoft-dynamics.md){target="_blank"}。

>[!NOTE]
>
>「ユーザーをMicrosoftに同期」フローアクションを使用する場合（トリガーキャンペーンでのみ）、リード/連絡先は Dynamics でリアルタイムに作成されます。

## 手動での人物または連絡先の同期の強制 {#can-i-manually-force-a-sync-of-a-person-or-a-contact}

手動で強制的に同期することはできません。Marketo と Dynamics の間で更新を同期するには、自動バックグラウンド同期が唯一の方法です。[担当者を Microsoft に同期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md){target="_blank"}は、リードの同期を強制するものではありません。

## Marketo に同期されるフィールド {#what-fields-will-sync-to-marketo}

設定の際に、[同期するフィールドを選択](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"}できます。ただし、Marketo は、Dynamics 同期ユーザーがアクセスできるフィールドのみを同期します。

## Marketo による Dynamics の検証ルールの尊重 {#will-marketo-respect-the-dynamics-validation-rules}

検証ルールが尊重され、競合が発生した場合、結果がリードのアクティビティログに記録されます。
