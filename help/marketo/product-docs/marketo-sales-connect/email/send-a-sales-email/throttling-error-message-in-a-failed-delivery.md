---
unique-page-id: 14352604
description: 失敗した配信でのエラーメッセージのスロットリング — Marketto Docs — 製品ドキュメント
title: 失敗した配信でのエラーメッセージのスロットリング
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '121'
ht-degree: 0%

---


# 失敗した配信でのエラーメッセージのスロットリング {#throttling-error-message-in-a-failed-delivery}

自分のサーバー経由で送信する場合、同時に送信できる電子メールの数に制限があります。 Sales Connect経由で送信する場合、多数の電子メールを送信できますが、同時に送信しようとします。 したがって、サーバーで1分あたり100通の電子メールが送信できないことに気付いている場合は、 [Webアプリケーションを通じて一度に100通の電子メールを送信する必要があり](http://toutapp.com/login) ます。 そうしないと、電子メール配信プロバイダーによって制限されているので、電子メールが「失敗した配信」フォルダーに送られる可能性があります。
