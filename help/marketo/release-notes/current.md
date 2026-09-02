---
description: 最新のリリースノート - Marketo ドキュメント - 製品ドキュメント
title: 最新のリリースノート
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
TQID: https://experienceleague.adobe.com/QJFy7PeGXlvS3jcJGcZJROlc8c1UvphO-TOOwPUQeX8
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: f71e690b-4480-4b67-9ef5-88f42f9cdfdb
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2:
  - id: c942e9f6-ed06-481a-abdd-1195363d1452
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: b40977d6745fdf31a48c6e08a7b070cd164408c8
workflow-type: tm+mt
source-wordcount: 477
ht-degree: 19%

---

# リリースノート：2026年8月 {#release-notes-aug-26}

以下では、2026年8月リリースに含まれるすべての機能について説明します。 利用可能な機能については、お使いの Adobe Marketo Engage のエディションをご確認ください。

Adobe Dynamic Chat 専用のリリースノートについて詳しくは、[こちらを参照](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}してください。

## 標準リリースサイクルの機能 {#standard-release-cycle-features}

以下の機能は標準リリースサイクルに該当し、2026年8月14日（PT）にリリースが開始され、残りの機能は今後数週間にわたって段階的にロールアウトされます。 **&#x200B;**&#x200B;リリースされる機能と日付は変更される場合があります。 各機能のステータスは、その機能の横に表示されている情報を確認してください。

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">機能</th>
   <th style="width:10%">ステータス</th>
   <th style="width:25%">ドキュメント</th>
  </tr>
  <tr>
   <td><strong>Marketo Engageの新しいUI</strong>: Marketo Engageのインターフェイスがリフレッシュされ、メニュー、アイコン、レイアウトが更新され、よりクリーンで現代的なエクスペリエンスが得られます。 これはビジュアルアップデートのみで、既存の機能やワークフローには影響しません。
</td>
   <td>8月の月全体に段階的に展開</td>
   <td><i>該当なし</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong> アーカイブでキャンペーンを無効にする</strong>: フォルダーをアーカイブすると、そのフォルダーツリー内のすべてのキャンペーンが無効になり、スケジュール解除されるようになりました。これにより、アーカイブされたスマートキャンペーンが予期せず実行されるのを防ぎます。
</td>
   <td>リリース</td>
   <td>該当なし</td>
  </tr>
    <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong> メール Designer - Script Builder</strong>: Script Builderは、パーソナライゼーション スクリプトをより迅速に作成するためのAIを活用したアシスタントです。
</td>
   <td><i>近日リリース予定</i></td>
   <td><i>近日リリース予定</i></td>
  </tr>
  </tbody>
</table>
<br/>

## お知らせ {#announcements}

* **Marketo AIは現在、Coworker for Marketo Engageになっています**: Coworker for Marketo Engageは、時間のかかるマーケティング機能を自動化するために設計された担当者のスキルを提供します。 すべてのユーザーが利用できる新しい名前、同じ機能。 [詳細情報](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/coworker-for-marketo/overview){target="_blank"}

* **Rest API &#39;access_token&#39; パラメーターの非推奨**: Marketo REST API呼び出しの認証に使用される`access_token` クエリパラメーターは非推奨（廃止予定）であり、2026年8月31日を過ぎると使用できなくなります。 すべての新規および既存の統合では、「Authorization」ヘッダーを使用して REST API 呼び出しを認証する必要があります。[詳しくは、こちらを参照してください](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。

* **REST API Campaign Run ID**：特定の状況において、アクティビティのCampaign Run ID値が、2つの引用符のペアの間で、誤った形式で返されることがありました（例：`"campaignRunId": ""102938""`）。<br/>8月のリリース以降、この値は常に正しい数値形式（`"campaignRunId": 102938`）で返されます

* **リード活動を取得およびリード変更を取得するための静的リストサイズ制限**:2026年9月30日（PT）以降、ターゲットリストに10,000個以上のリードが含まれ、ターゲットスタティックリストにレコードが多すぎることを示すエラーコードが10,003個ある場合、`listId` パラメーターを含むリード活動を取得またはリード変更エンドポイントの取得呼呼呼呼失敗が発生発生します。 詳細については、[移行ガイド &#x200B;](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"}を参照してください。

* **REST API結合リードの制限**:2026年7月31日（PT）現在、結合リード API呼び出しのleadIds パラメーターに25を超えるIDを含む呼び出しは、1080 エラーコードになり、呼び出しはスキップされます。 25以上のレコードを1つのレコードに統合する必要があるジョブは、それらの呼び出しを成功させるために複数のジョブに分割する必要があります。
