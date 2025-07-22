---
unique-page-id: 45417322
description: リードや連絡先の削除 - Marketo ドキュメント - 製品ドキュメント
title: リードや連絡先の削除
exl-id: d561b424-6a2b-4abe-b9bd-81eb23f1a25b
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 36%

---

# リードや連絡先の削除 {#deleting-a-lead-or-contact}

[!DNL Microsoft Dynamics] でリード/連絡先を削除する際に知っておくべきことがいくつかあります。

* リードが [!DNL Dynamics] で削除されたからといって、Marketoによってユーザーが自動的に削除されるわけではありません。 代わりに、「Microsoftが削除されました」フィールドのフラグは true に設定されます。 必要に応じて、このフィールドをトリガーにして、Marketo でレコードを削除できます。

* 「顧客の削除」フローアクション：これは、Marketo の人物のみを削除します（Dynamics でも削除するオプションは使用できません）。

* リードがMarketoで削除され（[!DNL Dynamics] では更新されず）、その後 [!DNL Dynamics] で更新された場合、Marketoに新しいユーザー（同じメールアドレス、新しいユーザー ID）が作成されます。

* [!DNL Dynamics] でリードが削除され（Marketoでは削除されない）、その後「ユーザーをMicrosoftに同期」フローアクションを実行すると、[!DNL Dynamics] で新しいリードが作成されます。
