---
unique-page-id: 14352404
description: 「管理設定」タブ — Marketto Docs — 製品ドキュメント
title: 「管理設定」タブ
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 0%

---


# 管理設定タブ{#admin-settings-tab}

「管理設定」タブでは、任意のアカウントの管理者がチームの設定（プランの制限に関する）を確認できるほか、チームの電子メールのSalesforceへの記録方法を一括管理できます。

[チーム&#x200B;**のすべてのSalesforce同期設定を上書きする]チェックボックスを選択すると、BCCによるログのみを許可するか、API経由のみでログを許可するかのオプションが表示されます。**

**API logging**&#x200B;を選択した場合、Opportunities、Leads、Contactsのすべての設定`will be set for the entire team after you click **Save Changes**.`

ここから、チーム全体でオポチュニティとタスク同期を一括して有効にすることもできます。

>[!NOTE]
>
>これらの設定を一括有効にすると、チームのSalesforce設定全体で多数のAPI呼び出しが使用されます。

1 - 「自分のチームの設定を構成」を有効にします。

2 — チーム全体の同期の設定を有効にする

3 — 電子メールアクティビティと最新のMSEアクティビティをSFDCに記録する方法を設定します。

4 - 「販売接続タスクを同期」の有効化はオプションです

(注意：MSEでは、SFDCが行わない間はタスクをスキップできます。SFDCがタスクをスキップした場合、その処理をSFDCがどのように処理するかを決める必要があります。
