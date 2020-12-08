---
unique-page-id: 45417322
description: リードまたは担当者の削除 — Marketto Docs — 製品ドキュメント
title: リードまたは担当者の削除
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---


# リードまたは担当者の削除 {#deleting-a-lead-or-contact}

Microsoft Dynamicsでリード/連絡先を削除する際に知っておくべきことがいくつかあります。

-Dynamicsでリードが削除されたので、Marketorはユーザーを自動的に削除しません。 代わりに、「Microsoft is Deleted」フラグがtrueに設定されます。 必要に応じて、このフィールドからトリガーして、マーケティング先のレコードを削除できます。

- 「人物の削除」フロー・アクション：これにより、Marketor内のユーザーが削除されるだけです（Dynamics内のユーザーも削除するオプションは使用できません）。

 — リードがMarketoで削除され（Dynamicsでは削除されません）、その後Dynamicsで更新されると、Marketoで新しい人（同じ電子メールアドレス、新しい人ID）が作成されます。

- Dynamicsでリードが削除され（Marketoではなく）、その後「個人をMicrosoftに同期」フローアクションを実行すると、Dynamicsで新しいリードが作成されます。
