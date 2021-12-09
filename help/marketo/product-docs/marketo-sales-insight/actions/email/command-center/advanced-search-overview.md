---
description: 詳細検索の概要 — Marketoドキュメント — 製品ドキュメント
title: 詳細検索の概要
hide: true
hidefromtoc: true
exl-id: a7cf5078-1d24-4fc0-a82d-02f46f93893d
source-git-commit: fda1bf51d4016a61c41be9acba4771db1797a552
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 5%

---

# 詳細検索の概要 {#advanced-search-overview}

詳細検索を利用して、E メールを閲覧、クリックまたは返信した見込み客をターゲットにすることで、最も関心の高い見込み客のターゲットリストを作成できます。

## 詳細検索へのアクセス方法 {#how-to-access-advanced-search}

1. Web アプリケーションで、 **コマンドセンター**.

   ![](assets/advanced-search-overview-1.png)

1. クリック **電子メール**.

   ![](assets/advanced-search-overview-2.png)

1. 該当するタブを選択します。

   ![](assets/advanced-search-overview-3.png)

1. 「詳細検索」をクリックします。

   ![](assets/advanced-search-overview-4.png)

## フィルター {#filters}

**日**

検索の日付範囲を選択します。 プリセット日は、選択した E メールステータス（送信済み、未配信、保留中）に応じて更新されます。

![](assets/advanced-search-overview-5.png)

**対象ユーザー**

「Who」セクションの E メールの受信者/送信者でフィルタリングします。

![](assets/advanced-search-overview-6.png)

<table>
 <tr>
  <td><strong>ドロップダウン</strong></td>
  <td><strong>説明</strong></td>
 </tr>
 <tr>
  <td><strong>表示形式</strong></td>
  <td>セールスコネクトインスタンスの特定の送信者でフィルターします（このオプションは、管理者のみが利用できます）。</td>
 </tr>
 <tr>
  <td><strong>グループ別</strong></td>
  <td>特定の受信者グループで E メールをフィルタリングします。</td>
 </tr>
 <tr>
  <td><strong>担当者別</strong></td>
  <td>特定の受信者でフィルターします。</td>
 </tr>
</table>

**タイミング**

作成日、配信日、失敗日、または予定日別に選択します。 使用可能なオプションは、選択した E メールのステータス（送信済み、配信不能、保留中）に応じて異なります。

![](assets/advanced-search-overview-7.png)

**キャンペーン**

キャンペーンパーティシペーションで E メールをフィルタリングします。

![](assets/advanced-search-overview-8.png)

**ステータス**

選択できる E メールステータスは 3 つあります。 選択したステータスに応じて、タイプ/アクティビティのオプションが変わります。

![](assets/advanced-search-overview-9.png)

_**ステータス：送信済み**_

![](assets/advanced-search-overview-10.png)

送信した電子メールアクティビティ別にフィルタリングします。 表示回数/表示回数、クリック数/クリック数、返信数/返信なしを選択できます。

_**ステータス：保留中**_

![](assets/advanced-search-overview-11.png)

保留中のすべてのメールでフィルターします。

<table>
 <tr>
  <td><strong>ステータス</strong></td>
  <td><strong>説明</strong></td>
 </tr>
 <tr>
  <td><strong>スケジュール済み</strong></td>
  <td>作成ウィンドウ（Salesforce または Web アプリ）、電子メールプラグイン、またはキャンペーンからスケジュールされた電子メール。</td>
 </tr>
 <tr>
  <td><strong>下書き</strong></td>
  <td>現在ドラフト状態のメール。 メールを下書きとして保存するには、件名と受信者が必要です。</td>
 </tr>
 <tr>
  <td><strong>進行中</strong></td>
  <td>送信中の電子メール。 E メールは、数秒間以上この状態に保たれないでください。</td>
 </tr>
</table>

_**ステータス：未配信**_

![](assets/advanced-search-overview-12.png)

配信されなかった E メールでフィルターします。

<table>
 <tr>
  <td><strong>ステータス</strong></td>
  <td><strong>説明</strong></td>
 </tr>
 <tr>
  <td><strong>失敗</strong></td>
  <td>セールスコネクトからのメール送信に失敗した場合（一般的な理由は次のとおりです）。配信停止/ブロック済み連絡先に送信されている電子メール、または動的フィールドへの入力で問題が発生した場合 )。</td>
 </tr>
 <tr>
  <td><strong>バウンス</strong></td>
  <td>E メールは、受信者のサーバーによって拒否された場合、バウンス済みとしてマークされます。 セールスコネクトサーバー経由で送信されたメールのみがここに表示されます。</td>
 </tr>
 <tr>
  <td><strong>スパム</strong></td>
  <td>受信者によって E メールがスパム（迷惑メールの一般用語）としてマークされた場合。 セールスコネクトサーバー経由で送信されたメールのみがここに表示されます。</td>
 </tr>
</table>

## 保存済みの検索結果 {#saved-searches}

保存済みの検索を作成する方法を次に示します。

1. すべてのフィルターを設定したら、「 **フィルターに名前を付けて保存**.

   ![](assets/advanced-search-overview-13.png)

1. 検索に名前を付け、「 **保存**.

   ![](assets/advanced-search-overview-14.png)

保存済みの検索結果は、左側のサイドバーに表示されます。

![](assets/advanced-search-overview-15.png)
