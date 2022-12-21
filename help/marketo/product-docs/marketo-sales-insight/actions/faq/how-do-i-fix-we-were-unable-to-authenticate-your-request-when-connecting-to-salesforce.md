---
description: Salesforce に接続する際の「リクエストを認証できませんでした」の修正方法 - Marketo ドキュメント - 製品ドキュメント
title: Salesforce に接続する際の「リクエストを認証できませんでした」の修正方法
exl-id: ef876f0f-bd76-4ba5-bf48-885ee048ceae
source-git-commit: d9b8b92ac5f051178b8eb9b450c4949b56d50b99
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 100%

---

# Salesforce に接続する際の「リクエストを認証できませんでした」の修正方法 {#how-do-i-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

Sales Insight を Sales Insight Actions に接続しようとしたときに「リクエストを認証できませんでした」というエラーメッセージが表示された場合は、Salesforce の API へのアクセスに制約がある可能性があります。Salesforce 管理者に次の点を確認してください。

## ユーザ権限での API が有効化されている {#enable-api-in-user-permissions}

1. Salesforce 管理者が SFDC にログインしている
1. 「**設定**」を選択します。
1. 「**ユーザを管理**」を選択します。
1. 「**プロファイル**」を選択します。
1. ToutApp ユーザが属するプロファイルを探し、「**編集**」をクリックします。
1. 下の「**管理権限**」までスクロールし、「**API 有効**」がオンになっていることを確認します。

## Salesforce によって Sales Insight Actions の接続がブロックされているかどうかを確認する {#check-if-salesforce-is-blocking-sales-insight-actions-from-connecting}

1. Salesforce 管理者に SFDC にログインしてもらいます。
1. 「**設定**」を選択します。
1. 「**アプリの管理**」を選択します。
1. 「**接続済みのアプリケーションの OAuth 使用状況**」を選択します。
1. Sales Insight Actions の横に「ブロック」と表示されていることを確認します。「ブロック解除」が表示されたらボタンをクリックして、Sales Insight Actions の Salesforce へのアクセスのブロックを解除します。
