---
description: Salesforce に接続する際の「リクエストを認証できませんでした」の修正方法 — Marketoドキュメント — 製品ドキュメント
title: Salesforce に接続する際の「リクエストを認証できませんでした」の修正方法
hide: true
hidefromtoc: true
source-git-commit: c398aff77e09f4a63db5d51af55178aa663ec98e
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 38%

---

# Salesforce に接続する際の「リクエストを認証できませんでした」の修正方法 {#how-do-i-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

Sales Insight のアクションを Salesforce に接続しようとした際に「リクエストを認証できませんでした」というエラーメッセージが表示された場合は、Salesforce の API へのアクセスに制限がある可能性があります。 Salesforce 管理者に次の点を確認してください。

## ユーザー権限での API が有効化されている {#enable-api-in-user-permissions}

1. Salesforce 管理者が SFDC にログインしている
1. 「**設定**」を選択します。
1. 「**ユーザーを管理**」を選択します。
1. 「**プロファイル**」を選択します。
1. ToutApp ユーザーが属するプロファイルを探し、「**編集**」をクリックします。
1. 下の「**管理権限**」までスクロールし、「**API 有効**」がオンになっていることを確認します。

## Salesforce が Sales Insight のアクションを接続からブロックしているかどうかを確認 {#check-if-salesforce-is-blocking-sales-insight-actions-from-connecting}

1. Salesforce 管理者に SFDC にログインしてもらいます。
1. 「**設定**」を選択します。
1. 「**アプリの管理**」を選択します。
1. 「**接続済みのアプリケーションの OAuth 使用状況**」を選択します。
1. Sales Insight のアクションの横に「ブロック」が表示されていることを確認します。 「ブロック解除」が表示された場合は、ボタンをクリックして、Salesforce への Sales Insight アクションのアクセスをブロック解除します。
