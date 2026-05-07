---
description: Sales Insight ActionsをSalesforceに接続する際の認証エラーを修正します。 OAuth、権限、接続手順を確認します。
title: Salesforce に接続する際の「リクエストを認証できませんでした」の修正方法
exl-id: ef876f0f-bd76-4ba5-bf48-885ee048ceae
feature: Sales Insight Actions
source-git-commit: 240b78561db11e169188698880d4707a5c1f64de
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 71%

---

# [!DNL Salesforce] に接続する際の「リクエストを認証できませんでした」の修正方法 {#how-do-i-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

Marketo Sales インスタンスをSalesforceに接続しようとしていて、「リクエストを認証できません」というエラーが表示される場合は、Salesforce インスタンスの設定方法に関連している可能性があります。

この失敗した認証ページを生成する可能性のあるエラーには、次の 2 種類があります。

* Login error restricted Domain
* Oauth アプリがブロックされました

URLを確認することで、取得するタイプを特定できます。

![](assets/how-do-i-fix-we-were-unable-to-authenticate-1.png)

![](assets/how-do-i-fix-we-were-unable-to-authenticate-2.png)

## 制限ドメインのログイン エラーの解決 {#resolve-login-error-restricted-domain}

このエラーは通常、ルーティングできないカスタムドメインがあることを示しています。 このエラーを解決するには、まず接続先の Salesforce インスタンスにログインしてみてください。 次に、手順を実行して Salesforce に接続します。

接続先のインスタンスがSalesforce サンドボックスのドメインで、エラーが発生した場合は、インスタンスを更新してSalesforce サンドボックスに対応するように追加の手順を実行する必要があります。 [詳細情報](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/set-up-a-sales-insight-actions-sandbox.md){target="_blank"}

## Oauth アプリの解決がブロックされました {#resolve-oauth-app-blocked}

URL 内に「Oauth App Blocked」というエラータイプ（または別のタイプ）が記載された「要求を認証できませんでした」というエラーメッセージが表示された場合は、Salesforce API へのアクセスが制限されている可能性があります。 Salesforce 管理者に、以下が実施されていることを確認してください。

### ユーザ権限での API の有効化 {#enable-api-in-user-permissions}

1. Salesforce 管理者を Salesforce にログインしてもらいます。
1. 「**設定**」を選択します。
1. 「**ユーザを管理**」を選択します。
1. 「**プロファイル**」を選択します。
1. ToutApp ユーザが属するプロファイルを探し、「**編集**」をクリックします。
1. 下の「**管理権限**」までスクロールし、「**API 有効**」がオンになっていることを確認します。

### Salesforce によってセールスインサイトアクションの接続がブロックされているかどうかを確認する {#check-if-salesforce-is-blocking-sales-insight-actions-from-connecting}

1. Salesforce 管理者を Salesforce にログインしてもらいます。
1. 「**設定**」を選択します。
1. 「**アプリの管理**」を選択します。
1. 「**接続済みのアプリケーションの OAuth 使用状況**」を選択します。
1. セールスインサイトアクションの横に「ブロック」と表示されていることを確認します。 「ブロック解除」と表示された場合は、このボタンをクリックして、セールスインサイトアクションの Salesforce へのアクセスのブロックを解除します。
