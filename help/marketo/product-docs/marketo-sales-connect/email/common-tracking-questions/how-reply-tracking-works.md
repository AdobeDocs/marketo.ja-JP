---
unique-page-id: 14352482
description: 返信トラッキングの動作方法 - Marketo ドキュメント - 製品ドキュメント
title: 返信トラッキングの動作方法
exl-id: 8d087014-99b7-47ba-9f08-95b13bc16438
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '180'
ht-degree: 100%

---

# 返信トラッキングの動作方法 {#how-reply-tracking-works}

返信トラッキングは、送信するすべてのメールに含まれるメッセージ ID を調べることで行われます。すべてのメールには、最適な返信トラッキングに利用できる一意のメッセージ ID が含まれています。

>[!PREREQUISITES]
>
>**メールサーバーとの接続：**&#x200B;新しい返信が届いた日時を知るには、Sales Connect を受信ボックスに接続する必要があります。Sales Connect アカウントを [Gmail に接続する](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)必要があります。Outlook を使用している場合は、[Exchange サーバー](https://toutapp.com/next#settings/exchange_settings)と統合する必要があります。

Sales Connect が、送信メールに対する見込み客の返信をトラックできない場合、返信検出に基づくキャンペーンを停止したり、その返信を Salesforce に記録したりすることはできません。どのメールアドレスでも返信できるとはどういう意味でしょうか？

つまり、flynn@flynnsarcade.com にメールを送信し、kevinf@flynnsarcade.com で返信しても、返信をトラックできます。さらに、flynn@flynnsarcade.com と CC alan@encom.com にメールを送信し、Alan が返信すると、同様に返信が検出され、キャンペーンが終了します。
