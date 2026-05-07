---
unique-page-id: 45417322
description: Microsoft DynamicsとMarketo間でのリードおよび連絡先の削除の仕組みを説明します。 必要に応じて、「Microsoftは削除済み」フラグと「ユーザーを削除」フローアクションを使用します。
title: リードや連絡先の削除
exl-id: d561b424-6a2b-4abe-b9bd-81eb23f1a25b
feature: Microsoft Dynamics
source-git-commit: d20c398cd1f5ed2646f56995c35a57630c3f2e95
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 77%

---

# リードや連絡先の削除 {#deleting-a-lead-or-contact}

[!DNL Microsoft Dynamics] でリード／取引先責任者を削除する際には、いくつかの注意点があります。

* Marketoは、[!DNL Dynamics]でリードが削除されたという理由だけで、ユーザーを自動的に削除しません。 代わりに、フィールドの「Microsoft 削除済み」フラグが true に設定されます。 必要に応じて、このフィールドをトリガーにして、Marketo でレコードを削除できます。

* 「顧客の削除」フローアクション：これは、Marketo の人物のみを削除します（Dynamics でも削除するオプションは使用できません）。

* リードが Marketo で削除され（[!DNL Dynamics] では削除されない）、その後、[!DNL Dynamics] で更新されると、Marketo で新しい人物（同じメールアドレス、新しい人物 ID）が作成されます。

* リードが [!DNL Dynamics] で削除され（Marketo では削除されない）、その後、「人物を Microsoft に同期」フローアクションを実行すると、[!DNL Dynamics] で新しいリードが作成されます。
