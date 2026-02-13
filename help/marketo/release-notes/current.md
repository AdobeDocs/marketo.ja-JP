---
description: 最新のリリースノート - Marketo ドキュメント - 製品ドキュメント
title: 最新のリリースノート
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: ce6a748acfb25ebc90c31dbfb16cf0230ca20b73
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 58%

---

# リリースノート：2026年2月 {#release-notes-jan-26}

以下に、2026 年 2 月リリースに含まれるすべての機能を示します。 利用可能な機能については、お使いの Marketo Engage のエディションをご確認ください。

Adobe Dynamic Chat 専用のリリースノートについて詳しくは、[こちらを参照](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}してください。

## 標準リリースサイクルの機能 {#standard-release-cycle-features}

以下の機能は標準リリースサイクルに従い、**2026年2月20日**（PT）からリリースを開始し、その次の週から残りの機能が段階的にロールアウトされます。リリースの機能と日付は変更される場合があります。各機能のステータスについては、各機能の隣で確認してください。

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">機能</th>
   <th style="width:10%">ステータス</th>
   <th style="width:25%">ドキュメント</th>
  </tr>
  <tr>
   <td><strong> メールDesigner - フォルダーアクション </strong>：古いメールエディターと同等です。
   <ul>
   <li>メールDesignerアセットのフォルダーアクションの共有とアーカイブ。</li>
   <li>ワークスペース間でフォルダーを共有し、フォルダーを右クリックして新しいアセットを作成したり、ドラッグ&amp;ドロップでアセットを移動したりします。</li>
   </ul>
   </td>
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong> メールDesigner - ブランド品質チェッカー </strong>：一般的なコンテンツ品質を評価して、ブランドガイドラインに依存せずに、読みやすさ、コンテンツのまとまり、効果に関する潜在的な問題を特定します。</td>
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong> メールDesigner - AI アシスタントの画像生成 </strong>：現在は、Fireflyに加えて、ナノバナナモデルを使用してメールコンテンツ用の AI アシスタントで画像を生成できます。</td>
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong> メールDesigner - API</strong>：メールDesignerに API 呼び出しを使用できるようになりました。</td>
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong> 選択リスト管理 </strong>:Marketo インターフェイス内のフィールドで使用できる値を指定します。</td>
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
  </tbody>
</table>
<br/>

## お知らせ {#announcements}

* **Rest API「access_token」パラメーターの廃止**：Marketo REST API 呼び出しの認証に使用される `access_token` クエリパラメーターは非推奨（廃止予定）となり、2026年3月31日（PT）以降は使用できなくなります。すべての新規および既存の統合では、「Authorization」ヘッダーを使用して REST API 呼び出しを認証する必要があります。[詳しくは、こちらを参照してください](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。

* **SOAP API の廃止**：Marketo SOAP API のサポートは、2026年3月31日（PT）に終了する予定です。SOAP API 機能を使用するサービスは、[REST API](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/rest-api){target="_blank"} に移行する必要があります。
