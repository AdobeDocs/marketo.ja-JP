---
unique-page-id: 3571848
description: Microsoft Dynamics Sync — リード同期 —Marketoドキュメント — 製品ドキュメント
title: Microsoft Dynamics同期 — リード同期
exl-id: ea04a039-32f7-41f9-85fb-18df8e236390
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# Microsoft Dynamics同期：リード同期{#microsoft-dynamics-sync-lead-sync}

Marketoとダイナミクスの同期は非常に強力です。 以下に詳細を示します。

## 2つのシステム間で詳細を同期させる方法{#how-are-details-kept-in-sync-between-the-two-systems}

同期は双方向です。 DynamicsのリードまたはMarketoの担当者を変更すると、両方のシステムに更新が反映されます。

>[!NOTE]
>
>削除は、常に両方の方向で自動的に同期するとは限りません。 「[リードまたは連絡先の削除](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/deleting-a-lead-or-contact.md)」を参照してください。

## 両方のシステムの同じフィールドに変更が同時に行われた場合はどうなりますか。 （データの衝突） {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

これはまれですが、Marketoは人（リード）に勝ち、ダイナミクスは接触に勝ちます。 これは、マーケティング部門が人々に対して権限を持つと考えられるのに対し、連絡先の正式な記録システムは販売部門(CRM)にあるからです。

## Marketoを使用してDynamicsでリードを作成できますか？{#can-i-create-a-lead-in-dynamics-using-marketo}

はい、[個人をMicrosoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md)フローアクションに同期します。 リードが存在しない場合は、Dynamicsにリードが作成されます。 リードが存在する場合、フローステップは何も実行しません。

>[!NOTE]
>
>「個人をMicrosoftに同期」フローアクション(トリガーキャンペーンのみ)を使用する場合、リード/連絡先はDynamicsでリアルタイムに作成されます。

## 手動でMarketoからDynamicsのリードへの人の同期を強制できますか？{#can-i-manually-force-a-sync-of-a-person-from-marketo-to-a-lead-in-dynamics}

いいえ。バックグラウンドの自動同期は、Marketoとダイナミクスの間で更新を同期する唯一の方法です。 [個人をMicrosoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md)に同期フローアクションは、リードの同期を強制しません。

## どのフィールドがMarketoと同期しますか。{#what-fields-will-sync-to-marketo}

[設定中に、同期するフィールドを選択](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync)できます。

## Marketoはダイナミクスの検証規則を順守しますか？{#will-marketo-respect-the-dynamics-validation-rules}

はい. データ形式が正しくない場合、または必須フィールド情報がない場合、同期は失敗します。 この場合、Marketoはユーザーのアクティビティログに結果を記録します。
