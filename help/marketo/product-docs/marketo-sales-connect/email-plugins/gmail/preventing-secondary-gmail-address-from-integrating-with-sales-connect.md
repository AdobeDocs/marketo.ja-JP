---
unique-page-id: 14352546
description: GmailアドレスセカンダリがSales Connectと統合できない原因 — Marketto Docs — 製品ドキュメント
title: GmailアドレスがSales Connectと統合されるのセカンダリを防ぐ
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---


# GmailアドレスセカンダリとSales Connectとの統合を禁止する{#preventing-secondary-gmail-address-from-integrating-with-sales-connect}

## Gmail統合の破損（個人のGmailがメールを送信する理由） {#broken-gmail-integration-why-is-my-personal-gmail-sending-emails}

Gmail接続が切断される最も一般的な理由は、ユーザーの個人アカウントとの間の偶然の統合です。 これは、ユーザーが「接続」をクリックした場合や、個人アカウントから電子メールを送信しようとした場合に発生する可能性があります。 これは、Chromeの同じインスタンスでGmailアカウントにアクセスする場合に、勤務先の電子メールと同じインスタンスにこのオプションが存在するので、非常に魅力的です。

## Sales Connectが私の個人Gmailとの統合を試みる理由は何ですか。{#why-does-sales-connect-even-try-to-integrate-with-my-personal-gmail}

Sales Connectは、Chromeブラウザーにインストールされた拡張機能を通じてGmailと統合されます。 拡張部は、Gmailが開いているというインスタンスを検出するたびに、Gmailと統合するオプションをオファーします。 個人のGmailアカウントとの統合を防ぐため、3つのいずれかをお勧めします。

別のChromeユーザーとしてサインイン（推奨）

[このリンク](http://support.google.com/chrome/answer/2364824?hl=en)をクリックして、別のChromeプロファイルの作成方法を参照してください。

**長所**:別のユーザーとしてサインインすると、Chromeの新しいインスタンスが開きます。このインスタンスはChromeの新しいウィンドウです。このウィンドウには、古い拡張機能は1つも存在しません。 また、Gmailに毎回サインインする必要がないように、Cookieも保持されます。

**短所**:2つのChromeウィンドウを開いている必要があります。

別のブラウザーを使用

**長所：拡張機能がインストールされていない別のインターネットブラウザー（IEまたはFirefox）を** 使用すると、この問題は発生しません。

**短所**:複数のブラウザーを使用すると迷惑な場合があります。

匿名のウィンドウを使う

**長所：匿名** のウィンドウは、Chromeの裸版を開くようなものです。つまり、拡張機能がインストールされず、Sales Connectが接続できなくなります。

**短所**:1日の開始を行うたびに、Gmailにサインインする必要があります。誤ってウィンドウを閉じた場合は、再度サインインする必要があります。
