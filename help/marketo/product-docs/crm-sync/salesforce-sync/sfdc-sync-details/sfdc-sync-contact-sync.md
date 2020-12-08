---
unique-page-id: 2953457
description: SFDC同期 — 連絡先の同期 — マーケティング担当者向けドキュメント — 製品ドキュメント
title: SFDC同期 — 連絡先の同期
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 0%

---


# SFDC同期：連絡先の同期 {#sfdc-sync-contact-sync}

>[!NOTE]
>
>**FYI**
>
>Marketoは現在、すべての購読で言語を標準化しているので、購読およびdocs.marketo.comの人物/人物にリード/リードを表示できます。 これらの用語は同じことを意味し、記事の説明には影響しません。 他にも変化がある。 [詳細情報](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

Marketoがデータベース全体をSalesforceと同期することをご存じですか。 同期して5分待ち、その後、毎日、再び同期します。 MarketoがSalesforce連絡先を特別に扱う方法について、以下に詳しく説明します。

## 同期の方向 {#sync-direction}

連絡先の同期は双方向です。 SalesforceまたはMarketoの連絡先に変更を加えると、両方のシステムに更新が反映されます。

## 両方のシステムで変更が同時に行われた場合はどうなりますか。 {#what-if-changes-are-made-in-both-systems-at-the-same-time}

私たちは優しく、セールスフォースに勝たせています。 このようなデータの衝突が起きることはまれです。

## 人をMarketoの連絡先に変換できますか。 {#can-i-convert-a-person-into-a-contact-in-marketo}

はい、「** [人](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md)*の変換」フローアクションを使用します。

>[!CAUTION]
>
>Marketor内の顧客をコンバージョンすると、Salesforce内で新しいアカウントとオポチュニティが作成されます。 重複アカウントが不要な場合は、Salesforceを使用して変換します。

## 手動で連絡先の同期を強制できますか？ {#can-i-manually-force-a-sync-of-a-contact}

はい。「** [Sync Person to SFDC](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) **flow」アクションを使用すると、リアルタイムで同期が行われます。

## すべての標準フィールドはMarketoと同期しますか。 {#does-every-single-standard-field-sync-to-marketo}

いいえ。すべての標準フィールドが役に立つとは限りません。 すべてのカスタムフィールドを同期の一部とすることができます。

>[!NOTE]
>
>マーケティング担当者は、Marketo Syncユーザーがアクセスできるフィールドのみを同期します。

## Salesforceの検証ルールは、マーケティング担当者に適用されますか。 {#will-marketo-respect-the-salesforce-validation-rules}

はい、競合がある場合は、リードアクティビティログに結果を記録します。
