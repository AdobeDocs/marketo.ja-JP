---
description: リリースノート - 2026年3月 – Marketo ドキュメント – 製品ドキュメント
title: リリースノート - 2026年2月
feature: Release Information
source-git-commit: 48aeac444cca4abfc4393eb53dc091b8e73a5b63
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 18%

---

# リリースノート：2026年3月 {#release-notes-mar-26}

以下では、2026年3月リリースに含まれるすべての機能について説明します。 利用可能な機能については、お使いの Marketo Engage のエディションをご確認ください。

Adobe Dynamic Chat 専用のリリースノートについて詳しくは、[こちらを参照](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}してください。

## 標準リリースサイクルの機能 {#standard-release-cycle-features}

以下の機能は標準リリースサイクルに該当し、2026年3月27日（PT）にリリースが開始され、残りの機能は今後数週間にわたって段階的にロールアウトされます。 ****&#x200B;リリースの機能と日付は変更される場合があります。 各機能のステータスについては、各機能の隣で確認してください。

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">機能</th>
   <th style="width:10%">ステータス</th>
   <th style="width:25%">ドキュメント</th>
  </tr>
  <tr>
   <td><strong>Email Designer - ブランドの管理（ベータ版） </strong>：組織/ブランド固有のコピーライティングガイドラインに基づいてメールコンテンツを生成します。</td>
   <td>リリース</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/brands/manage-brands.md" target="_blank">ブランドの構築と管理</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>電子メール Designer - フラグメント内の編集可能なHTML コンポーネント </strong>：ビジュアルフラグメント内では、コンポーネントプロパティパネルを通じて、画像、テキスト、ボタンのコンポーネントで編集可能なフィールドがサポートされています。 HTML コンポーネントの場合、編集可能フィールドは、HTML コンポーネント自体のソースコード内で変数ベースの構文を使用して、異なる方法で設定されます。
   </td>
   <td>リリース</i></td>
   <td><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/email-designer/customizable-fragments#editable-html" target="_blank">フラグメント内の編集可能なHTML コンポーネント</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>電子メール Designer - クイックアクション </strong>: <i>古い電子メールエディターと同じ</i>。 すべてのメール Designer アセット（メール、メールテンプレート、フラグメント）でクイックアクションが使用できるようになりました。 サポートされているクイックアクションには、複製、削除、移動、ドラフトの作成/編集などがあります。
   </td>
   <td>リリース</i></td>
   <td>該当なし</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
   <tr>
   <td><strong>電子メール Designer - Outlook レンダリングの修正</strong>：この更新プログラムは、特にMS Outlookでのレンダリングの問題を修正します。 高度なHTMLモードを使用すると、HTML/CSSのマイナーな編集や、メールテンプレートへのスクリプトタグの追加を行うことができます。
   </td>
   <td>リリース</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/advanced-html-mode.md" target="_blank">高度なHTMLエディターでメールテンプレートを編集できます</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Email Designer - Brand Score Checker</strong>：一般的なコンテンツの品質を評価して、ブランドガイドラインに依存せずに、読みやすさ、コンテンツの一貫性、有効性に関する潜在的な問題を特定します。</td>
   <td>リリース</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/brands/brand-score.md" target="_blank">ブランドスコア</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong> プッシュ通知</strong>: プッシュ通知メッセージで設定されたリダイレクト URIで、Marketo Engage トークンがサポートされるようになりました（<i>Launch アプリ URL</i>にのみ適用）。
   </td>
   <td>リリース</td>
   <td><a href="/help/marketo/product-docs/mobile-marketing/push-notifications/configure-mobile-push-notification.md#redirect-uris">リダイレクト URI</a></td>
  </tr>
  </tbody>
</table>
<br/>

## お知らせ {#announcements}

* **SEO機能の廃止**: 2026年3月31日火曜日、Marketo Engageは検索エンジン最適化機能（SEO）を廃止します。 SEOを積極的に活用していない場合、何もする必要はありません。 最近SEOを利用したことがある場合は、データを書き出すオプションもあります。 [詳細情報](https://experienceleaguecommunities.adobe.com/adobe-marketo-engage-27/seo-feature-deprecation-248617){target="_blank"}。

* **REST API結合リードの制限**:2026年3月31日（PT）以降、結合リード API呼び出しのleadIds パラメーターに25を超えるIDを含む呼び出しは、1080 エラーコードになり、呼び出しはスキップされます。 25以上のレコードを1つのレコードに統合する必要があるジョブは、それらの呼び出しを成功させるために複数のジョブに分割する必要があります。

* **Rest API &#39;access_token&#39; パラメーターの非推奨**: Marketo REST API呼び出しの認証に使用される`access_token` クエリパラメーターは非推奨（廃止予定）であり、2026年7月31日を過ぎると使用できなくなります。 すべての新規および既存の統合では、「Authorization」ヘッダーを使用して REST API 呼び出しを認証する必要があります。[詳しくは、こちらを参照してください](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。

* **SOAP APIの非推奨化**: Marketo SOAP APIのサポートは、2026年7月31日に終了します。 SOAP API 機能を使用するサービスは、[REST API](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/rest-api){target="_blank"} に移行する必要があります。
