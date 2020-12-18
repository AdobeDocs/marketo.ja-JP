---
unique-page-id: 14352407
description: 配信チャネルの概要 — Marketto Docs — 製品ドキュメント
title: 配信チャネルの概要
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---


# 配信チャネルの概要{#delivery-channel-overview}

活用できる3つのチャネル、選択方法、重ね合わせるタイミング、微妙な違いを分類します。

>[!NOTE]
>
>この情報は、[Webアプリケーション](http://toutapp.com/login)からの電子メールを送信する場合にのみ有効です。 GmailまたはOutlookでSales Connectを使用している場合は、これらの電子メールサーバー経由で電子メールが配信されます。

## MSC電子メールサーバー（デフォルト） {#msc-email-servers-default}

デフォルトでは、電子メールの配信に対してこの方法が選択されます。 MSC電子メールサーバーは、GmailやOutlookを使用しないユーザーにとって優れたオプションです。 また、これらはアドビのサーバーなので、バウンスや失敗した配信に関するエラーメッセージを取得し、「会話」タブの「失敗した配信」セクションでユーザーに表示する機能もあります。

MSCサーバーを使用するもう1つの利点は、[電子メールID](https://help.toutapp.com/hc/en-us/articles/215371427)を使用する場合に、作成したIDの電子メールアドレスが受信者に表示されることです。

MSCサーバーを使用している場合、受信者に「via toutapp.com」タグが表示されることがあります。 これは、Sales Connectを使用して送信された電子メールを知らせる電子メールクライアントです。

詳しくは、[Gmailヘルプ記事](https://support.google.com/mail/answer/1311182?hl=en)を参照してください。

>[!NOTE]
>
>MSCサーバーには、使用可能な[DMARCレコード](https://dmarc.org/)がありません。 独自のサーバーでホワイトリストに登録することはできません。

## Gmailサーバー{#gmail-server}

会社の電子メールプロバイダーがGmailの場合は、既存のアカウントを利用して、Sales Connectの電子メールを送信できます。 「via toutapp.com」情報を避けたい場合や、会社のドメインの評判と配信品質を信頼したい場合は、これは非常に良い選択です。 Gmailサーバーを使用する利点の1つは、Webアプリケーションから送信する内容はすべてGmail送信フォルダーに自動的に追加されるという点です。

Sales Connectの電子メールを配信する1つのGmailアカウント（1つの電子メールアドレス）に対してのみ、適切に接続できます。 つまり、複数の電子メールIDを使用する場合、詳細を確認する際には、接続しているアカウントのアドレスのみが表示されます。

Webアプリケーションでは、IDは上記で作成したとおりに表示されます。 ただし、Gmailサーバーを経由して送信すると、接続されているアカウントのアドレスが表示されます。

>[!NOTE]
>
>Sales ConnectはGmailサーバーを直接管理しないので、バウンスした電子メールイベントはWebアプリケーションに記録しません。

## カスタムSMTPサーバー{#custom-smtp-server}

自分のサーバの代金を払う？ Microsoft Exchange環境を使用する これは、お客様にとってのオプションです。 [設定の際には、](http://docs.marketo.com/x/zYTS)これらの説明を調べてください。 Gmailサーバーと同様、Sales Connectはサーバーを直接管理しないので、バウンスした電子メールイベントをWebアプリケーションに記録しません。

