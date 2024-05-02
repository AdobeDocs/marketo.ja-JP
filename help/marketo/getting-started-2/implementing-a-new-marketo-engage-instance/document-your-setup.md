---
description: 新しいMarketo Engageインスタンスの設定を文書化します。
title: 新しいインスタンスのベストプラクティス – 設定のドキュメント化
hide: true
hidefromtoc: true
feature: Getting Started
exl-id: c64d25e8-564b-487d-824e-7fcbfbf5d8bb
source-git-commit: 3004885d1b6b986eb30072d2f67c5bd29ad251c7
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 69%

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
    <td><li><a href="https://experienceleague.adobe.com/ja/docs/marketo/using/getting-started-with-marketo/quick-wins/import-a-list-of-people" target="_blank">Marketo Engage に読み込む</a>レコードの取得元となるデータソースのリストを収集します。</li>
    <li>複数のデータソースから読み込む場合は、マスターリストを使用するか、個人レコードにデータソースを示す<a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo" target="_blank">カスタムフィールドを作成</a>することを検討してください。</li></td>
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
    <td><li>安全上の理由から、インスタンス内の<a href="https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user#add-a-user" target="_blank">現在のユーザ</a>をドキュメント化します。少なくとも次の詳細を含める必要があります（Adobe Admin Console／ユーザに移動すると、すべて表示されます）。</li>
    <br>名前
    <br>メール
    <br>ID タイプ
    <br>製品プロファイル
    <p>
    <li>Marketo Engage 製品管理者は、Marketo Engage ユーザリストを定期的に監査および更新する社内プロセスを開発します。Adobe Admin Consoleのユーザーリストを変更するには、 <a href="https://helpx.adobe.com/jp/enterprise/using/users.html" target="_blank">一括アクション</a>.csv のアップロード、User Management REST API の使用など。</li></td>
  </tr>
  <tr>
    <td>組織</td>
    <td><li>合意されたフォルダー構造、プログラム、アセットなどの標準命名規則と、決定の背後にある理由をドキュメント化します。<a href="https://experienceleague.adobe.com/ja/docs/marketo-learn/tutorials/fundamentals/best-practices-to-organize-a-new-instance" target="_blank">詳しくは、こちらにあるベストプラクティスを参照してください。</a></li></td>
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
    <td><li>社内マーケティングチームの Marketo Engage に対する期待と Marketo Engage の機能の整列を開始します。</li>
    <li>Marketo Engage インスタンスの関係者となるチームを特定し、Marketo Engage をテクノロジーとして使用して達成する目標をドキュメント化します。</li></td>
  </tr>
</tbody>
</table>
