---
unique-page-id: 45417322
description: リードまたは担当者の削除 — Marketto Docs — 製品ドキュメント
title: リードまたは担当者の削除
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---


# リードまたは連絡先の削除{#deleting-a-lead-or-contact}

Microsoft Dynamicsでリード/連絡先を削除する際に知っておくべきことがいくつかあります。

* Dynamicsでリードが削除されたので、Marketorはユーザーを自動的に削除しません。 代わりに、「Microsoft is Deleted」フラグがtrueに設定されます。 必要に応じて、このフィールドにトリガーを設定し、マーケティング担当者のレコードを削除できます。

* 「人物の削除」フローアクション：これにより、Marketor内のユーザーが削除されるだけです（Dynamics内のユーザーも削除するオプションは使用できません）。

* リードがMarketorで削除され（Dynamicsでは削除されません）、その後Dynamicsで更新された場合、Marketoで新しい人（同じ電子メールアドレス、新しい人ID）が作成されます。

* Dynamicsでリードが削除され（Marketoではなく）、その後「個人をMicrosoftに同期」フローアクションを実行すると、Dynamicsで新しいリードが作成されます。
