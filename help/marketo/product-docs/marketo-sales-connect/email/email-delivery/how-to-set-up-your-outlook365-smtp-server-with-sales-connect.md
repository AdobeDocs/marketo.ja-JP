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


# Outlook365 SMTPサーバーをSales Connectで設定する方法 {#how-to-set-up-your-outlook-smtp-server-with-sales-connect}

>[!NOTE]
>
>Outlookを使用していて、Marketo Sales Connectとの電子メール配信チャネルを設定しようとしている場合は、電子メール接続機能を [使用してExchangeサーバーに接続することをお勧めします](http://docs.marketo.com/x/Z4AOAQ)。

カスタムの [SMTP](http://docs.marketo.com/x/zYTS) サーバを代替配信チャネルとして設定するために、ToutAppでは、セキュリティを確保するために何らかの認証を使用する必要があります。 SMTP設定ページでは、任意の [SMTPサーバーを設定できます](http://toutapp.com/next#settings/email-servers/smtp/configure)。 Office365 SMTPサーバーをセットアップするには、次の構成をお勧めします。\
**SMTP Server**:smtp.office365.com\
**サーバーポート**:ポート587 — 保護\
**認証方法**:ログイン(SSL/TLS)\
**ユーザー名またはログイン**:Office365の電子メールアドレス\
**パスワード**:Office365電子メールパスワード\
**ドメイン**:会社のドメイン

SMTPサーバーのセットアップで問題が解決しない場合は、Exchange管理者に問い合わせて、適切な資格情報が使用されていることを確認してください。

>[!NOTE]
>
>Office365 SMTP経由で送信する場合、Microsoftは1日10,000個の受信者 `limit of 30 messages sent per minute`に制限を設けます。 さらに、Office365 SMTPサーバー `each member` 経由で電子メールを送信するチームの中で、Sales Connectの設定で独自の電子メールアドレスとパスワードを設定する必要があります。 MicrosoftのOffice365アカウントポリシーに従って、この構成 `Make this deliverability channel to all my team members``" will not work` の設定&quot;のボックスをチェックしています。

