---
unique-page-id: 3571833
description: Microsoft Dynamics 同期 - 連絡先の同期 - Marketo ドキュメント - 製品ドキュメント
title: Microsoft Dynamics 同期 - 連絡先の同期
exl-id: d4583ea0-2b52-415e-b28c-a8eafebeff64
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 57%

---

# [!DNL Microsoft Dynamics] Sync: Contact Sync {#microsoft-dynamics-sync-contact-sync}

Marketoがデータベース全体を [!DNL Dynamics] と同期することをご存知ですか？ 同期し、5分待ってから、毎日、再び同期します。Marketoでの [!DNL Dynamics] ーザーの連絡先の具体的な取り扱い方法に関する詳細を以下に示します。

## 2 つのシステム間での詳細の同期方法 {#how-are-details-kept-in-sync-between-the-two-systems}

連絡先の同期は、双方向です。[!DNL Dynamics] またはMarketo内のユーザーの連絡先に変更を加えると、その変更は両方のシステムに反映されます。

## 両方のシステムの同じフィールドに同時に変更が加えられた場合の動作（データの競合） {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

これはまれですが、Marketoは人に勝ち、[!DNL Dynamics] は連絡先に勝ちます。 これは、人物についてはマーケティング部門が権限を持ち、連絡先についてはセールス（CRM）部門が公式な記録システムを持っていると考えているからです。

## Marketo を使用した連絡先の作成 {#can-i-create-a-contact-using-marketo}

はい。[以下に手順を示します](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync/create-a-contact-in-microsoft-dynamics.md){target="_blank"}。

>[!NOTE]
>
>「ユーザーをMicrosoftに同期」フローアクションを使用する場合（トリガーキャンペーンでのみ）、リード/連絡先は [!DNL Dynamics] でリアルタイムに作成されます。

## 手動での人物または連絡先の同期の強制 {#can-i-manually-force-a-sync-of-a-person-or-a-contact}

いいえ、自動のバックグラウンド同期は、Marketoと [!DNL Dynamics] の間で更新を同期させる唯一の方法です。 [担当者を Microsoft に同期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md)は、リードの同期を強制するものではありません。

## Marketo に同期されるフィールド {#what-fields-will-sync-to-marketo}

設定の際に、[同期するフィールドを選択](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync)できます。ただし、Marketoで同期されるのは、[!DNL Dynamics] sync ユーザーがアクセスできるフィールドのみです。

## Marketoは [!DNL Dynamics] の検証ルールを尊重しますか？ {#will-marketo-respect-the-dynamics-validation-rules}

検証ルールが尊重され、競合が発生した場合、結果がリードのアクティビティログに記録されます。
