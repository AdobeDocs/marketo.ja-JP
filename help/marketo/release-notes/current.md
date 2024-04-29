---
description: 最新のリリースノート - Marketo ドキュメント - 製品ドキュメント
title: 最新のリリースノート
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 8473c4d59210bb18c3968a56883034febf00c320
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 78%

---

# リリースノート：2024年4月 {#release-notes-apr-24}

2024年4月リリースに含まれるすべての機能を以下に示します。機能の可用性についてはお使いの Marketo Engage のエディションをご確認ください。

Adobe Dynamic Chat専用のリリースノート [詳細はこちら](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>星（![星](assets/yellow-star.png)）で示す機能は有償オプションです。詳しくは、Marketo Engage 担当営業にお問い合わせください。

## 標準リリースサイクルの機能 {#standard-release-cycle-features}

以下の機能は標準リリースサイクルに該当し、リリースは **2024年4月26日**（PT）から開始し、その次の週から残りの機能が段階的にロールアウトされます。リリースの機能と日付は変更される場合があります。各機能のステータスについては、各機能の隣で確認してください。

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">機能</th> 
   <th style="width:10%">ステータス</th>
   <th style="width:25%">ドキュメント</th>
  </tr>
     <tr> 
   <td><strong>インタラクティブウェビナーの機能強化</strong>：ホストと発表者に対して、ウェビナータイトルの追加、部屋名の変更、イベント配信後にエンゲージメントデータを手動で同期する機能を提供できるようになりました。</td> 
   <td>出荷済み</td>
   <td><li><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/create-an-interactive-webinar.md">インタラクティブウェビナーの作成</a></li>
   <li><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/event-workflows.md#manual-sync">手動同期</a></li></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>監査記録の機能強化</strong>：
   新しいタイプのアクションを、フィールド管理で行われた変更、ユーザ＆ロールに行われた変更、リストとスマートリストから書き出されたユーザ数の監査記録で取り込めるようになりました。</td> 
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>新しいユーザ＆ロールの権限</strong>：新しい権限が利用可能になり、ユーザは Marketo Engage へのより詳細なアクセスが可能になります。新しいエクスペリエンスや Predictive Audiences など、以前はゲートされていなかった管理者の一部を制御し、権限を分割してアセット監査記録と管理者監査記録へのアクセス権を個別に付与し、アセットやフォルダーの新しい作成および移動権限を利用して読み取り専用ユーザーが変更を加えないようにします。 新しい権限は 4 月 26 日（PT）以降お使いのMarketo Engageインスタンスに表示されますが、現時点ではパッシブであり、今四半期後にアクセスできるようになります。</td> 
   <td>出荷済み</td>
   <td><a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md">ロールの権限の説明</a></td>
  </tr>
 </tbody> 
</table>
<br/>

## お知らせ {#announcements}

* **アクティビティ API の更新**：4月26日（PT）に、[Marketo REST API](https://developers.marketo.com/rest-api/lead-database/activities/){target="_blank"}. The activities listed below will now include Browser, Platform, Device, and User Agent attributes. Call the [Get Activity Types](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Activities/getAllActivityTypesUsingGET){target="_blank"} エンドポイントを使用してアクティビティを取得し、各アクティビティの属性の詳細を確認すると返される、web ベースおよびメールベースのアクティビティにいくつかの新しい属性を追加します。

**Web ベースのアクティビティ**

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:30%">アクティビティ</th> 
   <th style="width:70%">新しく追加された属性</th>
   </tr>
  <tr> 
   <td>Web ページに訪問</td> 
   <td>ブラウザー、プラットフォーム、デバイス</td>
  </tr>
   <tr> 
   <td>フォームの入力</td> 
   <td>ブラウザー、プラットフォーム、デバイス</td>
  </tr>
  <tr> 
   <td>リンクをクリック</td> 
   <td>ブラウザー、プラットフォーム、デバイス</td>
  </tr>
 </tbody> 
</table>

**メールベースのアクティビティ**

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:30%">アクティビティ</th> 
   <th style="width:70%">新しく追加された属性</th>
  </tr>
   <tr> 
   <td>メールの送信</td> 
   <td>ブラウザー、プラットフォーム、デバイス、ユーザエージェント</td>
  </tr>
   </tr>
  <tr> 
   <td>配信済みメール</td> 
   <td>ブラウザー、プラットフォーム、デバイス、ユーザエージェント</td>
  </tr>
   <tr> 
   <td>バウンスメール</td> 
   <td>ブラウザー、プラットフォーム、デバイス、ユーザエージェント</td>
  </tr>
  <tr> 
   <td>メールの配信停止</td> 
   <td>ブラウザー、プラットフォーム、デバイス</td>
  </tr>
  <tr> 
   <td>メールを開く</td> 
   <td>ブラウザー</td>
  </tr>
   <tr> 
   <td>メールをクリック</td> 
   <td>ブラウザー</td>
  </tr>
  <tr> 
   <td>ソフトバウンスメール</td> 
   <td>ブラウザー、プラットフォーム、デバイス、ユーザエージェント</td>
  </tr>
 </tbody> 
</table>
