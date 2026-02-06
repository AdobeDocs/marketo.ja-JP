---
description: リリースノート - 2025年1月 - Marketo ドキュメント - 製品ドキュメント
title: リリースノート - 2025年1月
feature: Release Information
exl-id: fd816b9c-9e06-4292-87d6-9fa991c4681f
source-git-commit: 8e72b24e18ae108ec74e6d4fa6b04f10130439a4
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 95%

---

# リリースノート：2025年1月 {#release-notes-jan-25}

以下に、2025年1月リリースに含まれるすべての機能を示します。利用可能な機能については、お使いの Marketo Engage のエディションをご確認ください。

Adobe Dynamic Chat 専用のリリースノートについて詳しくは、[こちらを参照](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}してください。

>[!AVAILABILITY]
>
>星印（![星印](assets/yellow-star.png)）で示す機能は有償オプションです。詳しくは、Marketo Engage 担当営業にお問い合わせください。

## 標準リリースサイクルの機能 {#standard-release-cycle-features}

次の機能は標準リリースサイクルに該当し、リリースは **2025年1月17日（PT）**&#x200B;から開始し、その次の週から残りの機能が段階的にロールアウトされます。リリースの機能と日付は変更される場合があります。各機能のステータスについては、各機能の隣で確認してください。

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:65%">機能</th>
   <th style="width:10%">ステータス</th>
   <th style="width:25%">ドキュメント</th>
  </tr>
    <tr>
   <td><strong>新しいメールデザイナー</strong>：Marketo Engage の新しいネイティブメールデザイナーを使用して、最新の効率的なメールを作成します。事前に設計された標準のメールテンプレートの 1 つにアクセスするか、独自のテンプレートを簡単に作成します。動的コンテンツを使用し、Adobe Experience Manager Cloud Services から画像にアクセスします。コンテンツアクセラレーターの生成 AI 機能を使用して、革新的でパフォーマンスの高いメールを大規模に作成します。
   <p><img src="assets/note-icon.png" alt="メモアイコン"> メモ：新しいメールデザイナーにアクセスするには、Marketo Engage サブスクリプションを <a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview">Adobe Identity Management システム（IMS）</a>に移行する必要があります。まだ移行しておらず、迅速な対応をリクエストする場合は、アドビのアカウントチーム（担当のアカウントマネージャー）または <a href="https://nation.marketo.com/t5/support/ct-p/Support">Marketo サポート</a>にお問い合わせください。コンテンツアクセラレーターの生成 AI 機能に対するアクセス権を取得するには、アドビのアカウントチームにお問い合わせください。</td>
   <td>リリース日</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/overview.md">メールデザイナー - 概要</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>インタラクティブウェビナーのイベントから登録者を登録解除</strong>：何らかの理由でウェビナーの登録者が必要ない場合は、登録解除できるようになりました。ワークフローにより、登録者は Marketo イベントプログラムと Adobe Connect の両方から削除されます。</td>
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>アーカイブ時にキャンペーンを無効にする</strong>：アクティブなトリガーキャンペーンを無効にし、アーカイブ時にフォルダー内のキャンペーンの予定されているバッチ実行をキャンセルします。アクティブなキャンペーン（トリガーキャンペーンをアクティブ化とバッチキャンペーンをスケジュール）を含むフォルダーのアーカイブに追加の権限チェックがあるので、この機能はこのリリースではデフォルトで無効になり、Marketo Engage サブスクリプションで<b>管理</b>／<b>アイデアスペース</b>に移動して有効にすることができます。</td>
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
 </tbody>
</table>
<br/>

## お知らせ {#announcements}

* **ソーシャル機能の廃止**：2024年7月31日水曜日（PT）に、Marketo Engage では製品内の次のソーシャル機能の廃止を開始しました。

   * 投票
   * ソーシャルボタン
   * 紹介オファー
   * 動画の共有
   * 懸賞

この時点では、ユーザは Marketo Engage でこれらのソーシャル機能を作成、複製、埋め込むことができなくなりました。既存のソーシャルアセットは、2025年1月31日（PT）まで引き続き機能します。2025年2月1日（PT）をもって、ソーシャルアセットは機能しなくなります。ランディングページに埋め込まれたソーシャル機能を削除する必要があります。[詳細情報](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

* **プログラムメンバー API の更新**:[&#x200B; プログラムメンバーの取得 &#x200B;](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/lead-database/program-members#query){target="_blank"} API が強化され、プログラムメンバーの識別子を取得する機能がサポートされるようになりました。 これを行うには、API リクエストの fields パラメーターで指定されたフィールドのリストに ID を追加します。

* **Rest API「access_token」パラメーターの廃止**：Marketo REST API 呼び出しの認証に使用される `access_token` クエリパラメーターは非推奨（廃止予定）となり、2026年3月31日（PT）以降は使用できなくなります。すべての新規および既存の統合では、「Authorization」ヘッダーを使用して REST API 呼び出しを認証する必要があります。[詳しくは、こちらを参照してください](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。

* **SOAP API の廃止**：Marketo SOAP API のサポートは、2026年3月31日（PT）に終了する予定です。SOAP API 機能を使用するサービスは、[REST API](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/rest-api){target="_blank"} に移行する必要があります。
