---
unique-page-id: 14352484
description: Salesforce - Marketo Docs — 製品ドキュメントに接続する際の「要求を認証できませんでした」の修正方法
title: Salesforceに接続する際の「要求を認証できませんでした」の修正方法
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---


# Salesforceに接続する際の「要求を認証できませんでした」の修正方法{#how-to-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

Sales ConnectをSalesforceに接続しようとしたときに「要求を認証できませんでした」というエラーメッセージが表示された場合は、SalesforceのAPIへのアクセスに制限がある可能性があります。 Salesforce管理者に問い合わせて、以下の項目が正しいことを確認してください。

## ユーザー権限でAPIを有効にする{#enable-api-in-user-permissions}

1. Salesforce管理者にSFDCにログインしてもらいます。
1. 「**セットアップ**」を選択します。
1. 「**ユーザーを管理**」を選択します。
1. **プロファイル**&#x200B;を選択します。
1. ToutAppユーザーが属するプロファイルを探し、**編集**&#x200B;をクリックします。
1. 「**管理権限**」まで下にスクロールし、「**APIが有効**」がオンになっていることを確認します。

## SalesforceがSales Connectが{#check-if-salesforce-is-blocking-sales-connect-from-connecting}の接続からブロックしているかどうかを確認

1. Salesforce管理者にSFDCにログインしてもらいます。
1. 「**セットアップ**」を選択します。
1. 「**アプリを管理**」を選択します。
1. 「**Connected Apps OAuth Usage**」を選択します。
1. Sales Connectの横に「ブロック」と表示されていることを確認します。 「ブロック解除」が表示された場合は、ボタンをクリックして、Sales ConnectのSalesforceへのアクセスをブロック解除します。

