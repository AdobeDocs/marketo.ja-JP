---
description: 詳細検索の概要 - Marketo ドキュメント - 製品ドキュメント
title: 詳細検索の概要
exl-id: a7cf5078-1d24-4fc0-a82d-02f46f93893d
source-git-commit: 66baa3063b2f6798f04f1b81d6ea52a484975174
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 100%

---

# 詳細検索の概要 {#advanced-search-overview}

詳細検索を利用して、メールを閲覧したりクリックしたり、メールに返信した見込み客をターゲットすることで、最もエンゲージメントの高い見込み客のターゲットリストを作成できます。

## 詳細検索へのアクセス方法 {#how-to-access-advanced-search}

1. Web アプリケーションで、「**コマンドセンター**」をクリックします。

   ![](assets/advanced-search-overview-1.png)

1. 「**メール**」をクリックします。

   ![](assets/advanced-search-overview-2.png)

1. 該当するタブを選択します。

   ![](assets/advanced-search-overview-3.png)

1. 「詳細検索」をクリックします。

   ![](assets/advanced-search-overview-4.png)

## フィルター {#filters}

**日付**

検索の日付範囲を選択します。プリセット日付は、選択したメールステータス（送信済み、未配信、保留中）に応じて更新されます。

![](assets/advanced-search-overview-5.png)

**対象者**

「対象者」セクションのメールの受信者／送信者でフィルタリングします。

![](assets/advanced-search-overview-6.png)

<table>
 <tr>
  <td><strong>ドロップダウン</strong></td>
  <td><strong>説明</strong></td>
 </tr>
 <tr>
  <td><strong>次のユーザとして表示</strong></td>
  <td>Sales Connect インスタンスの特定の送信者でフィルターします（このオプションは、管理者のみが利用できます）。</td>
 </tr>
 <tr>
  <td><strong>グループ別</strong></td>
  <td>特定の受信者グループでメールをフィルタリングします。</td>
 </tr>
 <tr>
  <td><strong>人物別</strong></td>
  <td>特定の受信者でフィルターします。</td>
 </tr>
</table>

**タイミング**

作成日、配信日、失敗した日付、スケジュールした日付別に選択します。使用可能なオプションは、選択したメールのステータス（送信済み、配信不能、保留中）に応じて異なります。

![](assets/advanced-search-overview-7.png)

**キャンペーン**

キャンペーン参加でメールをフィルタリングします。

![](assets/advanced-search-overview-8.png)

**ステータス**

選択できるメールステータスは 3 つあります。選択したステータスに応じて、タイプ／アクティビティのオプションが変わります。

![](assets/advanced-search-overview-9.png)

_**ステータス：送信済み**_

![](assets/advanced-search-overview-10.png)

送信したメールアクティビティ別にフィルタリングします。表示／表示なし、クリック／クリックなし、返信／返信なしを選択できます。

_**ステータス：保留中**_

![](assets/advanced-search-overview-11.png)

保留中のすべてのメールでフィルタリングします。

<table>
 <tr>
  <td><strong>ステータス</strong></td>
  <td><strong>説明</strong></td>
 </tr>
 <tr>
  <td><strong>スケジュール済み</strong></td>
  <td>作成ウィンドウ（Salesforce または web アプリ）、メールプラグイン、またはキャンペーンからスケジュールされたメール。</td>
 </tr>
 <tr>
  <td><strong>ドラフト</strong></td>
  <td>現在のステートがドラフトのメールです。メールをドラフトとして保存するには、件名と受信者が必要です。</td>
 </tr>
 <tr>
  <td><strong>進行中</strong></td>
  <td>送信中のメール。メールがこの状態に保たれるのは数秒間ほどです。</td>
 </tr>
</table>

_**ステータス：未配信**_

![](assets/advanced-search-overview-12.png)

配信されなかったメールでフィルタリングします。

<table>
 <tr>
  <td><strong>ステータス</strong></td>
  <td><strong>説明</strong></td>
 </tr>
 <tr>
  <td><strong>失敗</strong></td>
  <td>Sales Connect からのメール送信に失敗した場合（一般的な理由は次のとおりです。配信停止／ブロック済み取引先責任者に送信されたメール、または動的フィールドへの入力で問題が発生した場合）。</td>
 </tr>
 <tr>
  <td><strong>バウンス</strong></td>
  <td>メールは、受信者のサーバーによって拒否された場合、バウンス済みとしてマークされます。Sales Connect サーバー経由で送信されたメールのみがここに表示されます。</td>
 </tr>
 <tr>
  <td><strong>スパム</strong></td>
  <td>受信者によってメールがスパム（迷惑メールの一般用語）としてマークされた場合。Sales Connect サーバー経由で送信されたメールのみがここに表示されます。</td>
 </tr>
</table>

## 保存した検索条件 {#saved-searches}

検索条件を保存する方法を次に示します。

1. すべてのフィルターを設定したら、「**フィルターに名前を付けて保存**」をクリックします。

   ![](assets/advanced-search-overview-13.png)

1. 検索に名前を付け、「**保存**」をクリックします。

   ![](assets/advanced-search-overview-14.png)

保存した検索条件は、左側のサイドバーに表示されます。

![](assets/advanced-search-overview-15.png)
