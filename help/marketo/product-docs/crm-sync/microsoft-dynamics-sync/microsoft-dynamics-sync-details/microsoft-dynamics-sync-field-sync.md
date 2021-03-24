---
unique-page-id: 3571838
description: Microsoft Dynamics Sync - Field Sync - Marketto Docs — 製品ドキュメント
title: Microsoft Dynamics Sync — フィールド同期
translation-type: tm+mt
source-git-commit: ed9399396c82a3b2fb93c83ffdaa1dc7b0827306
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---


# Microsoft Dynamics同期：フィールドの同期{#microsoft-dynamics-sync-field-sync}

MarkettoとDynamicsの同期は非常に強力です。 詳しくは、

## 2つのシステム間でフィールドの詳細を同期させる方法{#how-are-field-details-kept-in-sync-between-the-two-systems}

同期は、リードと連絡先のエンティティに対しては双方向です。 Dynamicsのリードや連絡先、またはMarketoの担当者に変更を加えると、両方のシステムに更新が反映されます。

アカウント、ユーザー、オポチュニティ、チーム、カスタムエンティティの場合、同期は一方向です。Dynamics to Marketor。 Dynamicsでこれらのエンティティに変更を加えると、Marketorに更新が反映されます。

## 両方のシステムの同じフィールドに変更が同時に行われた場合はどうなりますか。 （データの衝突） {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

これはまれですが、Marketoは人（リード）に勝ち、Dynamicsは連絡先に勝ちます。 これは、マーケティング部門が人々に対して権限を持つと考えられるのに対し、連絡先の正式な記録システムは販売部門(CRM)にあるからです。 一方向同期エンティティの場合、Dynamicsは常に勝ちます。

## Marketoを使用してDynamicsでフィールドを作成できますか？{#can-i-create-a-field-in-dynamics-using-marketo}

いいえ。現在、この機能はサポートされていません。

## Dynamicsにフィールドを作成しました。 Marketoと同期できますか。{#i-created-a-field-in-dynamics-can-i-sync-it-to-marketo}

はい。同期ユーザーがDynamicsでフィールド[にアクセスできる限り、フィールド](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync)を同期できます。

## Marketoと同期するフィールドは何ですか。{#what-fields-will-sync-to-marketo}

[設定中に、同期するフィールドを選択](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync)できます。

## MarketorとDynamicsの同期後にカスタムフィールドを追加する必要がある場合はどうなりますか？{#what-if-i-need-to-add-a-custom-field-after-marketo-and-dynamics-are-synced}

いつでもフィールドを追加でき、DynamicsからMarketorにデータが更新されるように期待できます。 詳しくは、[新しいカスタムフィールド用のMicrosoft Dynamicsとのクイック同期を使用する](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md)を参照してください。

## 同期するフィールドが追加された後にDynamicsでフィールドを削除する場合はどうしますか？{#what-if-i-want-to-delete-a-field-in-dynamics-after-the-field-has-been-added-to-sync}

Marketorは、同期するフィールドへの参照を保存します。 Dynamicsでフィールドを削除する場合は、[同期が無効](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md)の状態で削除することをお勧めします。 次に、[同期するフィールドの選択](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md)を編集して保存し、Marketorのスキーマを更新します。