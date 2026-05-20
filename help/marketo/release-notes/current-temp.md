---
description: 最新のリリースノート - Marketo ドキュメント - 製品ドキュメント
title: 最新のリリースノート
hide: true
feature: Release Information
exl-id: 0ca5e844-c30b-4c86-a23d-d8f2c1bdddf5
TQID: https://experienceleague.adobe.com/RZsCx9HAyJuDLO46WfshT30be-rMMDZjnygvU32NGfk
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
source-git-commit: a04ec3931933c8e6cc0a0ffc26b1b559cd7cc9ce
workflow-type: tm+mt
source-wordcount: 421
ht-degree: 28%

---

# リリースノート：2026年5月 {#release-notes-may-26}

以下では、2026年5月リリースに含まれるすべての機能について説明します。 利用可能な機能については、お使いの Marketo Engage のエディションをご確認ください。

Adobe Dynamic Chat 専用のリリースノートについて詳しくは、[こちらを参照](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}してください。

## 標準リリースサイクルの機能 {#standard-release-cycle-features}

以下の機能は標準リリースサイクルに該当し、2026年5月22日（PT）にリリースが開始され、残りの機能は今後数週間にわたって段階的にロールアウトされます。 **&#x200B;**&#x200B;リリースの機能と日付は変更される場合があります。 各機能のステータスについては、各機能の隣で確認してください。

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">機能</th>
   <th style="width:10%">ステータス</th>
   <th style="width:25%">ドキュメント</th>
  </tr>
  <tr>
   <td><strong> メール Designer - メールフラグメントの条件付きコンテンツ </strong>: <i>古いメールエディターと同等</i>。 フラグメントで条件付きコンテンツがサポートされるようになりました。</td>
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong> ピックリスト管理</strong>: Marketo Engageのフィールドで使用できる値を指定できるようになりました。
   </td>
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
  </tbody>
</table>
<br/>

## お知らせ {#announcements}

* **ソーシャル機能の非推奨フィールド**: 2025年、Marketo Engageは次のソーシャル機能を非推奨にしました。

   * 投票
   * ソーシャルボタン
   * 紹介オファー
   * 動画の共有
   * 懸賞

今年の初めに、取り残されていた関連フィールドがMarketoから削除されました。 その後すぐに、特定のソーシャル関連のリードフィールドを参照するAPI リクエストで「フィールドが見つかりません」エラーが返され、中断が発生しました。 影響を受けるフィールドが再度使用可能になった後にサービスが復元されたため、さらなる中断を防ぐために、Marketoはソーシャル機能の非推奨化からソーシャルフィールドを永続的に分離しました（そのため、Marketo アカウントで利用できるようになります）。 Marketoのソーシャル関連フィールドを参照するAPI クエリと統合を確認し、それらのフィールドが継続的なビジネスプロセスに引き続き必要かどうかを判断することをお勧めします。

* **Rest API &#39;access_token&#39; パラメーターの非推奨**: Marketo REST API呼び出しの認証に使用される`access_token` クエリパラメーターは非推奨（廃止予定）であり、2026年7月31日を過ぎると使用できなくなります。 すべての新規および既存の統合では、「Authorization」ヘッダーを使用して REST API 呼び出しを認証する必要があります。[詳しくは、こちらを参照してください](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。

* **SOAP APIの非推奨化**: Marketo SOAP APIのサポートは、2026年7月31日に終了します。 SOAP API 機能を使用するサービスは、[REST API](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/rest-api){target="_blank"} に移行する必要があります。

* **リードアクティビティを取得およびリード変更を取得するための静的リストサイズの制限**: 2026年9月30日（PT）以降、「`listId`」パラメーターを含むリードアクティビティを取得およびリード変更を取得」エンドポイントへの呼び出しは、ターゲット静的リストに10,000個以上のリードが含まれている場合、1003 エラーコードを返します。 詳しくは、[移行ガイド &#x200B;](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"}を参照してください。
