---
description: Adobe IMSユーザー移行トラブルシューティングガイド - Marketo ドキュメント – 製品ドキュメント
title: Adobe IMSユーザー移行トラブルシューティングガイド
hide: true
hidefromtoc: true
feature: Marketo with Adobe Identity
exl-id: 921d9d45-c5c2-405c-bd3b-be8aa6d11e2f
source-git-commit: e96bc8676a73694ec60f46bb045f2a6ea5d8069c
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 0%

---

# Adobe IMSユーザー移行トラブルシューティングガイド {#adobe-ims-user-migration-troubleshooting-guide}

IMS ユーザーの移行プロセス中に、移行される各Adobe ユーザーに対してMarketo Engage ユーザーが 1 つ作成されます（同じメールアドレスで既に存在する場合を除く）。 作成されない場合がありますが、これは Active Directory 内のユーザーのレコードや、メールアドレスに関する問題が原因である可能性があります。 これが発生すると、Marketo Engage管理者には、self-migration console でユーザーの移行ステータスフィールドに理由が表示されます。

## エラー メッセージ {#error-messages}

まず、ユーザーを移行する必要があるかどうかを判断します。移行すると、どの解決手順に従うかに影響します。

特定のエラーに直接ジャンプするには、右側の「このページ上」のセクションを使用します。

### ディレクトリに存在しない {#not-in-directory}

**根本原因**：ユーザーが Active Directory （AD）に存在しません。 AD 同期が有効になっている SSO を持つ組織では、ユーザーの作成は ID プロバイダー（IdP）を通じてのみ許可されます。 そのため、ユーザーの移行中に、Admin Consoleを使用してユーザーを追加することはできません。

**解決策**:

_ユーザーを移行する必要がない場合_ - Marketo Engage admin で Migration Console のユーザーをスキップできます。 すべてのユーザーが移行またはスキップによって考慮されると、「移行完了」ボタンが表示されます。 ボタンをクリックして、ユーザー移行プロセスを終了します。

_ユーザーを移行する必要がある場合_ - システム管理者が適切な権限を持つユーザーを Active Directory に追加する必要があります。 Marketo Engage管理者は、このユーザーのユーザー移行を移行コンソールから再実行できます。

### Gmail 無効な文字 {#gmail-invalid-character}

**根本原因**:Adobe セキュリティポリシーにより、`.` と `+` の文字は Gmail メールアドレスでは使用できません。 Gmail 以外のメールアドレスでは、両方の文字を使用できます。

**解決策**:

_ユーザーを移行する必要がない場合_ - Marketo Engage admin で Migration Console のユーザーをスキップできます。 すべてのユーザーが移行またはスキップによって考慮されると、「移行完了」ボタンが表示されます。 ボタンをクリックして、ユーザー移行プロセスを終了します。

_ユーザーを移行する必要がある場合_ - Adobeのセキュリティポリシーに準拠して再検証できるように、メールアドレスをMarketo Engageで更新する必要があります。 Marketo管理者は、このユーザーのユーザー移行を移行コンソールから再実行できます。

### 非アクティブユーザー {#inactive-user}

**根本原因**:AD 同期が有効になっており、ユーザーのフェデレーテッド アカウントは存在しますが、非アクティブ/無効の状態です。

**解決策**:

_ユーザーを移行する必要がない場合_ - Marketo Engage admin で Migration Console のユーザーをスキップできます。 すべてのユーザーが移行またはスキップによって考慮されると、「移行完了」ボタンが表示されます。 ボタンをクリックして、ユーザー移行プロセスを終了します。

_ユーザーを移行する必要がある場合_ - ユーザーのステータスと適切な権限を復元する必要があります。 Marketo Engage管理者は、このユーザーのユーザー移行を移行コンソールから再実行できます。

### ドメインに含まれない {#not-in-domain}

**根本原因**:Admin Consoleではドメインの適用が有効になっていますが、ユーザーのメールアドレスのドメインが許可されているドメインではありません。

**解決策**:

_ユーザーを移行する必要がない場合_ - Marketo Engage admin で Migration Console のユーザーをスキップできます。 すべてのユーザーが移行またはスキップによって考慮されると、「移行完了」ボタンが表示されます。 ボタンをクリックして、ユーザー移行プロセスを終了します。

_ユーザーを移行する必要がある場合_ - ドメイン適用（DE）ポリシーに準拠するために、Marketo Engageでメールアドレスを更新する必要があります。 または、システム管理者は、[ ドメインを移動 ](https://helpx.adobe.com/enterprise/using/manage-domains-directories.html#move-domains-across-directories){target="_blank"} して、別のドメイン強制（DE）無効ディレクトリに移動するか、DE ポリシー下にない [ 新しいディレクトリを作成 ](https://helpx.adobe.com/jp/enterprise/using/set-up-identity.html){target="_blank"} することができます。 Marketo Engage管理者は、このユーザーのユーザー移行を移行コンソールから再実行できます。

### 失敗を作成 {#create-failure}

**根本原因**：このエラーは、バックエンドの様々な理由が原因で発生する可能性があります。

**解決策**:

[Marketo サポート ](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} の関連詳細を添えて、サポートケースを送信します。

### Type2e ユーザーエラー {#type2e-user-failure}

**根本原因**：このエラーは、バックエンドの様々な理由が原因で発生する可能性があります。

**解決策**:

[Marketo サポート ](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} の関連詳細を添えて、サポートケースを送信します。
