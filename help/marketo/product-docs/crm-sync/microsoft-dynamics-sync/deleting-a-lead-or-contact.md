---
unique-page-id: 45417322
description: リードまたは担当者の削除 —Marketoドキュメント — 製品ドキュメント
title: リードまたは担当者の削除
exl-id: d561b424-6a2b-4abe-b9bd-81eb23f1a25b
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---

# リードまたは連絡先の削除{#deleting-a-lead-or-contact}

Microsoft Dynamicsでリード/連絡先を削除する際に知っておくべきことがいくつかあります。

* Marketoは、Dynamicsでリードが削除されたので、自動的に人を削除しません。 代わりに、「Microsoft is Deleted」フラグがtrueに設定されます。 必要に応じて、このフィールドをトリガーして、Marketoのレコードを削除できます。

* 「人物の削除」フローアクション：これにより、Marketo内のユーザーのみが削除されます（Dynamics内のユーザーも削除するオプションは使用できません）。

* リードがMarketoで削除され（Dynamicsでは削除されません）、その後Dynamicsで更新された場合、Marketoに新しい人（同じ電子メールアドレス、新しい人ID）が作成されます。

* Dynamicsでリードが削除され(Marketoでは削除されません)、その後「個人をMicrosoftに同期」フローアクションを実行すると、Dynamicsで新しいリードが作成されます。
