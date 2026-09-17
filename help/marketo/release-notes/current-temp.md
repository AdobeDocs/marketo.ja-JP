---
description: 最新のリリースノート - Marketo ドキュメント - 製品ドキュメント
title: 最新のリリースノート
hide: true
feature: Release Information
exl-id: 0ca5e844-c30b-4c86-a23d-d8f2c1bdddf5
TQID: https://experienceleague.adobe.com/RZsCx9HAyJuDLO46WfshT30be-rMMDZjnygvU32NGfk
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
    internal-label: Forms
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: f71e690b-4480-4b67-9ef5-88f42f9cdfdb
    internal-label: Resources
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
    internal-label: Templates
subfeature_v2:
  - id: c942e9f6-ed06-481a-abdd-1195363d1452
    internal-label: Dynamic Chat
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: ba06d7ce62da1ceb3f696527532975622e06fa70
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 18%
---
# リリースノート：2026年9月 {#release-notes-sep-26}

以下では、2026年9月リリースに含まれるすべての機能について説明します。 利用可能な機能については、お使いの Adobe Marketo Engage のエディションをご確認ください。

Adobe Dynamic Chat 専用のリリースノートについて詳しくは、[こちらを参照](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}してください。

## 標準リリースサイクルの機能 {#standard-release-cycle-features}

以下の機能は標準リリースサイクルに該当し、2026年9月25日（PT）にリリースが開始され、残りの機能は今後数週間にわたって段階的にロールアウトされます。 **&#x200B;**&#x200B;リリースされる機能と日付は変更される場合があります。 各機能のステータスは、その機能の横に表示されている情報を確認してください。

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">機能</th>
   <th style="width:10%">ステータス</th>
   <th style="width:25%">ドキュメント</th>
  </tr>
  <tr>
   <td><strong>Marketo Engageの新しいUI</strong>: Marketo Engageのインターフェイスがリフレッシュされ、メニュー、アイコン、レイアウトが更新され、よりクリーンで現代的なエクスペリエンスが得られます。 これはビジュアルアップデートのみです。既存の機能やワークフローには影響しません。 <i> クラシック UIを選択する機能は、2027年1月リリース </i>から利用できます。
</td>
   <td>一般提供（9月末）</td>
   <td><i>該当なし</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>読み込み時にパーティションを選択</strong>: ワークスペースとパーティションが有効になっている環境で個人レコードを読み込む際に、ローカルワークスペースのパーティションのリストからパーティションを選択できるようになりました。</td>
   <td><i>近日リリース予定</i></td>
   <td><i>近日リリース予定</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>CRM同期に関する即時アラート </strong>: CRM通知を購読したユーザーは、ネイティブ CRM同期の有効ステータスが変更されると、すぐに通知を受け取り、管理者はCRM同期ステータスをより詳細に把握できます。</td>
   <td><i>近日リリース予定</i></td>
   <td><i>近日リリース予定</i></td>
  </tr>
   <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong> セルフサービスのフローステップ – コールバックタイムアウトの増加</strong>: セルフサービスのフローステップのコールバックタイムアウト時間が1時間から4時間に延長されました。 ユーザー側での操作は必要ありません。</td>
   <td><i>近日リリース予定</i></td>
   <td><i>近日リリース予定</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong> メールDesigner - テーブル </strong>: コンテンツの種類「テーブル」をメールにドラッグ&amp;ドロップし、列と行の数を設定できるようになりました。</td>
   <td><i>近日リリース予定</i></td>
   <td><i>近日リリース予定</i></td>
  </tr>
  </tbody>
</table>
<br/>

## お知らせ {#announcements}

* カスタムアクティビティ属性の&#x200B;**API名の制限**: APIまたはUIを介して作成されたカスタムアクティビティ属性のAPI名に、英数字とアンダースコアのみを含めることができるようになりました。英数字で始める必要があります。

* **リードアクティビティを取得およびリード変更を取得するための静的リストサイズの制限**:2026年9月30日（PT）以降、ターゲットリストに10,000個以上のリードが含まれている場合、`listId` パラメーターを含むリード活動を取得またはリード変更を取得のエンドポイントへの呼び出しは、1003 エラーコード（ターゲット静的リストが多すぎることを示す）で示場合）で失敗します。 詳細については、[移行ガイド &#x200B;](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"}を参照してください。

* **REST API &#39;access_token&#39; パラメーターの非推奨化**: Marketo REST API呼び出しの認証に使用される`access_token` クエリパラメーターは、2026年8月31日（PT）をもって非推奨（廃止予定）になりました。 すべての新規および既存の統合では、「Authorization」ヘッダーを使用して REST API 呼び出しを認証する必要があります。[詳しくは、こちらを参照してください](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。

* **REST API Campaign Run ID**：特定の状況において、アクティビティのCampaign Run ID値が、2つの引用符のペア（例：`"campaignRunId": ""102938""`）の間で、誤った形式で返されることがありました。<br/>8月のリリース以降、この値は常に正しい数値形式（`"campaignRunId": 102938`）で返されます。

* **WebからのGrab Imagesの廃止**：最新のセキュリティとプライバシーのベストプラクティスに準拠するため、10月のリリースで[WebからのGrab Images](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/images-and-files/grab-the-images-from-a-web-page){target="_blank"}機能は廃止されます。
