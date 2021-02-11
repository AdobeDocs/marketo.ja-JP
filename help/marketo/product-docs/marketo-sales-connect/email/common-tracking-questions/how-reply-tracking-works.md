---
unique-page-id: 14352482
description: 返信トラッキングの仕組み — Marketto Docs — 製品ドキュメント
title: 返信追跡の仕組み
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 0%

---


# 応答追跡の仕組み{#how-reply-tracking-works}

返信追跡は、送信するすべての電子メールに含まれるメッセージIDを調べることで行われます。 すべての電子メールには一意のメッセージIDが含まれており、このIDを使用して、最適な返信追跡をいくつか行うことができます。

>[!PREREQUISITES]
>
>**電子メールサーバーとの接続：** Sales Connectは、受信トレイに接続されている必要があります。これにより、新しい返信が届いた時点がわかります。Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-tab-for-gmail-users.md)に接続するSales Connectアカウント[が必要です。 Outlookを使用している場合は、[Exchangeサーバー](https://toutapp.com/next#settings/exchange_settings)と統合する必要があります。

Sales Connectが見込み客の電子メールへの返信を追跡できない場合、返信検出に基づくキャンペーンを停止したり、Salesforceに返信したログを記録したりすることはできません。  どの電子メールアドレスでも返信できるということですか。

つまり、flynn@flynnsarcade.comに電子メールを送信し、kevinf@flynnsarcade.comに返信した場合、返信を追跡できます。 さらに、flynn@flynnsarcade.comとCC alan@encom.comに電子メールを送信し、Alanが返信した場合は、返信を検出してキャンペーンを終了します。
