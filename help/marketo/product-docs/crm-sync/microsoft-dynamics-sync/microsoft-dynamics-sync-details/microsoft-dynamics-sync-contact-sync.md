---
unique-page-id: 3571833
description: Microsoft Dynamics 同期 - 連絡先の同期 - Marketo ドキュメント - 製品ドキュメント
title: Microsoft Dynamics 同期 - 連絡先の同期
exl-id: d4583ea0-2b52-415e-b28c-a8eafebeff64
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 100%

---

# [!DNL Microsoft Dynamics] 同期：取引先責任者の同期 {#microsoft-dynamics-sync-contact-sync}

Marketo がデータベース全体を [!DNL Dynamics] と同期しているのを知っていましたか？同期し、5 分待ってから、毎日、再び同期します。ここでは、Marketo が [!DNL Dynamics] の取引先責任者をどのように扱っているかを詳しく説明します。

## 2 つのシステム間での詳細の同期方法 {#how-are-details-kept-in-sync-between-the-two-systems}

連絡先の同期は、双方向です。[!DNL Dynamics] で取引先責任者に、または Marketo で人物に変更を加えると、更新内容が両方のシステムに反映されます。

## 両方のシステムの同じフィールドに同時に変更が加えられた場合の動作（データの競合） {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

人物では Marketo が、取引先責任者では [!DNL Dynamics] が優先される場合がまれにあります。これは、人物についてはマーケティング部門が権限を持ち、取引先責任者についてはセールス（CRM）部門が公式な記録システムを持っていると考えているからです。

## Marketo を使用した連絡先の作成 {#can-i-create-a-contact-using-marketo}

はい。[以下に手順を示します](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync/create-a-contact-in-microsoft-dynamics.md){target="_blank"}。

>[!NOTE]
>
>「人物を Microsoft に同期」フローアクション（トリガーキャンペーン内のみ）を使用すると、[!DNL Dynamics] でリード／取引先責任者がリアルタイムで作成されます。

## 手動での人物または連絡先の同期の強制 {#can-i-manually-force-a-sync-of-a-person-or-a-contact}

手動で強制的に同期することはできません。Marketo と [!DNL Dynamics] の間で更新を同期するには、自動バックグラウンド同期が唯一の方法です。[担当者を Microsoft に同期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md)は、リードの同期を強制するものではありません。

## Marketo に同期されるフィールド {#what-fields-will-sync-to-marketo}

設定の際に、[同期するフィールドを選択](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync)できます。ただし、Marketoは、[!DNL Dynamics] 同期ユーザがアクセスできるフィールドのみを同期します。

## Marketo は [!DNL Dynamics] の検証ルールを遵守しますか？ {#will-marketo-respect-the-dynamics-validation-rules}

検証ルールが尊重され、競合が発生した場合、結果がリードのアクティビティログに記録されます。
