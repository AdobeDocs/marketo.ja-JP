---
unique-page-id: 45417322
description: リードや連絡先の削除 - Marketo ドキュメント - 製品ドキュメント
title: リードや連絡先の削除
exl-id: d561b424-6a2b-4abe-b9bd-81eb23f1a25b
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '157'
ht-degree: 100%

---

# リードや連絡先の削除 {#deleting-a-lead-or-contact}

Microsoft Dynamics でリード／連絡先を削除する際には、いくつかの注意点があります。

* Dynamics でリードが削除されたからといって、Marketo が自動的に人物を削除することはありません。代わりに、フィールドの「Microsoft 削除済み」フラグが true に設定されます。必要に応じて、このフィールドをトリガーにして、Marketo でレコードを削除できます。

* 「顧客の削除」フローアクション：これは、Marketo の人物のみを削除します（Dynamics でも削除するオプションは使用できません）。

* リードが Marketo で削除され（Dynamics では削除されない）、その後、Dynamics で更新されると、Marketo で新しい人物（同じメールアドレス、新しい人物 ID）が作成されます。

* リードが Dynamics で削除され（Marketo では削除されない）、その後、「担当者を Microsoft に同期」フローアクションを実行すると、Dynamics で新しいリードが作成されます。
