---
unique-page-id: 14352546
description: セカンダリ Gmail アドレスがSales Connectと統合されないようにする方法について説明します。 プラグインにはプライマリメールのみを使用してください。
title: セカンダリの Gmail アドレスと Sales Connect の統合の防止
exl-id: a84fe53b-0ec8-400c-8747-be496c68a8e3
feature: Marketo Sales Connect
TQID: https://experienceleague.adobe.com/rOA-dhKUDpXxEJ9dAna3wk05XaiB-UJKRrSaDJofnds
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 323
ht-degree: 93%

---

# セカンダリの Gmail アドレスと [!DNL Sales Connect] の統合の防止 {#preventing-secondary-gmail-address-from-integrating-with-sales-connect}

## Gmail 統合の破損（個人用 Gmail がメールを送信する理由） {#broken-gmail-integration-why-is-my-personal-gmail-sending-emails}

Gmail 接続が切断される最も一般的な理由は、ユーザーの個人アカウントとの間の偶発的な統合です。 これは、ユーザーが「接続」をクリックした場合や、自分の個人アカウントからメールを送信しようとした場合に発生する可能性があります。 これは、作業用メールと同じ [!DNL Chrome] インスタンスで Gmail アカウントにアクセスする際に、このオプションが存在するので、ついそうしてしまいがちです。

## [!DNL Sales Connect] は、なぜ個人用の Gmail との統合を試みるのでしょうか？ {#why-does-sales-connect-even-try-to-integrate-with-my-personal-gmail}

[!DNL Sales Connect] は、[!DNL Chrome] ブラウザーにインストールされた拡張機能を通じて Gmail と統合されます。 拡張機能で Gmail の開いたインスタンスが検出されるたびに、そのインスタンスと統合するオプションを提供します。 個人の Gmail アカウントとの統合を防ぐには、次の 3 つのうちいずれかをお勧めします。

別の [!DNL Chrome] ユーザとしてログインする（推奨）

[このリンク](https://support.google.com/chrome/answer/2364824?hl=ja)をクリックして、別の [!DNL Chrome] プロファイルの作成方法を読みます。

**長所**：別のユーザとしてログインすると、[!DNL Chrome] の新しいインスタンスが開きます。 このインスタンスは [!DNL Chrome] の新しいウィンドウで、古い拡張機能はこのウィンドウには存在しません。 また、cookie を保持するので、毎回 Gmail にログインする必要がなくなります。

**短所**：[!DNL Chrome] のウィンドウを 2 つ開く必要があります。

別のブラウザーを使用する

**長所**：拡張機能がインストールされていない別のインターネットブラウザー（IE または Firefox）を使用すると、この問題が発生しません。

**短所**：複数のブラウザーを使用すると面倒な場合があります。

匿名ウィンドウを使用する

**長所**：匿名ウィンドウは、何も設定されていない [!DNL Chrome] を開くようなものです。 つまり、拡張機能はインストールされず、[!DNL Sales Connect] は接続できません。

**短所**：その日の作業を開始するたびに Gmail にログインする必要があります。誤ってウィンドウを閉じた場合は、もう一度ログインする必要があります。
