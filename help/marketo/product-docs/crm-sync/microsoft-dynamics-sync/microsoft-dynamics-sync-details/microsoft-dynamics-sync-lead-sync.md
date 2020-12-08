---
unique-page-id: 3571848
description: Microsoft Dynamics Sync - Lead Sync - Marketto Docs — 製品ドキュメント
title: Microsoft Dynamics同期 — リード同期
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 0%

---


# Microsoft Dynamics同期：リードの同期 {#microsoft-dynamics-sync-lead-sync}

MarkettoとDynamicsの同期は非常に強力です。 以下に詳細を示します。

## 2つのシステム間で詳細を同期させる方法 {#how-are-details-kept-in-sync-between-the-two-systems}

同期は双方向です。 DynamicsのリードまたはMarketoの担当者を変更すると、両方のシステムに更新が反映されます。

>[!NOTE]
>
>削除は、常に両方の方向で自動的に同期するとは限りません。 「リードまたは担当者の [削除](http://docs.marketo.com/x/agO1Ag)」を参照してください。

## 両方のシステムの同じフィールドに変更が同時に行われた場合はどうなりますか。 （データの衝突） {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

これはまれですが、Marketoは人（リード）に勝ち、Dynamicsは連絡先に勝ちます。 これは、マーケティング部門が人々に対して権限を持つと考えられるのに対し、連絡先の正式な記録システムは販売部門(CRM)にあるからです。

## Marketorを使用してDynamicsでリードを作成できますか？ {#can-i-create-a-lead-in-dynamics-using-marketo}

はい。「個人をMicrosoft [に同期](../../../../product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md) 」フローアクションを使用します。 リードが存在しない場合は、Dynamicsにリードが作成されます。 リードが存在する場合、フローステップは何も実行しません。

>[!NOTE]
>
>「個人をMicrosoftに同期」フローアクション(トリガーキャンペーンのみ)を使用する場合、Dynamicsでリアルタイムにリード/連絡先が作成されます。

## 手動でMarketoからDynamicsのリードに人を同期させることはできますか。 {#can-i-manually-force-a-sync-of-a-person-from-marketo-to-a-lead-in-dynamics}

いいえ。バックグラウンドの自動同期は、MarketoとDynamicsの間で更新を同期する唯一の方法です。 「 [個人をMicrosoft](../../../../product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md) Flowに同期」アクションでは、リードの同期を強制しません。

## Marketoと同期するフィールドは何ですか。 {#what-fields-will-sync-to-marketo}

セットアップ時に同期するフィールドを [選択できます](https://docs.marketo.com/pages/viewpage.action?pageId=3571830#Step3of3:ConnectMicrosoftDynamicswithMarketo(Online)-SelectFieldstoSync) 。

## マーケティング担当者はDynamics検証ルールを順守しますか？ {#will-marketo-respect-the-dynamics-validation-rules}

はい。 データ形式が正しくない場合、または必須フィールド情報がない場合、同期は失敗します。 この場合、ユーザーのアクティビティログに結果が記録されます。

