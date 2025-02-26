---
description: Adobe IMSトラブルシューティングガイド - Marketo ドキュメント – 製品ドキュメント
title: Adobe IMSトラブルシューティングガイド
hide: true
hidefromtoc: true
feature: Marketo with Adobe Identity
source-git-commit: eccebb8352c56770dea5af9395c8bc83a08525dd
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 0%

---

# Adobe IMSトラブルシューティングガイド {#adobe-ims-troubleshooting-guide}

IMS ユーザーの移行プロセス中に、移行する各Adobe ユーザーに対してMarketo Engage ユーザーが 1 つ作成されます。 場合によっては、作成されないことがあります（様々な理由で、Active Directory 内のユーザーのレコードやメールアドレスの問題に関連しています）。 これが発生すると、Marketo Engage管理者には、self-migration console 上のユーザーの移行ステータスフィールドに理由が表示されます。 Adobe ユーザーの作成に関する様々な問題を解決する方法については、以下を参照してください。

## エラー メッセージ {#error-messages}

* <a href="#not-in-directory"> ディレクトリにない </a>
* <a href="#gmail-invalid-character">Gmail 無効な文字 </a>
* <a href="#inactive-user"> 非アクティブユーザー </a>
* <a href="#not-in-domain"> ドメインに存在しない </a>
* <a href="#create-failure"> 作成エラー </a>
* <a href="#type2e-user-failure">Type2e ユーザーエラー </a>



<table>
<thead>
  <tr>
    <th style="width:20%">エラー メッセージ</th>
    <th style="width:40%">根本原因</th>
    <th style="width:40%">解決策</th>
  </tr>
  </thead>
<tbody>
  <tr>
    <td><i><a id="not-in-directory">ディレクトリに存在しない</a></i></td>
    <td>ユーザーが Active Directory （AD）に存在しません。 AD 同期が有効になっている SSO を持つ組織では、ユーザーの作成は ID プロバイダー（IdP）を通じてのみ許可されます。 そのため、ユーザーの移行中に、Admin Consoleを使用してユーザーを追加できませんでした。</td>
    <td>移行 – ユーザーは、適切な権限を持つ Active Directory に追加する必要があります。 Marketo管理者が、移行コンソールからこのユーザーのユーザー移行を再実行します。 
    <br> 移行しない – Marketo管理者が移行コンソールでユーザーをスキップできます。 移行またはスキップですべてのユーザーが考慮されると、「移行完了」ボタンが表示されます。 クリックして、ユーザー移行プロセスを終了します。</td>
  </tr>
  <tr>
    <td><i><a id="gmail-invalid-character">Gmail 無効な文字</a></i></td>
    <td>Adobeのセキュリティポリシーごとに、「。」 および「+」記号は、Gmail ドメインのみのメールアドレスでは使用できません  
    <br>Gmail ドメイン以外のメールアドレスでは、両方の特殊文字を使用できます。 </td>
    <td>移行 – Adobeのセキュリティポリシーに準拠するには、Marketo Engageでメールアドレスを更新する必要があります。 Marketo管理者が、移行コンソールからこのユーザーのユーザー移行を再実行します。<br> 移行しない – Marketo管理者が移行コンソールでユーザーをスキップできます。 移行またはスキップですべてのユーザーが考慮されると、「移行完了」ボタンが表示されます。 クリックして、ユーザー移行プロセスを終了します。</td>
  </tr>
  <tr>
    <td><i><a id="inactive-user">非アクティブユーザー</a></i></td>
    <td>AD 同期が有効で、ユーザーのフェデレーテッド アカウントは存在しますが、非アクティブ/無効の状態です。</td>
    <td>移行 – ユーザーのステータスと適切な権限を復元する必要があります。 Marketo管理者が、移行コンソールからこのユーザーのユーザー移行を再実行します。
    <br> 移行しない – Marketo管理者が移行コンソールでユーザーをスキップできます。 移行またはスキップですべてのユーザーが考慮されると、「移行完了」ボタンが表示されます。 クリックして、ユーザー移行プロセスを終了します。</td>
  </tr>
  <tr>
    <td><i><a id="not-in-domain">ドメインに含まれない</a></i></td>
    <td>Admin Consoleではドメインの適用が有効になっていますが、ユーザーのメールアドレスのドメインが許可されているドメインではありません。 
    <br> ドメイン強制ポリシーは、ディレクトリレベルで設定されます。</td>
    <td>移行 – ドメインの実施ポリシーに準拠するようにメールアドレスをMarketo Engageで更新する必要があります。更新しない場合は、システム管理者が <a href="https://helpx.adobe.com/enterprise/using/manage-domains-directories.html#move-domains-across-directories"> のいずれかを実行できます 
    ドメインを、DE ポリシーの下にない、別のドメイン強制（DE）無効ディレクトリに移動する </a> または <a href="https://helpx.adobe.com/jp/enterprise/using/set-up-identity.html"> 新しいディレクトリを作成する </a>。 Marketo管理者が、移行コンソールからこのユーザーのユーザー移行を再実行します。 <br> 移行しない – Marketo管理者が移行コンソールでユーザーをスキップできます。 移行またはスキップですべてのユーザーが考慮されると、「移行完了」ボタンが表示されます。 クリックして、ユーザー移行プロセスを終了します。</td>
  </tr>
  <tr>
    <td><i><a id="create-failure">失敗を作成</a></i></td>
    <td>バックエンドには様々な理由があります。</td>
    <td>サポートケースを送信してください。</td>
  </tr>
  <tr>
    <td><i><a id="type2e-user-failure">Type2e ユーザーエラー</a></i></td>
    <td>バックエンドには様々な理由があります。</td>
    <td>サポートケースを送信してください。</td>
  </tr>
</tbody>
</table>
