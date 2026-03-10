---
unique-page-id: 45417322
description: Microsoft DynamicsとMarketoの間におけるリードおよび連絡先の削除の仕組みについて説明します。 必要に応じて、「Microsoftの削除」フラグと「ユーザーの削除」フローアクションを使用します。
title: リードや連絡先の削除
exl-id: d561b424-6a2b-4abe-b9bd-81eb23f1a25b
feature: Microsoft Dynamics
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '166'
ht-degree: 84%

---

# リードや連絡先の削除 {#deleting-a-lead-or-contact}

[!DNL Microsoft Dynamics] でリード／取引先責任者を削除する際には、いくつかの注意点があります。

* [!DNL Dynamics] でリードが削除されたからといって、Marketo が自動的に人物を削除することはありません。代わりに、フィールドの「Microsoft 削除済み」フラグが true に設定されます。必要に応じて、このフィールドをトリガーにして、Marketo でレコードを削除できます。

* 「顧客の削除」フローアクション：これは、Marketo の人物のみを削除します（Dynamics でも削除するオプションは使用できません）。

* リードが Marketo で削除され（[!DNL Dynamics] では削除されない）、その後、[!DNL Dynamics] で更新されると、Marketo で新しい人物（同じメールアドレス、新しい人物 ID）が作成されます。

* リードが [!DNL Dynamics] で削除され（Marketo では削除されない）、その後、「人物を Microsoft に同期」フローアクションを実行すると、[!DNL Dynamics] で新しいリードが作成されます。
