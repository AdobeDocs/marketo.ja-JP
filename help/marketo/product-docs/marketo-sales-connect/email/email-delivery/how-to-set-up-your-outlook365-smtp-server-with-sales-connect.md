---
unique-page-id: 14352600
description: Outlook365 SMTPサーバーをSales Connect - Marketto Docs — 製品ドキュメントでセットアップする方法
title: Outlook365 SMTPサーバーをSales Connectで設定する方法
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---


# Outlook365 SMTPサーバーをSales Connectでセットアップする方法{#how-to-set-up-your-outlook-smtp-server-with-sales-connect}

>[!NOTE]
>
>Outlookを使用し、Marketo Sales Connectとの電子メール配信チャネルを設定しようとしている場合は、Exchangeサーバー[にEメール接続機能](http://docs.marketo.com/x/Z4AOAQ)を使用して接続することをお勧めします。

カスタムの[SMTP](http://docs.marketo.com/x/zYTS)サーバーを代替配信チャネルとして設定するために、ToutAppでは、セキュリティ上の理由から何らかの認証を使用する必要があります。 [SMTP設定ページ](http://toutapp.com/next#settings/email-servers/smtp/configure)には、任意のSMTPサーバーを設定できます。 Office365 SMTPサーバーをセットアップするには、次の構成をお勧めします。\
**SMTP Server**:smtp.office365.com\
**サーバーポート**:ポート587 — 保護\
**認証方法**:ログイン(SSL/TLS)\
**ユーザー名またはログイン**:Office365の電子メールアドレス\
**パスワード**:Office365電子メールパスワード\
**ドメイン**:会社のドメイン

SMTPサーバーのセットアップで問題が解決しない場合は、Exchange管理者に問い合わせて、適切な資格情報が使用されていることを確認してください。

>[!NOTE]
>
>Office365 SMTP経由で送信する場合、Microsoftは`limit of 30 messages sent per minute`を設け、1日10,000受信者に制限します。 また、Office365 SMTPサーバー経由で電子メールを送信するチームの`each member`は、Sales Connect設定で、独自の電子メールアドレスとパスワードを使用してこれを設定する必要があります。 MicrosoftのOffice365アカウントポリシーに従って、この構成の設定&quot; `Make this deliverability channel to all my team members` `" will not work`のボックスをチェックしています。

