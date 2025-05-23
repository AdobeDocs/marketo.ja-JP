---
description: 最新のリリースノート - Marketo ドキュメント - 製品ドキュメント
title: 最新のリリースノート
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: fddc2f24d9a66146f567c762305ab2825c2f29ae
workflow-type: tm+mt
source-wordcount: '473'
ht-degree: 68%

---

# リリースノート：2025年5月 {#release-notes-may-25}

2025年5月リリースに含まれるすべての機能を以下に示します。利用可能な機能については、お使いの Marketo Engage のエディションをご確認ください。

Adobe Dynamic Chat 専用のリリースノートについて詳しくは、[こちらを参照](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}してください。

>[!AVAILABILITY]
>
>星（![星](assets/yellow-star.png)）で示す機能は有償オプションです。詳しくは、Marketo Engage 担当営業にお問い合わせください。

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
   <td><strong>メールデザイナーのテンプレートの互換性</strong>：従来のメールエディターのメールテンプレートは、新しい<a href="/help/marketo/product-docs/email-marketing/email-designer/overview.md">メールデザイナー</a>と互換性を持つようになりました。</td>
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong> 任意の属性のトリガートークン </strong>:Smart Campaign フィールドで任意のアクティビティ属性のデータを使用できるように、トリガートークンのリストが拡張されています。</td> 
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong> メールコンテンツ Personalization</strong>:Marketo Engageは、他のAEP アプリケーショントークンと同じキャメルケース構文に従うようになり、Adobe DX 製品全体で一貫したエクスペリエンスが提供されます。 すべての標準トークンと、メンバー、プログラム、マイトークンなどのMarketo Engage固有のトークンは、新しいメールDesignerで使用できます。</td> 
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>E メールDesigner Assetsのロールベースのアクセス制御 </strong>：ロールベースのアクセス制御（RBAC）システムに対する新しい機能強化により、新しい E メールDesignerを活用した、アセットの権限がより詳細に提供され、ユーザー管理が強化されます。</td> 
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>E メールDesignerで作成したメールのクローン </strong>：新しい E メールDesignerを使用して作成された既存のメールをクローンできるようになりました。</td> 
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>GenStudioの統合 </strong>: メール内からGenStudioを統合してパフォーマンスマーケティングを行い、マーケティング効率を向上させ、ブランドの一貫性を保ちます。</td> 
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## お知らせ {#announcements}

* **新しい分析機能 - パブリックベータ版**：[高度な BI 分析](/help/marketo/product-docs/reporting/advanced-bi-analytics/overview.md){target="_blank"}（以前の収益エクスプローラーおよび高度な Report Builder）は、4 月中旬に現在のすべての収益サイクルエクスプローラーユーザへのロールアウトを開始します。この新しいツールには、Marketo Engage データに関する柔軟なレポートとビジュアライゼーションインターフェイスが用意されています。これにより、進行状況やパフォーマンスなどに関する詳細を表示できます。より豊富なインタラクティブ機能とビジュアライゼーション、より高速なパフォーマンス、よりシームレスで直感的なユーザエクスペリエンスを備えています。

この機能にアクセスするには、高度な BI 分析アドオンを購入する必要があります。詳しくは、アドビのアカウントチーム（担当のアカウントマネージャー）にお問い合わせください。

* **Rest API「access_token」パラメーターの廃止**：Marketo REST API 呼び出しの認証に使用される `access_token` クエリパラメーターは非推奨（廃止予定）となり、2025年10月31日（PT）以降は使用できなくなります。すべての新規および既存の統合では、「Authorization」ヘッダーを使用して REST API 呼び出しを認証する必要があります。[詳しくは、こちらを参照してください](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。

* **SOAP API の廃止**：Marketo SOAP API のサポートは、2025年10月31日（PT）に終了する予定です。SOAP API 機能を使用するサービスは、[REST API](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/rest-api){target="_blank"} に移行する必要があります。
