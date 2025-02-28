---
description: Adobe IMSトラブルシューティングガイド - Marketo ドキュメント – 製品ドキュメント
title: Adobe IMSトラブルシューティングガイド
hide: true
hidefromtoc: true
feature: Marketo with Adobe Identity
exl-id: 921d9d45-c5c2-405c-bd3b-be8aa6d11e2f
source-git-commit: 2a01045abbc23bce9531c64e3494fb12a9adf1bd
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# Adobe IMSトラブルシューティングガイド {#adobe-ims-troubleshooting-guide}

IMS ユーザーの移行プロセス中に、移行する各Adobe ユーザーに対してMarketo Engage ユーザーが 1 つ作成されます。 場合によっては、作成されないことがあります（様々な理由で、Active Directory 内のユーザーのレコードやメールアドレスの問題に関連しています）。 これが発生すると、Marketo Engage管理者には、self-migration console 上のユーザーの移行ステータスフィールドに理由が表示されます。

## エラー メッセージ {#error-messages}

右側の「このページで」の節を使用して、特定のエラーに直接ジャンプし、その解決方法を学びます。

### ディレクトリに存在しない {#not-in-directory}

_根本原因_：ユーザーが Active Directory （AD）に存在しません。 AD 同期が有効になっている SSO を持つ組織では、ユーザーの作成は ID プロバイダー（IdP）を通じてのみ許可されます。 そのため、ユーザーの移行中に、Admin Consoleを使用してユーザーを追加することはできません。

_解決策_:

事前移行 – Marketo管理者が移行コンソールでユーザーをスキップできます。 すべてのユーザーが移行またはスキップによって考慮されると、「移行完了」ボタンが表示されます。 ボタンをクリックして、ユーザー移行プロセスを終了します。

移行後：適切な権限を持つユーザーを Active Directory に追加する必要があります。 Marketo Engage管理者は、このユーザーのユーザー移行を移行コンソールから再実行してください。

### Gmail 無効な文字 {#gmail-invalid-character}

_根本原因_:Adobe セキュリティポリシーにより、`.` と `+` の文字は Gmail メールアドレスでは使用できません。 Gmail 以外のメールアドレスでは、両方の文字を使用できます。

_解決策_:

事前移行 – Marketo管理者が移行コンソールでユーザーをスキップできます。 すべてのユーザーが移行またはスキップによって考慮されると、「移行完了」ボタンが表示されます。 ボタンをクリックして、ユーザー移行プロセスを終了します。

移行後 – Adobeのセキュリティポリシーに従って、メールアドレスをMarketo Engageで更新する必要があります。 Marketo管理者が、移行コンソールからこのユーザーのユーザー移行を再実行します。

### 非アクティブユーザー {#inactive-user}

_根本原因_:AD 同期が有効になっており、ユーザーのフェデレーテッド アカウントは存在しますが、非アクティブ/無効の状態です。

_解決策_:

事前移行 – Marketo管理者が移行コンソールでユーザーをスキップできます。 すべてのユーザーが移行またはスキップによって考慮されると、「移行完了」ボタンが表示されます。 ボタンをクリックして、ユーザー移行プロセスを終了します。

移行後 – ユーザーのステータスと適切な権限を復元する必要があります。 Marketo Engage管理者は、このユーザーのユーザー移行を移行コンソールから再実行してください。

### ドメインに含まれない {#not-in-domain}

_根本原因_:Admin Consoleではドメインの適用が有効になっていますが、ユーザーのメールアドレスのドメインが許可されているドメインではありません。

_解決策_:

事前移行 – Marketo管理者が移行コンソールでユーザーをスキップできます。 すべてのユーザーが移行またはスキップによって考慮されると、「移行完了」ボタンが表示されます。 ボタンをクリックして、ユーザー移行プロセスを終了します。

移行後 – ドメイン適用（DE）ポリシーに準拠するために、メールアドレスをMarketo Engageで更新する必要があります。 または、システム管理者は、[ ドメインを移動 ](https://helpx.adobe.com/enterprise/using/manage-domains-directories.html#move-domains-across-directories){target="_blank"} して、別のドメイン強制（DE）無効ディレクトリに移動するか、DE ポリシー下にない [ 新しいディレクトリを作成 ](https://helpx.adobe.com/jp/enterprise/using/set-up-identity.html){target="_blank"} することができます。 Marketo Engage管理者は、このユーザーのユーザー移行を移行コンソールから再実行してください。

### 失敗を作成 {#create-failure}

_根本原因_：このエラーは、バックエンドの様々な理由が原因で発生する可能性があります。

_解決策_:

移行前 – [ まだ移行されていない ](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} 移行のサポートケースを送信してください。

移行後 – （既に移行されている [ のサポートケースを送信し ](https://experienceleague.adobe.com/home?support-tab=home#support){target="_blank"} ください。

### Type2e ユーザーエラー {#type2e-user-failure}

_根本原因_：このエラーは、バックエンドの様々な理由が原因で発生する可能性があります。

_解決策_:

移行前 – [ まだ移行されていない ](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} 移行のサポートケースを送信してください。

移行後 – （既に移行されている [ のサポートケースを送信し ](https://experienceleague.adobe.com/home?support-tab=home#support){target="_blank"} ください。
