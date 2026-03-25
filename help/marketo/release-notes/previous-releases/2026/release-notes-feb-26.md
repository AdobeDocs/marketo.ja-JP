---
description: リリースノート - 2026年2月 – Marketo ドキュメント – 製品ドキュメント
title: リリースノート - 2026年2月
feature: Release Information
exl-id: 679d2fca-99ba-4321-ad0d-a297b7f193fc
source-git-commit: 70939d387dcfe6064e179e4e7e91b16c6baa7b8b
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 41%

---

# リリースノート：2026年2月 {#release-notes-feb-26}

以下では、2026年2月リリースに含まれるすべての機能について説明します。 利用可能な機能については、お使いの Marketo Engage のエディションをご確認ください。

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
   <td><strong>電子メール Designer - フォルダーのアクション </strong>：古い電子メールエディターと同じ。
   <ul>
   <li>E メール Designer アセットのフォルダー操作を共有およびアーカイブします。</li>
   <li>ワークスペース間でフォルダーを共有し、フォルダーを右クリックして新しいアセットを作成し、ドラッグ&amp;ドロップでアセットを移動します。</li>
   </ul>
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
   <td><strong> メールDesigner - API</strong>：メールDesignerにAPI呼び出しを使用できるようになりました。</td>
   <td>リリース</td>
   <td><a href="https://developer.adobe.com/marketo-apis/api/asset#">Marketo Asset API</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong> メール Designer - AI アシスタント Image Generation</strong>：これで、Fireflyに加えて、Nano Banana モデルを使用して、メール コンテンツのAI アシスタントで画像を生成できます。</td>
   <td>リリース</td>
   <td><a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/email-marketing/email-designer/ai-assistant#create-content-for-a-specific-section">メールの特定のセクションのコンテンツを作成</a></td>
  </tr>
  </tbody>
</table>
<br/>

## お知らせ {#announcements}

* **SEO機能の廃止**: 2026年3月31日火曜日、Marketo Engageは検索エンジン最適化機能（SEO）を廃止します。 SEOを積極的に活用していない場合、何もする必要はありません。 最近SEOを利用したことがある場合は、データを書き出すオプションもあります。 [詳細情報](https://experienceleaguecommunities.adobe.com/adobe-marketo-engage-27/seo-feature-deprecation-248617?profile.language=ja){target="_blank"}。

* **REST API結合リードの制限**:2026年3月31日（PT）以降、結合リード API呼び出しのleadIds パラメーターに25を超えるIDを含む呼び出しは、1080 エラーコードになり、呼び出しはスキップされます。 25以上のレコードを1つのレコードに統合する必要があるジョブは、それらの呼び出しを成功させるために複数のジョブに分割する必要があります。

* **Rest API「access_token」パラメーターの廃止**：Marketo REST API 呼び出しの認証に使用される `access_token` クエリパラメーターは非推奨（廃止予定）となり、2026年7月31日（PT）以降は使用できなくなります。すべての新規および既存の統合では、「Authorization」ヘッダーを使用して REST API 呼び出しを認証する必要があります。[詳しくは、こちらを参照してください](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。

* **SOAP API の廃止**：Marketo SOAP API のサポートは、2026年7月31日（PT）に終了する予定です。SOAP API 機能を使用するサービスは、[REST API](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/rest-api){target="_blank"} に移行する必要があります。
