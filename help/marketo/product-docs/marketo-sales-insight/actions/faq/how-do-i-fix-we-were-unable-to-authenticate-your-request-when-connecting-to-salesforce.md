---
description: Salesforce に接続する際の「リクエストを認証できませんでした」の修正方法 - Marketo ドキュメント - 製品ドキュメント
title: Salesforce に接続する際の「リクエストを認証できませんでした」の修正方法
exl-id: ef876f0f-bd76-4ba5-bf48-885ee048ceae
feature: Sales Insight Actions
source-git-commit: e6d939eca9731dc9df8ea506090a049e8741fa07
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 37%

---

# Salesforce に接続する際の「リクエストを認証できませんでした」の修正方法 {#how-do-i-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

Marketo Sales インスタンスを Salesforce に接続しようとして、「リクエストを認証できません」というエラーが表示された場合は、Salesforce インスタンスの設定方法に関連している可能性があります。

この認証失敗ページを生成できるエラーには 2 種類があります。

* ログインエラーが制限されたドメイン
* OAuth アプリがブロックされました

URL を確認することで、取得するタイプを識別できます。

![](assets/how-do-i-fix-we-were-unable-to-authenticate-1.png)

![](assets/how-do-i-fix-we-were-unable-to-authenticate-2.png)

## ログインエラーの制限ドメインの解決 {#resolve-login-error-restricted-domain}

このエラーは、通常、ルーティングできないカスタムドメインがあることを示します。 このエラーを解決するには、最初に接続する Salesforce インスタンスにサインインしてみてください。 次に、Salesforce に接続する手順を実行します。

接続しようとしているインスタンスが Salesforce Sandbox ドメインで、エラーが発生した場合は、追加の手順を実行して、Salesforce Sandbox と互換性を持つようにインスタンスを更新する必要があります。 [詳細情報](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/set-up-a-sales-insight-actions-sandbox.md){target="_blank"}

## ブロックされた OAuth アプリの解決 {#resolve-oauth-app-blocked}

URL に「Oauth App Blocked」エラータイプまたは別のタイプのエラーメッセージが表示された場合は、Salesforce の API へのアクセスに制限が生じる可能性があります。 Salesforce 管理者に次の点を確認してください。

### ユーザ権限での API が有効化されている {#enable-api-in-user-permissions}

1. Salesforce 管理者に Salesforce にログインしてもらう。
1. 「**設定**」を選択します。
1. 「**ユーザを管理**」を選択します。
1. 「**プロファイル**」を選択します。
1. ToutApp ユーザが属するプロファイルを探し、「**編集**」をクリックします。
1. 下の「**管理権限**」までスクロールし、「**API 有効**」がオンになっていることを確認します。

### Salesforce によって Sales Insight Actions の接続がブロックされているかどうかを確認する {#check-if-salesforce-is-blocking-sales-insight-actions-from-connecting}

1. Salesforce 管理者に Salesforce にログインしてもらう。
1. 「**設定**」を選択します。
1. 「**アプリの管理**」を選択します。
1. 「**接続済みのアプリケーションの OAuth 使用状況**」を選択します。
1. Sales Insight Actions の横に「ブロック」と表示されていることを確認します。「ブロック解除」が表示された場合は、ボタンをクリックして、Salesforce への Sales Insight アクションのアクセスをブロック解除します。
