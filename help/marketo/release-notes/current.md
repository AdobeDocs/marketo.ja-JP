---
description: 最新のリリースノート - Marketo ドキュメント - 製品ドキュメント
title: 最新のリリースノート
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 433aae54a012e6bbf04c90056d8815a88e76498c
workflow-type: ht
source-wordcount: '380'
ht-degree: 100%

---

# リリースノート：2024年4月 {#release-notes-apr-24}

2024年4月リリースに含まれるすべての機能を以下に示します。機能の可用性についてはお使いの Marketo Engage のエディションをご確認ください。

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
   <td><strong>インタラクティブウェビナー用のテンプレート</strong>：組織に合った仕様でブランド化された部屋レイアウトのカスタムテンプレートを作成して、時間を節約できます。</td> 
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
   <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
   </tr>
     <tr> 
   <td><strong>インタラクティブウェビナーの機能強化</strong>：ホストと発表者に対して、ウェビナータイトルの追加、部屋名の変更、イベント配信後にエンゲージメントデータを手動で同期する機能を提供できるようになりました。</td> 
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
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
   <td><strong>新しいユーザ＆ロールの権限</strong>：新しい権限が利用可能になり、ユーザは Marketo Engage へのより詳細なアクセスが可能になります。新しいエクスペリエンスや予測オーディエンスなど、これまでゲートされていなかった管理部分を制御し、アセット監査記録と管理監査記録へのアクセス権を個別に付与する権限を分割し、アセットとフォルダーに対する新規作成および移動権限を利用して、読み取り専用ユーザが変更を行うことを防ぎます。</td> 
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
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
