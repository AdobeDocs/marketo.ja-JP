---
description: 最新のリリースノート - Marketo ドキュメント - 製品ドキュメント
title: 最新のリリースノート
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 433aae54a012e6bbf04c90056d8815a88e76498c
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 36%

---

# リリースノート：2024 年 4 月 {#release-notes-apr-24}

2024 年 4 月リリースに含まれるすべての機能を以下に示します。 機能の可用性についてはお使いの Marketo Engage のエディションをご確認ください。

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
   <td><strong>インタラクティブ Web セミナーのテンプレート</strong>：組織に合った仕様の部屋レイアウト用のカスタムテンプレートを作成して、時間を節約できます。</td> 
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
   <td><strong>インタラクティブ Web セミナーの強化</strong>：ホストおよびプレゼンターに対して、ウェビナータイトルの追加、部屋名の変更、イベント配信後のエンゲージメントデータの手動同期をおこなう機能を提供できるようになりました。</td> 
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>監査証跡の強化</strong>：フィールド管理でおこなわれた変更、ユーザーと役割に対する変更、リストおよびスマートリストからエクスポートされたユーザーの数に関して、監査証跡に新しいタイプのアクションを取り込めるようになりました。</td> 
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>新しいユーザーと役割の権限</strong>：新しい権限が使用でき、ユーザーにより詳細なアクセス権を提供します。Marketo Engage。 管理者の一部は、以前は New Experience や Predictive Audiences などと統合されていなかったものの、アセット監査記録と管理監査証跡へのアクセス権を個別に付与する権限を分割し、読み取り専用ユーザーが変更できないように、アセットとフォルダーに対する新しい作成および移動権限を利用します。</td> 
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## お知らせ {#announcements}

* **アクティビティ API の更新**:4 月 27 日に、Web ベースおよび E メールベースのアクティビティに、 [Marketo REST API](https://developers.marketo.com/rest-api/lead-database/activities/){target="_blank"}. The activities listed below will now include Browser, Platform, Device, and User Agent attributes. Call the [Get Activity Types](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Activitys/getAllActivityTypesUsingGET){target="_blank"} エンドポイント：各アクティビティの属性の詳細を確認します。

**Web ベースのアクティビティ**

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:30%">アクティビティ</th> 
   <th style="width:70%">新しく追加された属性</th>
   </tr>
  <tr> 
   <td>Visit Webpage</td> 
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

**電子メールベースのアクティビティ**

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:30%">アクティビティ</th> 
   <th style="width:70%">新しく追加された属性</th>
  </tr>
   <tr> 
   <td>メールの送信</td> 
   <td>ブラウザー、プラットフォーム、デバイス、ユーザーエージェント</td>
  </tr>
   </tr>
  <tr> 
   <td>配信済みメール</td> 
   <td>ブラウザー、プラットフォーム、デバイス、ユーザーエージェント</td>
  </tr>
   <tr> 
   <td>バウンスメール</td> 
   <td>ブラウザー、プラットフォーム、デバイス、ユーザーエージェント</td>
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
   <td>ブラウザー、プラットフォーム、デバイス、ユーザーエージェント</td>
  </tr>
 </tbody> 
</table>
