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
source-git-commit: e8663ada66948bc30ff7ad90b26f6ba75d670ae8
workflow-type: tm+mt
source-wordcount: 466
ht-degree: 23%

---

# リリースノート：2026年7月#12日時点 {#release-notes-july-26-one}

以下では、2026年7月の最初のリリースに含まれるすべての機能について説明します。 利用可能な機能については、お使いの Marketo Engage のエディションをご確認ください。

Adobe Dynamic Chat 専用のリリースノートについて詳しくは、[こちらを参照](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}してください。

## 標準リリースサイクルの機能 {#standard-release-cycle-features}

以下の機能は標準リリースサイクルに該当し、2026年7月10日（PT）にリリースが開始され、残りの機能は今後数週間にわたって段階的にロールアウトされます。 **&#x200B;**&#x200B;リリースの機能と日付は変更される場合があります。 各機能のステータスについては、各機能の隣で確認してください。

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">機能</th>
   <th style="width:10%">ステータス</th>
   <th style="width:25%">ドキュメント</th>
  </tr>
  <tr>
   <td><strong>Marketo AI スキル – 製品知識</strong>：製品知識を使用すると、プラットフォームから離れることなく、Marketoの専門知識にオンデマンドでアクセスできます。平易な言葉で質問すると、MarketoのAIは、Adobeの公式ドキュメントにもとづいて回答します。
</td>
   <td>オープンベータ</td>
   <td><a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/marketo-ai/skills/product-knowledge" target="_blank">Marketo AIの概要</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Marketo AI スキル – リードを調査</strong>：特定の人物/リードがマイルストーン（MQL、プログラムの選定、キャンペーンなど）に到達しなかった理由を確認し、何が起こったのかを簡単な言葉で説明します。
</td>
   <td>オープンベータ</td>
   <td><a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/marketo-ai/skills/investigate-leads" target="_blank">Marketo AIの概要</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>電子メール Designer - AI アシスタントのコンテキストメニュー</strong>：電子メール DesignerのAI アシスタント機能に、コンテキストメニュー（黒いバー）からアクセスできるようになりました。 たとえば、テキストコンテンツを選択すると、コンテキストメニューにAI アシスタントアイコンが表示され、そこからクイックアクションを実行できます。</td>
   <td><i>近日リリース予定</i></td>
   <td><i>近日リリース予定</i></td>
  </tr>
  </tr>
  </tbody>
</table>
<br/>

## お知らせ {#announcements}

* **Rest API &#39;access_token&#39; パラメーターの非推奨**: Marketo REST API呼び出しの認証に使用される`access_token` クエリパラメーターは非推奨（廃止予定）であり、2026年8月31日を過ぎると使用できなくなります。 すべての新規および既存の統合では、「Authorization」ヘッダーを使用して REST API 呼び出しを認証する必要があります。[詳しくは、こちらを参照してください](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。

* **REST API結合リードの制限**: 2026年7月31日（PT）以降、結合リード API呼び出しのleadIds パラメーターに25を超えるIDを含む呼び出しは、1080 エラーコードになり、呼び出しはスキップされます。 25以上のレコードを1つのレコードに統合する必要があるジョブは、それらの呼び出しを成功させるために複数のジョブに分割する必要があります。

* **SOAP APIの非推奨化**: Marketo SOAP APIのサポートは、2026年7月31日に終了します。 SOAP API 機能を使用するサービスは、[REST API](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/rest-api){target="_blank"} に移行する必要があります。

* **リードアクティビティを取得およびリード変更を取得するための静的リストサイズの制限**: 2026年9月30日（PT）以降、「`listId`」パラメーターを含むリードアクティビティを取得およびリード変更を取得」エンドポイントへの呼び出しは、ターゲット静的リストに10,000個以上のリードが含まれている場合、1003 エラーコードを返します。 詳しくは、[移行ガイド &#x200B;](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"}を参照してください。
