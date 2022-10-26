---
description: Dynamic Chat の統合 — Marketoドキュメント — 製品ドキュメント
title: Dynamic Chat の統合
exl-id: b2e3b4da-9ca7-4299-9c50-f52e0de91e36
source-git-commit: 9d5c941dc4869b03787a6135550a133ce12b365b
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 6%

---

# Dynamic Chat の統合 {#dynamic-chat-integration}

Sales Insight とのダイナミックチャットの統合について詳しくご覧ください。

>[!PREREQUISITES]
>
>* Sales Insight SFDC パッケージはバージョンである必要があります [1.9 以降](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target=&quot;_blank&quot;}
>
>* 次を持っている必要があります： [Dynamic Chat の統合](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md){target=&quot;_blank&quot;} の設定


## Marketo Sales Insight の「設定」タブ {#marketo-sales-insight-configuration-tab}

Dynamic Chat の統合を有効にするには、以下の手順に従います。

1. Salesforce アカウントにログインし、タブバーの末尾にある「+」をクリックして、「 **Marketo Sales Insight 設定**.

1. 「Visualforce パネル」をクリックして展開します。

   ![](assets/dynamic-chat-integration-1.png)

1. を選択します。 **ダイナミックチャットデータの有効化** チェックボックス。

   ![](assets/dynamic-chat-integration-2.png)

## 機能の概要 {#feature-overview}

次のダイナミックチャットアクティビティは、Sales Insight ユーザーが利用できます…

アクションを実行したダイアログ：訪問者がチャットボットをクリックしてダイアログに移動したときに、Marketoにログインし、Sales Insight に入力します。

* ダイアログ名
* ページ URL
* ステータス（開始済み/ドロップ済み/完了済み）

予定予定：訪問者がチャットボットを使用して予定を正常にスケジュールしたら、Marketoにログインし、Sales Insight に入力します。

* ダイアログ名
* エージェント
* ページ URL
* スケジュール日（日付とタイムスタンプを挿入）
* ステータス（スケジュール済み、再スケジュール済み、キャンセル済み）

達成目標：Marketoにログインし、任意のダイアログフローで訪問者が目標に達したときに Sales Insight に入力します。

* ダイアログ名
* 目標名
* ページ URL

ドキュメントの操作：訪問者が Chatbot 経由で共有されたドキュメントを操作すると、Marketoにログインし、Sales Insight に入力されます。

* ダイアログ名
* ドキュメント
* Status

チャットアクティビティはインサイトダッシュボードで利用できます。

![](assets/dynamic-chat-integration-3.png)

[ チャット ] タブは、リードと連絡先パネルで使用できます。 アクティビティタイプ、ダイアログ名、日付の各列が含まれます。

![](assets/dynamic-chat-integration-4.png)

アクティビティのタイプをクリックすると、そのタイプに関する詳細を確認できます。

![](assets/dynamic-chat-integration-5.png)

同様に、アカウントパネルと商談パネルには、名前、アクティビティタイプ、ダイアログ名、日付列が含まれます。

![](assets/dynamic-chat-integration-6.png)

「チャット」タブは、「グローバルMarketo」タブにも表示されます。 これには、次の列と共に、3 つのアクティビティタイプ（アクションを実行したダイアログ、予定、達成目標）が含まれます。

* 顧客
* アカウント
* アクティビティのタイプ（アクションを実行したダイアログ、予定アポイント、目標に到達）
* ダイアログ名
* 日時スタンプ

繰り返しになりますが、アクティビティタイプをクリックすると、そのアクティビティの詳細を確認できます。

![](assets/dynamic-chat-integration-7.png)

>[!NOTE]
>
>[ ダイナミックチャットデータを有効にする ] チェックボックスが無効になっている場合、次の機能は無効になります。
>
>* インサイトダッシュボードのチャットアクティビティとの行（スマートグリッドと週別リスト表示）
>* リード、連絡先、アカウント、商談の各パネルの「チャット」タブ
>* 「グローバルMarketo」タブの「チャット」タブ
>
>これらの機能の 1 つのみを無効にすることはできません。

