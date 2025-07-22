---
unique-page-id: 14352546
description: セカンダリの Gmail アドレスと Sales Connect の統合の防止 - Marketo ドキュメント - 製品ドキュメント
title: セカンダリの Gmail アドレスと Sales Connect の統合の防止
exl-id: a84fe53b-0ec8-400c-8747-be496c68a8e3
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 56%

---

# セカンダリGmail アドレスと [!DNL Sales Connect] の統合の防止 {#preventing-secondary-gmail-address-from-integrating-with-sales-connect}

## Gmail 統合の破損（個人用 Gmail がメールを送信する理由） {#broken-gmail-integration-why-is-my-personal-gmail-sending-emails}

Gmail 接続が切断される最も一般的な理由は、ユーザーの個人アカウントとの間の偶発的な統合です。これは、ユーザーが「接続」をクリックした場合や、自分の個人アカウントからメールを送信しようとした場合に発生する可能性があります。これは、[!DNL Chrome] の同じインスタンスで Gmail アカウントにアクセスする際に仕事用メールと同じオプションが存在するので、非常に魅力的です。

## なぜ [!DNL Sales Connect] は私の個人的な Gmail と統合しようとしているのですか？ {#why-does-sales-connect-even-try-to-integrate-with-my-personal-gmail}

[!DNL Sales Connect] は、[!DNL Chrome] ブラウザーにインストールされている拡張機能を通じて Gmail と統合されます。 拡張機能で Gmail の開いたインスタンスが検出されるたびに、そのインスタンスと統合するオプションを提供します。個人の Gmail アカウントとの統合を防ぐには、次の 3 つのうちいずれかをお勧めします。

別のユーザーとしてサインイン [!DNL Chrome] 推奨）

別の [ プロファイル ](https://support.google.com/chrome/answer/2364824?hl=ja) の作成方法を参照するには、[!DNL Chrome] このリンク」をクリックします。

**長所**：別のユーザーとしてログインすると、[!DNL Chrome] の新しいインスタンスが開きます。 このインスタンスは [!DNL Chrome] の新しいウィンドウであり、古い拡張機能はこのウィンドウには存在しません。 また、Cookie を保持するので、毎回 Gmail にログインする必要がなくなります。

**短所**:[!DNL Chrome] の 2 つのウィンドウを開く必要があります。

別のブラウザーを使用する

**長所**：拡張機能がインストールされていない別のインターネットブラウザー（IE または Firefox）を使用すると、この問題が発生しません。

**短所**：複数のブラウザーを使用すると面倒な場合があります。

匿名ウィンドウを使用する

**長所：** 匿名ウィンドウは、[!DNL Chrome] の裸のバージョンを開くようなものです。 つまり、拡張機能はインストールされず、接続する [!DNL Sales Connect] ともありません。

**短所**：一日の作業を開始するたびに Gmail にサインインする必要があります。誤ってウィンドウを閉じた場合は、もう一度ログインする必要があります。
