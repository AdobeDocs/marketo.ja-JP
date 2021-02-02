---
unique-page-id: 3571833
description: Microsoft Dynamics Sync — 連絡先の同期 — Marketto Docs — 製品ドキュメント
title: Microsoft Dynamics Sync — 連絡先の同期
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 0%

---


# Microsoft Dynamics同期：連絡先同期{#microsoft-dynamics-sync-contact-sync}

Marketoがデータベース全体をDynamicsと同期することを知っていますか。 同期して5分待ち、その後、毎日、再び同期します。 MarketoがDynamicsの連絡先を特別に扱う方法について、次に詳しく説明します。

## 2つのシステム間で詳細を同期させる方法{#how-are-details-kept-in-sync-between-the-two-systems}

連絡先の同期は双方向です。 Dynamicsの連絡先またはMarketoの担当者に変更を加えると、両方のシステムに更新が反映されます。

## 両方のシステムの同じフィールドに変更が同時に行われた場合はどうなりますか。 （データの衝突） {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

これはまれですが、Marketoがユーザーに勝ち、Dynamicsが連絡先に勝ちます。 これは、マーケティング部門が人々に対して権限を持つと考えられるのに対し、連絡先の正式な記録システムは販売部門(CRM)にあるからです。

## Marketoを使用して連絡先を作成できますか。{#can-i-create-a-contact-using-marketo}

はい。 [方法は](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync/create-a-contact-in-microsoft-dynamics.md)。

>[!NOTE]
>
>「個人をMicrosoftに同期」フローアクション(トリガーキャンペーンのみ)を使用する場合、リード/連絡先はDynamicsでリアルタイムに作成されます。

## 手動で人または連絡先の同期を強制できますか。{#can-i-manually-force-a-sync-of-a-person-or-a-contact}

いいえ。バックグラウンドの自動同期は、MarketoとDynamicsの間で更新を同期する唯一の方法です。 [個人をMicrosoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md)に同期しても、リードの同期は強制されません。

## Marketoと同期するフィールドは何ですか。{#what-fields-will-sync-to-marketo}

[設定中に、同期するフィールドを選択](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync)できます。 ただし、Dynamics同期ユーザーがアクセス権を持つフィールドのみが同期されます。

## マーケティング担当者はDynamics検証ルールを順守しますか？{#will-marketo-respect-the-dynamics-validation-rules}

はい、競合がある場合は、リードアクティビティログに結果を記録します。
