---
unique-page-id: 2953455
description: SFDC同期 — リード同期 — マーケティング担当者向けドキュメント — 製品ドキュメント
title: SFDC同期 — リード同期
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---


# SFDC同期：リードの同期 {#sfdc-sync-lead-sync}

SalesforceデータベースからMarketoの同期を知っていましたか。 同期し、5分待ってから、再び同期します。 毎日、毎日。 ここでは、MarketoがSalesforceのリードを具体的にどのように扱うかについて詳しく説明します。

## 同期の方向 {#sync-direction}

リード（人物）と連絡先の同期は双方向です。 SalesforceまたはMarketoのレコードに変更を加えると、両方のシステムに更新が反映されます。

## 両方のシステムで変更が同時に行われた場合はどうなりますか。 {#what-if-changes-are-made-in-both-systems-at-the-same-time}

マーケットが勝つ。 このようなデータの衝突が起きることはまれです。

## Marketoを使用してSalesforceでリードを作成できますか。 {#can-i-create-a-lead-in-salesforce-using-marketo}

はい、「 [個人をSFDCに同期](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) 」フローアクションを使用します。 これにより、リードが存在しない場合は、Salesforceにリードが作成されます。

## Marketonの担当者を手動でSalesforceのリードに同期させることはできますか。 {#can-i-manually-force-a-sync-of-a-person-in-marketo-to-a-lead-in-salesforce}

はい。「 [個人をSFDCに同期](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) 」フローアクションを使用すると、リアルタイムで同期されます。

## すべての標準フィールドはMarketoと同期しますか。 {#does-every-single-standard-field-sync-to-marketo}

いいえ。すべての標準フィールドが役に立つとは限りません。 すべてのカスタムフィールドを同期の一部とすることができます。

>[!NOTE]
>
>マーケティング担当者は、Salesforce同期ユーザーがアクセス権を持つフィールドのみを同期します。

## Salesforceの検証ルールは、マーケティング担当者に適用されますか。 {#will-marketo-respect-the-salesforce-validation-rules}

はい。 データ形式が正しくない場合、または必須フィールド情報がない場合、同期は失敗します。 これが発生した場合、Marketorはリードアクティビティログに結果を記録します。
