---
unique-page-id: 14352484
description: Salesforce に接続する際の「リクエストを認証できませんでした」の修正方法 - Marketo ドキュメント - 製品ドキュメント
title: Salesforce に接続するf際の「リクエストを認証できませんでした」の修正方法
exl-id: ddd49064-f584-4490-8d45-29cf61ed3ebe
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '186'
ht-degree: 100%

---

# Salesforce に接続するf際の「リクエストを認証できませんでした」の修正方法 {#how-to-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

Sales Connect を Salesforce に接続しようとしたときに「リクエストを認証できませんでした」というエラーメッセージが表示された場合は、Salesforce の API へのアクセスに制約がある可能性があります。Salesforce 管理者に次の点を確認してください。

## ユーザー権限での API が有効化されている {#enable-api-in-user-permissions}

1. Salesforce 管理者が SFDC にログインしている
1. 「**設定**」を選択します。
1. 「**ユーザーを管理**」を選択します。
1. 「**プロファイル**」を選択します。
1. ToutApp ユーザーが属するプロファイルを探し、「**編集**」をクリックします。
1. 下の「**管理権限**」までスクロールし、「**API 有効**」がオンになっていることを確認します。

## Salesforce によって Sales Connect の接続がブロックされているかどうかを確認する {#check-if-salesforce-is-blocking-sales-connect-from-connecting}

1. Salesforce 管理者に SFDC にログインしてもらいます。
1. 「**設定**」を選択します。
1. 「**アプリの管理**」を選択します。
1. 「**接続済みのアプリケーションの OAuth 使用状況**」を選択します。
1. Sales Connect の横に「ブロック」と表示されていることを確認します。「ブロック解除」が表示されたらボタンをクリックして、Sales Connect の Salesforce へのアクセスのブロックを解除します。
