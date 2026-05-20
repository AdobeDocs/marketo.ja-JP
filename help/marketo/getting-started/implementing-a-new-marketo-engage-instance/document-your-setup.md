---
description: 新しいMarketo Engage インスタンスの設定を文書化します。
title: 新しいインスタンスのベストプラクティス – 設定のドキュメント化
feature: Getting Started
exl-id: c64d25e8-564b-487d-824e-7fcbfbf5d8bb
TQID: https://experienceleague.adobe.com/pqbf84tAUt49rWUD7rONRuZNgR8v5yMmYTqwqlXqgAs
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45id: c5f60233-d5ea-4453-a799-0ad258b4d399id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: e64968b2-4ee5-47f9-8cae-0588f184b9eb
topic_v2: id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adebid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 536
ht-degree: 57%

---

# 新しいインスタンスのベストプラクティス：設定のドキュメント化 {#new-instance-best-practices-document-your-setup}

新しいMarketo Engage インスタンスを設定するための主な製品領域を理解したら、次のステップは、インスタンス設定とテクノロジースタックのドキュメントを作成することです。 スプレッドシートやプロジェクト管理アプリケーションなど、ドキュメントは、進捗状況や記録の詳細を追跡し、インスタンスを構造化し、組織内の将来のマーケターのために持続可能な状態に保つための優れたリソースです。

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
    <td><li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/quick-wins/import-a-list-of-people" target="_blank">Marketo Engage に読み込む</a>レコードの取得元となるデータソースのリストを収集します。</li>
    <li>複数のデータソースから読み込む場合は、マスターリストを使用するか、個人レコードに<a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo" target="_blank"> カスタムフィールドを作成して</a> データソースを示すことを検討してください。</li></td>
  </tr>
  <tr>
    <td>データベース統合</td>
    <td><li>Marketo Engage と CRM の間のネイティブ同期を活用する場合は、システム間で同期するフィールドを注意深く検討してください。 すべてのフィールドを同期する必要はないので、データフローについて戦略的に考えましょう。</li></td>
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
    <td><li>安全上の理由から、インスタンス内の<a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user#add-a-user" target="_blank">現在のユーザ</a>をドキュメント化します。 以下の詳細は少なくとも含める必要があります（また、すべて管理者/ ユーザーと役割に移動すると表示されます）。</li>
    <ul>
    <li>名前</li>
    <li>メール</li>
    <li>ログイン</li>
    <li>役割</li>
    <li>アクセス有効期限</li>
    <li>ユーザー作成日</li>
    <li>最新のログイン日</li></ul>
    <p><img src="assets/note-icon.png" alt="メモアイコン"> メモ：この機能を拡張して、役割や権限に関するドキュメントを追加することもできます。
    <p>
    <li>Marketo Engage 製品管理者は、Marketo Engage ユーザリストを定期的に監査および更新する社内プロセスを開発します。 Adobe Admin Consoleのユーザーリストに変更を加えるには、.CSVのアップロード、User Management REST APIの使用など、<a href="https://helpx.adobe.com/jp/enterprise/using/users.html" target="_blank">一括アクション </a>を検討します。</li></td>
  </tr>
  <tr>
    <td>組織</td>
    <td><li>合意されたフォルダー構造、プログラム、アセットなどの標準的な命名規則、意思決定の背景にある「なぜ」を文書化します。 <a href="https://experienceleague.adobe.com/ja/docs/marketo-learn/tutorials/fundamentals/best-practices-to-organize-a-new-instance" target="_blank">詳しくは、こちらにあるベストプラクティスを参照してください。</a></li></td>
  </tr>
  <tr>
    <td>変更ログ</td>
    <td><li>インスタンスの変更内容と変更の理由をドキュメント化できる変更ログを作成します。 <a href="https://experienceleague.adobe.com/ja/docs/marketo-learn/auditing-an-inherited-instance/develop-an-instance-governance-guide" target="_blank">詳しくは、こちらにあるベストプラクティスを参照してください。</a></li></td>
  </tr>
  <tr>
    <td>プレイブック</td>
    <td><li>インスタンスにオンボーディングする社内ユーザ用のユーザプレイブックまたは管理者プレイブックを作成します。</li></td>
  </tr>
  <tr>
    <td>社内チームとの対話</td>
    <td><li>Marketo Engageに対する社内のマーケティングチームの期待とMarketo Engageの能力を一致させることができます。</li>
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
