---
description: リリースノート - 2026年7月 – Marketo ドキュメント – 製品ドキュメント
title: リリースノート - 2026年7月
feature: Release Information
source-git-commit: bd433a683cab2437f6c32a5f52454d8ac4d9293a
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 19%

---

# リリースノート：2026年7月 {#release-notes-july-26}

以下では、2026年7月リリースに含まれるすべての機能について説明します。 利用可能な機能については、お使いの Adobe Marketo Engage のエディションをご確認ください。

Adobe Dynamic Chat 専用のリリースノートについて詳しくは、[こちらを参照](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}してください。

## 標準リリースサイクルの機能 {#standard-release-cycle-features}

以下の機能は標準リリースサイクルに該当し、2026年7月10日（PT）にリリースが開始され、残りの機能は今後数週間にわたって段階的にロールアウトされます。 ****&#x200B;リリースされる機能と日付は変更される場合があります。 各機能のステータスは、その機能の横に表示されている情報を確認してください。

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">機能</th>
   <th style="width:10%">ステータス</th>
   <th style="width:25%">ドキュメント</th>
  </tr>
  <tr>
   <td><strong>Marketo AI スキル – 製品知識</strong>：製品知識を使用すると、プラットフォームから離れることなく、Marketoの専門知識にオンデマンドでアクセスできます。 平易な言葉で質問すると、MarketoのAIは、Adobeの公式ドキュメントにもとづいて回答を提供します。
</td>
   <td>リリース</td>
   <td><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-ai/skills/product-knowledge" target="_blank">製品知識</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Marketo AI スキル – リードを調査</strong>：特定の人物/リードがマイルストーン（MQL、プログラムの選定、キャンペーンなど）に到達しなかった理由を確認し、何が起こったのかを平易な言葉で説明します。
</td>
   <td>リリース</td>
   <td><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-ai/skills/investigate-leads" target="_blank">リードの調査</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong> メール Designer - モジュール </strong>：メールの組み立てを高速化するために設計された、すぐに使用できる完全に構造化されたコンテンツ ブロックにアクセスできるようになりました。</td>
   <td>リリース</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/email-modules.md" target="_blank">メールDesignerでのモジュールの使用</a></td>
  </tr>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>電子メールDesigner - コンテンツの生成コンテキストメニュー</strong>：電子メールDesignerの「コンテンツの生成」機能に、コンテキストメニュー（黒いバー）からアクセスできるようになりました。 例えば、テキストコンテンツを選択すると、コンテキストメニューに「コンテンツを生成」アイコンが表示され、そこからクイックアクションを実行できます。</td>
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
* **リードアクティビティを取得およびリード変更を取得するための静的リストサイズの制限**: 2026年9月30日（PT）以降、「`listId`」パラメーターを含むリードアクティビティを取得およびリード変更を取得」エンドポイントへの呼び出しは、ターゲット静的リストに10,000個以上のリードが含まれている場合、1003 エラーコードを返します。 詳しくは、[移行ガイド ](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"}を参照してください。
