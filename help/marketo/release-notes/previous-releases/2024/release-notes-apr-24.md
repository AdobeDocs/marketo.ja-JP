---
description: リリースノート - 2024 年 4 月 – Marketo ドキュメント – 製品ドキュメント
title: リリースノート - 2024年4月
feature: Release Information
exl-id: d87474f8-fc47-407b-bc97-e343b56c1f8f
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 71%

---

# リリースノート：2024年4月 {#release-notes-apr-24}

2024年4月リリースに含まれるすべての機能を以下に示します。機能の可用性については、お使いの Adobe Marketo Engage のエディションをご確認ください。

Adobe Dynamic Chat 専用のリリースノートについて詳しくは、[こちらを参照](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}してください。

>[!AVAILABILITY]
>
>星印（![星印](assets/yellow-star.png)）で示す機能は有償オプションです。詳しくは、Marketo Engage 担当営業にお問い合わせください。

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
   <td><strong>インタラクティブウェビナーの機能強化</strong>：ホストとプレゼンターに対して、ウェビナータイトルの追加、部屋名の変更、イベント配信後にエンゲージメントデータを手動で同期する機能を提供できるようになりました。</td>
   <td>リリース済み</td>
   <td><li><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/create-an-interactive-webinar.md">インタラクティブウェビナーの作成</a></li>
   <li><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/event-workflows.md#manual-sync">手動による同期</a></li></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
    <tr>
   <td><strong> 監査証跡の機能強化 </strong>:
   フィールド管理で行われた変更、ユーザーおよびロールに対して行われた変更、リストおよびスマート・リストからエクスポートされたユーザーの数に関する新しいタイプのアクションを監査証跡で取得できるようになりました。</td>
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
    <tr>
   <td><strong>新しいユーザ＆ロールの権限</strong>：新しい権限が利用可能になり、ユーザは Marketo Engage へのより詳細なアクセスが可能になります。新しいエクスペリエンスや予測オーディエンスなど、これまでゲートされていなかった管理部分を制御し、アセット監査記録と管理監査記録へのアクセス権を個別に付与する権限を分割し、アセットとフォルダーに対する新規作成および移動権限を利用して、読み取り専用ユーザが変更を行うことを防ぎます。
   <p>新しい権限は 4月26日（PT）以降、お使いの Marketo Engage インスタンスに表示されますが、現時点ではパッシブであり、今四半期後半にアクセス可能になる予定です。
   <li>Adobe Experience Managerへのアクセス</li>
   <li>Adobe組織マッピングへのアクセス</li>
   <li>Admin Audit Trail へのアクセス</li>
   <li>アセット監査証跡へのアクセス</li>
   <li>新しいエクスペリエンスにアクセス</li>
   <li>Predictive Audiences へのアクセス</li>
   <li>レポートを作成</li>
   <li>リストの作成</li>
   <li>キャンペーンアクティビティをエクスポート</li>
   </td>
   <td>リリース済み</td>
   <td><a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md">ロール権限の説明</a></td>
  </tr>
 </tbody>
</table>
<br/>

## お知らせ {#announcements}

* **アクティビティ API の更新**: 4 月 26 日（PT）に、[Marketo REST API](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Activities){target="_blank"} を使用してアクティビティを取得する際に返される web ベースのアクティビティとメールベースのアクティビティに、新しい属性をいくつか追加します。 以下にリストされるアクティビティに、ブラウザー、プラットフォーム、デバイスおよびユーザーエージェント属性が含まれるようになりました。 [&#x200B; アクティビティタイプを取得 &#x200B;](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Activities/operation/getAllActivityTypesUsingGET){target="_blank"} エンドポイントを呼び出して、各アクティビティの属性の詳細を確認します。

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
