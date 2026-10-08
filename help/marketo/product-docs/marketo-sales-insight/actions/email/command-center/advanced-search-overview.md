---
description: コマンドセンターで高度な検索を使用して、メールとタスクを検索する方法を説明します。 日付、送信者、ステータスなどの基準でフィルタリングできます。
title: 詳細検索の概要
exl-id: a7cf5078-1d24-4fc0-a82d-02f46f93893d
feature: Sales Insight Actions
TQID: 'https://experienceleague.adobe.com/J-LNmjNNqY98t8gHi9-nRTds113phlyIb66MWyvJagk'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: 412786a7-b8da-5b9d-8c3f-2539a3faad9f
    internal-label: Sales Insight Actions
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 94%
---
# 詳細検索の概要 {#advanced-search-overview}

詳細検索を利用して、メールを閲覧したりクリックしたり、メールに返信した見込み客をターゲットすることで、最もエンゲージメントの高い見込み客のターゲットリストを作成できます。

## 詳細検索へのアクセス方法 {#how-to-access-advanced-search}

1. Web アプリケーションで、「**[!UICONTROL コマンドセンター]**」をクリックします。

   ![](assets/advanced-search-overview-1.png)

1. 「**[!UICONTROL メール]**」をクリックします。

   ![](assets/advanced-search-overview-2.png)

1. 該当するタブを選択します。

   ![](assets/advanced-search-overview-3.png)

1. 「[!UICONTROL 詳細検索]」をクリックします。

   ![](assets/advanced-search-overview-4.png)

## フィルター {#filters}

**日付**

検索の日付範囲を選択します。 プリセット日は、選択したメールステータス（[!UICONTROL 送信済み]、[!UICONTROL 未配信]、[!UICONTROL 保留中]）に応じて更新されます。

![](assets/advanced-search-overview-5.png)

**対象者**

「[!UICONTROL 対象者]」セクションのメールの受信者／送信者でフィルタリングします。

![](assets/advanced-search-overview-6.png)

<table>
 <tr>
  <td><strong>ドロップダウン</strong></td>
  <td><strong>説明</strong></td>
 </tr>
 <tr>
  <td><strong>[!UICONTROL ビュー形式]</strong></td>
  <td>Sales Connect インスタンスの特定の送信者でフィルターします（このオプションは、管理者のみが利用できます）。</td>
 </tr>
 <tr>
  <td><strong>[!UICONTROL グループ別]</strong></td>
  <td>特定の受信者グループでメールをフィルターします。</td>
 </tr>
 <tr>
  <td><strong>[!UICONTROL 人物別]</strong></td>
  <td>特定の受信者でフィルターします。​</td>
 </tr>
</table>

**タイミング**

作成日、配信日、失敗した日付、スケジュールした日付別に選択します。 使用できるオプションは、選択したメールのステータス（[!UICONTROL 送信済み]、[!UICONTROL 配信不能]、[!UICONTROL 保留中]）に応じて異なります。

![](assets/advanced-search-overview-7.png)

**キャンペーン**

キャンペーンへの参加状況でメールをフィルターします。

![](assets/advanced-search-overview-8.png)

**ステータス**

選択できるメールステータスは 3 つあります。 選択したステータスに応じて、タイプ／アクティビティのオプションが変更されます。

![](assets/advanced-search-overview-9.png)

_&#x200B;**ステータス：送信済み**&#x200B;_

![](assets/advanced-search-overview-10.png)

送信したメールアクティビティ別にフィルターします。 [!UICONTROL 表示回数]／[!UICONTROL 表示なし]、[!UICONTROL クリック数]／[!UICONTROL クリックなし]、[!UICONTROL 返信数]／[!UICONTROL 返信なし]を選択できます。

_&#x200B;**ステータス：保留中**&#x200B;_

![](assets/advanced-search-overview-11.png)

保留中のすべてのメールでフィルターします。

<table>
 <tr>
  <td><strong>ステータス</strong></td>
  <td><strong>説明</strong></td>
 </tr>
 <tr>
  <td><strong>[!UICONTROL スケジュール済み]</strong></td>
  <td>作成ウィンドウ（Salesforce または web アプリ）、メールプラグイン、またはキャンペーンからスケジュールされたメール。</td>
 </tr>
 <tr>
  <td><strong>[!UICONTROL ドラフト]</strong></td>
  <td>現在ドラフト状態のメール。 メールをドラフトとして保存するには、件名と受信者が必要です。</td>
 </tr>
 <tr>
  <td><strong>[!UICONTROL 進行中]</strong></td>
  <td>送信中のメール。 メールがこの状態に保たれるのは数秒間ほどです。</td>
 </tr>
</table>

_&#x200B;**ステータス：未配信**&#x200B;_

![](assets/advanced-search-overview-12.png)

配信されなかったメールでフィルターします。

<table>
 <tr>
  <td><strong>ステータス</strong></td>
  <td><strong>説明</strong></td>
 </tr>
 <tr>
  <td><strong>[!UICONTROL 失敗]</strong></td>
  <td>セールスコネクトからのメール送信に失敗した場合（一般的な理由としては、購読解除済み／ブロック済みの取引先責任者にメールが送信された場合や、動的フィールドの入力に問題があった場合など）が該当します。</td>
 </tr>
 <tr>
  <td><strong>[!UICONTROL バウンス済み]</strong></td>
  <td>メールは、受信者のサーバーによって却下された場合、バウンス済みとしてマークされます。 Sales Connect サーバー経由で送信されたメールのみがここに表示されます。</td>
 </tr>
 <tr>
  <td><strong>[!UICONTROL スパム]</strong></td>
  <td>受信者によってメールがスパム（迷惑メールの一般用語）としてマークされた場合。 Sales Connect サーバー経由で送信されたメールのみがここに表示されます。</td>
 </tr>
</table>

## 保存した検索条件 {#saved-searches}

保存した検索条件を作成する方法を次に示します。

1. すべてのフィルターを設定したら、「**[!UICONTROL フィルターに名前を付けて保存]**」をクリックします。

   ![](assets/advanced-search-overview-13.png)

1. 検索に名前を付け、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/advanced-search-overview-14.png)

保存した検索条件は、左側のサイドバーに表示されます。

![](assets/advanced-search-overview-15.png)
