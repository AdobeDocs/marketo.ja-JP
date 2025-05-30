---
description: 新しいMarketo Engageインスタンスの設定を文書化します。
title: 新しいインスタンスのベストプラクティス – 設定のドキュメント化
feature: Getting Started
exl-id: c64d25e8-564b-487d-824e-7fcbfbf5d8bb
source-git-commit: 14583b7fa148aa2b03c8cf6316b9a106c11717b7
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 52%

---

# 新しいインスタンスのベストプラクティス：設定のドキュメント化 {#new-instance-best-practices-document-your-setup}

これで、新しいMarketo Engageインスタンスの設定に必要な主要な製品領域を説明したので、次の手順は、お使いのインスタンス設定とテクニカルスタックに関するドキュメントを作成することです。 スプレッドシートやプロジェクト管理アプリケーションを使用して作成する場合でも、ドキュメントは、進捗を追跡し、詳細を記録し、組織内の将来のマーケターのためにインスタンスを構造化し、持続可能な状態に保つための優れたリソースとなります。

## データ {#data}

<table>
<thead>
  <tr>
    <th style="width:20%">エリア</th>
    <th style="width:80%">アクション項目</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>リストの読み込み</td>
    <td><li><a href="https://experienceleague.adobe.com/ja/docs/marketo/using/getting-started/quick-wins/import-a-list-of-people" target="_blank">Marketo Engage に読み込む</a>レコードの取得元となるデータソースのリストを収集します。</li>
    <li>複数のデータソースから読み込む場合は、マスターリストを使用するか、人物レコードで <a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo" target="_blank"> カスタムフィールドの作成 </a> を使用して、データソースを示すことを検討してください。</li></td>
  </tr>
  <tr>
    <td>データベース統合</td>
    <td><li>Marketo Engage と CRM の間のネイティブ同期を活用する場合は、システム間で同期するフィールドを注意深く検討してください。すべてのフィールドを同期する必要はないので、データフローについて戦略的に考えましょう。</li></td>
  </tr>
</tbody>
</table>

## ドキュメント {#documentation}

<table>
<thead>
  <tr>
    <th style="width:20%">エリア</th>
    <th style="width:80%">アクション項目</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>ユーザ</td>
    <td><li>安全上の理由から、インスタンス内の<a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user#add-a-user" target="_blank">現在のユーザ</a>をドキュメント化します。少なくとも次の詳細を含める必要があります（また、すべての詳細は、管理者/ ユーザーと役割に移動すると表示されます）。</li>
    <ul>
    <li>名前</li>
    <li>メール</li>
    <li>ログイン</li>
    <li>ロール</li>
    <li>アクセスの有効期限</li>
    <li>ユーザー作成日</li>
    <li>最新のログイン日</li></ul>
    <p><img src="assets/note-icon.png" alt="メモアイコン"> メモ：これを拡張して、役割/権限に関するドキュメントを含めることもできます。
    <p>
    <li>Marketo Engage 製品管理者は、Marketo Engage ユーザリストを定期的に監査および更新する社内プロセスを開発します。Adobe Admin Consoleのユーザーのリストを変更するには、.CSV のアップロードや User Management REST API の使用など、<a href="https://helpx.adobe.com/jp/enterprise/using/users.html" target="_blank"> 一括アクション </a> を検討します。</li></td>
  </tr>
  <tr>
    <td>組織</td>
    <td><li>合意したフォルダー構造、プログラムやアセットなどの標準命名規則、および決定の背後にある理由を文書化します。 <a href="https://experienceleague.adobe.com/ja/docs/marketo-learn/tutorials/fundamentals/best-practices-to-organize-a-new-instance" target="_blank">詳しくは、こちらにあるベストプラクティスを参照してください。</a></li></td>
  </tr>
  <tr>
    <td>変更ログ</td>
    <td><li>インスタンスの変更内容と変更の理由をドキュメント化できる変更ログを作成します。<a href="https://experienceleague.adobe.com/ja/docs/marketo-learn/auditing-an-inherited-instance/develop-an-instance-governance-guide" target="_blank">詳しくは、こちらにあるベストプラクティスを参照してください。</a></li></td>
  </tr>
  <tr>
    <td>プレイブック</td>
    <td><li>インスタンスにオンボーディングする社内ユーザ用のユーザプレイブックまたは管理者プレイブックを作成します。</li></td>
  </tr>
  <tr>
    <td>社内チームとの対話</td>
    <td><li>社内マーケティングチームのMarketo Engageに対する期待を、Marketo Engageの能力に合わせます。</li>
    <li>Marketo Engage インスタンスの関係者となるチームを特定し、Marketo Engage をテクノロジーとして使用して達成する目標をドキュメント化します。</li></td>
  </tr>
  <tr>
    <td>ワークスペースとパーティション（該当する場合）</td>
    <td><li>ワークスペースの定義方法と、データベースパーティションへの関連付け（つまり、すべてのユーザとビジネスセクターとの比較が表示されるグローバルワークスペース）をドキュメント化します。</li>
    <li>適切なパーティションに新しいレコードを読み込みます。</li>
    <li>適切なパーティションにユーザを配置する値を CRM で定義します。</li></td>
  </tr>
</tbody>
</table>
