---
unique-page-id: 14352482
description: 返信トラッキングの動作方法 - Marketo ドキュメント - 製品ドキュメント
title: 返信トラッキングの動作方法
exl-id: 8d087014-99b7-47ba-9f08-95b13bc16438
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '163'
ht-degree: 77%

---

# 返信トラッキングの動作方法 {#how-reply-tracking-works}

返信トラッキングは、送信するすべてのメールに含まれるメッセージ ID を調べることで行われます。すべてのメールには、最適な返信トラッキングに利用できる一意のメッセージ ID が含まれています。

>[!PREREQUISITES]
>
>**メールサーバーとの接続**：新しい返信が届いた日時を知るには、[!DNL Sales Connect] をインボックスに接続する必要があります。[!DNL Sales Connect] アカウントを [Gmail に接続する](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)必要があります。[!DNL Outlook] を使用している場合は、[Exchange サーバー](https://toutapp.com/next#settings/exchange_settings)と統合する必要があります。

[!DNL Sales Connect] が送信メールに対する見込み客の返信をトラックできない場合、返信検出に基づくキャンペーンを停止したり、その返信を [!DNL Salesforce] に記録したりすることはできません。どのメールアドレスでも返信できるとはどういう意味でしょうか？

つまり、<flynn@flynnsarcade.com> にメールを送信し、そのユーザーが <kevinf@flynnsarcade.com> を使用して応答すると、返信を追跡できます。 さらに、<flynn@flynnsarcade.com> と CC <alan@encom.com> にメールを送信し、Alan が返信すると、返信を検出してキャンペーンも終了します。
