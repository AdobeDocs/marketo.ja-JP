---
description: リリースノート - 2025年5月 - Marketo ドキュメント - 製品ドキュメント
title: リリースノート - 2025年5月
feature: Release Information
exl-id: 99cd1d54-0a80-40fa-9d0c-1cb437be90f0
source-git-commit: 4a575c96100921c69c09996c649db979ac22cd4d
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 100%

---

# リリースノート：2025年5月 {#release-notes-may-25}

2025年5月リリースに含まれるすべての機能を以下に示します。利用可能な機能については、お使いの Marketo Engage のエディションをご確認ください。

Adobe Dynamic Chat 専用のリリースノートについて詳しくは、[こちらを参照](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}してください。

>[!AVAILABILITY]
>
>星印（![星印](assets/yellow-star.png)）で示す機能は有償オプションです。詳しくは、Marketo Engage 担当営業にお問い合わせください。

## 標準リリースサイクルの機能 {#standard-release-cycle-features}

以下の機能は標準リリースサイクルに該当します。リリースは **2025年5月23日**（PT）から開始し、その次の週から残りの機能が段階的にロールアウトされます。リリースの機能と日付は変更される場合があります。各機能のステータスについては、各機能の隣で確認してください。

<table style="table-layout:auto"> 
 <tbody>
 <tr> 
   <th style="width:65%">機能</th> 
   <th style="width:10%">ステータス</th>
   <th style="width:25%">ドキュメント</th>
  </tr>
  <tr> 
   <td><strong>メールデザイナーアセットのロールベースのアクセス制御</strong>：ロールベースのアクセス制御（RBAC）システムへの新しい機能強化により、新しいメールデザイナーで活用されるアセットに対して、より詳細な権限と改善されたユーザー管理が提供されます。</td> 
   <td>リリース済み</td>
   <td><a href="https://nation.marketo.com/t5/latest-product-innovations/product-updates-granular-permissions-to-new-email-designer/ba-p/357057">新しい E メールデザイナーに対するきめ細かい権限（ブログ投稿）</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>メールデザイナーで作成したメールの複製</strong>：新しいメールデザイナーを使用して作成した既存のメールを複製できるようになりました。</td> 
   <td>リリース済み</td>
   <td>該当なし</td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>任意の属性のトリガートークン</strong>：スマートキャンペーンフィールドで任意のアクティビティ属性のデータを使用できるように、トリガートークンの一覧が拡張されています。</td> 
   <td>リリース済み</td>
   <td>該当なし</td>
  </tr>
 </tbody> 
</table>
<br/>

## お知らせ {#announcements}

* **Facebook オフラインコンバージョン統合の更新**：2025年5月29日（PT）に、Marketo Engage の [Facebook オフラインコンバージョン](https://experienceleague.adobe.com/jp/docs/marketo/using/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions){target="_blank"}統合が新しい Meta [Conversions API](https://developers.facebook.com/docs/marketing-api/conversions-api){target="_blank"} に移行されます。これは、Graph API のバージョン管理に従って Meta が [Offline Conversions API](https://developers.facebook.com/docs/marketing-api/offline-conversions/){target="_blank"} を廃止したためです。詳しくは、Meta の [Conversions API を使用したオフラインイベントの送信](https://developers.facebook.com/docs/marketing-api/conversions-api/offline-events/){target="_blank"}（オフライン用の CAPI）ガイドを参照してください。

* **新しい分析機能 - パブリックベータ版**：[高度な BI 分析](/help/marketo/product-docs/reporting/advanced-bi-analytics/overview.md){target="_blank"}（以前の収益エクスプローラーおよび高度な Report Builder）は、4 月中旬に現在のすべての収益サイクルエクスプローラーユーザへのロールアウトを開始します。この新しいツールには、Marketo Engage データに関する柔軟なレポートとビジュアライゼーションインターフェイスが用意されています。これにより、進行状況やパフォーマンスなどに関する詳細を表示できます。より豊富なインタラクティブ機能とビジュアライゼーション、より高速なパフォーマンス、よりシームレスで直感的なユーザエクスペリエンスを備えています。

この機能にアクセスするには、高度な BI 分析アドオンを購入する必要があります。詳しくは、アドビのアカウントチーム（担当のアカウントマネージャー）にお問い合わせください。

* **Rest API「access_token」パラメーターの廃止**：Marketo REST API 呼び出しの認証に使用される `access_token` クエリパラメーターは非推奨（廃止予定）となり、2025年10月31日（PT）以降は使用できなくなります。すべての新規および既存の統合では、「Authorization」ヘッダーを使用して REST API 呼び出しを認証する必要があります。[詳しくは、こちらを参照してください](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。

* **SOAP API の廃止**：Marketo SOAP API のサポートは、2025年10月31日（PT）に終了する予定です。SOAP API 機能を使用するサービスは、[REST API](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/rest-api){target="_blank"} に移行する必要があります。
