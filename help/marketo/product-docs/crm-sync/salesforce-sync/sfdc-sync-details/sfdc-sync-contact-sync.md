---
unique-page-id: 2953457
description: SFDC同期 — 連絡先の同期 —Marketoドキュメント — 製品ドキュメント
title: SFDC同期 — 連絡先の同期
exl-id: 537bbc95-9233-4454-892e-81f962cf729d
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 0%

---

# SFDC同期：連絡先同期{#sfdc-sync-contact-sync}

Marketoがデータベース全体をSalesforceと同期したのを知っていましたか？ 同期して5分待ち、その後、毎日、再び同期します。 ここでは、MarketoがSalesforce連絡先を具体的に扱う方法について詳しく説明します。

## 同期方向{#sync-direction}

連絡先の同期は双方向です。 SalesforceまたはMarketoの連絡先を変更すると、両方のシステムに更新が反映されます。

## 両方のシステムで変更が同時に行われた場合はどうなりますか。{#what-if-changes-are-made-in-both-systems-at-the-same-time}

私たちは優しく、セールスフォースに勝たせています。 このようなデータの衝突が起きることはまれです。

## Marketoの連絡先に変えてもいい？{#can-i-convert-a-person-into-a-contact-in-marketo}

はい、**[人](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md)**&#x200B;をコンバートフローアクションを使用します。

>[!CAUTION]
>
>Marketoの人をコンバージョンすると、Salesforceで新しいアカウントとオポチュニティが作成されます。 重複アカウントが不要な場合は、Salesforceを使用して変換します。

## 手動で連絡先の同期を強制できますか？{#can-i-manually-force-a-sync-of-a-contact}

はい、**[人をSFDCに同期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)**&#x200B;フローアクションを使用すると、リアルタイムで同期されます。

## すべての標準フィールドはMarketoと同期しますか。{#does-every-single-standard-field-sync-to-marketo}

いいえ。すべての標準フィールドが役に立つとは限りません。 すべてのカスタムフィールドを同期の一部とすることができます。

>[!NOTE]
>
>Marketoは、Marketo同期ユーザがアクセスできるフィールドのみを同期します。

## MarketoはSalesforce検証ルールを順守しますか。{#will-marketo-respect-the-salesforce-validation-rules}

はい、競合がある場合は、リードアクティビティログに結果を記録します。
