---
unique-page-id: 37356329
description: 詳細検索の概要 - Marketo ドキュメント - 製品ドキュメント
title: 詳細検索の概要
exl-id: bb6e2c9f-b44a-43ba-94ae-ae30e182bcc8
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 71%

---

# 詳細検索の概要 {#advanced-search-overview}

詳細検索を利用して、メールを閲覧したりクリックしたり、メールに返信した見込み客をターゲットすることで、最もエンゲージメントの高い見込み客のターゲットリストを作成できます。

## 詳細検索へのアクセス方法 {#how-to-access-advanced-search}

1. 「**[!UICONTROL コマンドセンター]**」をクリックします。

   ![](assets/one.png)

1. 「**[!UICONTROL メール]**」をクリックします。

   ![](assets/two.png)

1. 該当するタブを選択します。

   ![](assets/three.png)

1. 「**[!UICONTROL 詳細検索]**」をクリックします。

   ![](assets/four.png)

## フィルター {#filters}

**日付**

検索の日付範囲を選択します。プリセットされた日付は、選択したメールステータス（[!UICONTROL &#x200B; 送信済み &#x200B;]、[!UICONTROL &#x200B; 未配信 &#x200B;]、[!UICONTROL &#x200B; 保留中 &#x200B;]）に応じて更新されます。

![](assets/date.png)

**対象者**

「[!UICONTROL Who]」セクションでメールの受信者/送信者でフィルタリングします。

![](assets/who.png)

| ドロップダウン | 説明 |
|---|---|
| **[!UICONTROL 別のユーザーとして表示]** | [!DNL Sales Connect] インスタンス内の特定の送信者でフィルターします（このオプションは、管理者のみが使用できます）。 |
| **[!UICONTROL グループ別]** | 特定の受信者グループでメールをフィルタリングします。 |
| **[!UICONTROL ユーザー別]** | 特定の受信者でフィルタリングします。 |

**タイミング**

作成日、配信日、失敗した日付、スケジュールした日付別に選択します。選択するメールステータス（[!UICONTROL &#x200B; 送信済み &#x200B;]、[!UICONTROL &#x200B; 未配信 &#x200B;]、[!UICONTROL &#x200B; 保留中 &#x200B;]）によって、使用可能なオプションが変わります。

![](assets/when.png)

**キャンペーン**

キャンペーン参加でメールをフィルタリングします。

![](assets/campaigns.png)

**ステータス**

選択できるメールステータスは 3 つあります。選択したステータスに応じて、タイプ／アクティビティのオプションが変わります。

![](assets/status.png)

***ステータス：送信済み***

![](assets/status-sent.png)

送信したメールアクティビティ別にフィルタリングします。表示／表示なし、クリック／クリックなし、返信／返信なしを選択できます。

***ステータス：保留中***

![](assets/status-pending.png)

保留中のすべてのメールでフィルタリングします。

| ステータス | 説明 |
|---|---|
| **[!UICONTROL スケジュール済み]** | 作成ウィンドウ（[!DNL Salesforce] または web アプリ）、メールプラグインまたはキャンペーンからスケジュールされたメール。 |
| **[!UICONTROL 下書き]** | 現在ドラフト状態のメール。メールをドラフトとして保存するには、件名と受信者が必要です。 |
| **[!UICONTROL 進行中]** | 送信中のメール。メールがこの状態に保たれるのは数秒間ほどです。 |

***ステータス：未配信***

![](assets/status-undelivered.png)

配信されなかったメールでフィルタリングします。

| ステータス | 説明 |
|---|---|
| **[!UICONTROL 失敗]** | [!DNL Sales Connect] からのメール送信に失敗した場合（一般的な理由は、メールが購読解除またはブロックされた連絡先に送信された場合や、動的フィールドへの入力に問題があった場合など）。 |
| **[!UICONTROL バウンス]** | メールは、受信者のサーバーによって拒否された場合、バウンス済みとしてマークされます。[!DNL Sales Connect] サーバーを介して送信されたメールのみが表示されます。 |
| **[!UICONTROL スパム]** | 受信者によってメールがスパム（迷惑メールの一般用語）としてマークされた場合。[!DNL Sales Connect] サーバーを介して送信されたメールのみが表示されます。 |

## 保存済みの検索結果 {#saved-searches}

保存済みの検索を作成する方法を次に示します。

1. すべてのフィルターを設定したら、「**[!UICONTROL フィルターに名前を付けて保存]**」をクリックします。

   ![](assets/save-search-1.png)

1. 検索に名前を付け、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/save-search-2.png)

   保存した検索条件は、左側のサイドバーに表示されます。

   ![](assets/advanced-search-overview-15.png)
