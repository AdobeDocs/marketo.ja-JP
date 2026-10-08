---
unique-page-id: 45417322
description: Microsoft DynamicsとMarketo間でのリードおよび連絡先の削除の仕組みを説明します。 必要に応じて、「Microsoftは削除済み」フラグと「ユーザーを削除」フローアクションを使用します。
title: リードや連絡先の削除
exl-id: d561b424-6a2b-4abe-b9bd-81eb23f1a25b
feature: Microsoft Dynamics
TQID: 'https://experienceleague.adobe.com/4BwBuLQFJ2pRehuS8EqW-UrEcg5sVeqcstu3azh0NvQ'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
subfeature_v2:
  - id: d5c7388a-594e-4d15-9b39-98d6ce479e8b
    internal-label: Microsoft Dynamics
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 77%
---
# リードや連絡先の削除 {#deleting-a-lead-or-contact}

[!DNL Microsoft Dynamics] でリード／取引先責任者を削除する際には、いくつかの注意点があります。

* Marketoは、[!DNL Dynamics]でリードが削除されたという理由だけで、ユーザーを自動的に削除しません。 代わりに、フィールドの「Microsoft 削除済み」フラグが true に設定されます。 必要に応じて、このフィールドをトリガーにして、Marketo でレコードを削除できます。

* 人物を削除フローステップ：これは Marketo の人物のみを削除します（人物を Dynamics でも削除するオプションは使用できません）。

* リードが Marketo で削除され（[!DNL Dynamics] では削除されない）、その後、[!DNL Dynamics] で更新されると、Marketo で新しい人物（同じメールアドレス、新しい人物 ID）が作成されます。

* リードが [!DNL Dynamics] で削除され（Marketo では削除されない）、その後、「人物を Microsoft に同期」フローアクションを実行すると、[!DNL Dynamics] で新しいリードが作成されます。
