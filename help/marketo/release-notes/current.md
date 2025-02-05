---
description: 最新のリリースノート - Marketo ドキュメント - 製品ドキュメント
title: 最新のリリースノート
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 6f2c91d31b1d2ea3f2977aa3c9b1ca40e5459a16
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 23%

---

# リリースノート：2025年1月 {#release-notes-jan-25}

以下に、2025 年 1 月リリースに含まれるすべての機能を示します。 利用可能な機能については、お使いの Marketo Engage のエディションをご確認ください。

Adobe Dynamic Chat 専用のリリースノートについて詳しくは、[こちらを参照](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}してください。

>[!AVAILABILITY]
>
>星（![星](assets/yellow-star.png)）で示す機能は有償オプションです。詳しくは、Marketo Engage 担当営業にお問い合わせください。

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
   <td><strong> 新しいメールDesigner</strong>:Marketo Engageの新しいネイティブなメールDesignerを使用して、最新の効率的なメールを作成します。 事前に設計された既製のメールテンプレートの 1 つにアクセスするか、独自のテンプレートを簡単に作成できます。 動的コンテンツを使用し、Adobe Experience Manager Cloud Services から画像にアクセスします。 コンテンツアクセラレーターの Gen-AI 機能を使用すると、革新的でパフォーマンスの高いメールを大規模に作成できます。
   <p><img src="assets/note-icon.png" alt="メモアイコン"> 注意：新しい電子メール デザイナーにアクセスするには、Marketo Engageのサブスクリプションを <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview">Adobe Identity Management System （IMS） </a> に移行する必要があります。 まだの場合は、迅速な対応をリクエストする際は、Adobeアカウントチーム （アカウントマネージャー）または <a href="https://nation.marketo.com/t5/support/ct-p/Support">Marketo サポート </a> にお問い合わせください。 コンテンツアクセラレーターの Gen-AI 機能を利用するには、Adobeアカウントチームにお問い合わせください。</td>
   <td>出荷済み</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/overview.md">E メールDesignerの概要</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong> インタラクティブウェビナーのイベントから登録者を登録解除 </strong>：何らかの理由でウェビナーの登録者が必要ない場合は、登録解除できるようになりました。 ワークフローでは、登録者がMarketo イベントプログラムとAdobe Connectの両方から削除されます。</td> 
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong> アーカイブ時にキャンペーンを無効にする </strong>：アクティブなトリガーキャンペーンを無効にし、アーカイブ時にフォルダー内のキャンペーンのスケジュールされたバッチ実行をキャンセルします。 アクティブなキャンペーンを含むアーカイブフォルダーに対しては追加の権限チェック（「トリガーキャンペーンのアクティブ化」および「バッチキャンペーンのスケジュール」）が行われるので、この機能はこのリリースでデフォルトで無効になり、Marketo Engageサブスクリプションで <b> 管理者 </b>/<b> 宝箱 </b> に移動すると有効になります。</td> 
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## お知らせ {#announcements}

* **ソーシャル機能の廃止**:2024 年 7 月 31 日水曜日（PT）に、Marketo Engage内の次のソーシャル機能の廃止が開始されました。

   * 投票
   * ソーシャルボタン
   * 紹介オファー
   * 動画の共有
   * 懸賞

その時点では、ユーザーはMarketo Engageでこれらのソーシャル機能を作成、クローン、埋め込むことができません。 既存のソーシャルアセットは、2025 年 1 月 31 日（PT）まで引き続き機能します。 2025 年 2 月 1 日（PT）をもって、ソーシャルアセットは機能しなくなります。 ランディングページに埋め込まれたソーシャル機能を削除する必要があります。 [詳細情報](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

* **プログラムメンバー API の更新**:[ プログラムメンバーの取得 ](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/program-members#query){target="_blank"} API が強化され、プログラムメンバーの識別子を取得する機能がサポートされるようになりました。 これを行うには、API リクエストの fields パラメーターで指定されたフィールドのリストに ID を追加します。

* **Rest API &#39;access_token&#39; パラメーターの廃止**:Marketo REST API 呼び出しの認証に使用される `access_token` クエリパラメーターは非推奨となり、2025 年 6 月 30 日（PT）以降は使用できなくなります。 すべての新規および既存の統合は、「Authorization」ヘッダーを使用して REST API 呼び出しを認証する必要があります [ 詳しくは、こちらを参照 ](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。

* **SOAP API の廃止**: Marketo SOAP API のサポートは 2025 年 10 月 31 日に終了します。 SOAP API 機能を使用するサービスは、[REST API](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/rest-api){target="_blank"} に移行する必要があります。
