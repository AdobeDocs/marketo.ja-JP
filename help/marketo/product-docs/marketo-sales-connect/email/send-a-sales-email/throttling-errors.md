---
unique-page-id: 14352581
description: エラーのスロットリング — Marketto Docs — 製品ドキュメント
title: エラーの制限
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '163'
ht-degree: 0%

---


# エラーの制限 {#throttling-errors}

## ファイル制限に達しました {#file-limit-reached}

自分のサーバー経由で送信する場合、同時に送信できる電子メールの数に制限があります。 Sales Connect経由で送信する場合、多数の電子メールを送信できますが、すべて同時に送信しようとします。 したがって、サーバーで1分あたり100通の電子メールが送信できなくなることを知っている場合は、 [Webアプリケーションを通じて最大100通の電子メールを送信する必要があります](http://toutapp.com/login)。 それ以外の場合は、サーバーで電子メールの制限が行われているため、電子メールが送信される可能性があります。

## 認証エラー {#authentication-error}

これは、SMTPサーバーへの接続を認証できなかったことを意味します。 おそらく、パスワードが最近変更されたので、新しい資格情報を認証するだけで済みます。

これを行うには、「 [SMTP設定」に移動します](http://docs.marketo.com/display/docs/assets/external-link-1.jspa) `where you should see the same error message. Update your credentials and hit **Authenticate and Save** to see a confirmation message.`

[失敗した配信]に移動して、これらの電子メールの再送信を試みます。
