---
unique-page-id: 14352482
description: 返信トラッキングの仕組み — Marketto Docs — 製品ドキュメント
title: 返信追跡の仕組み
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '243'
ht-degree: 0%

---


# 返信追跡の仕組み {#how-reply-tracking-works}

返信追跡は、送信するすべての電子メールに含まれるメッセージIDを調べることで行われます。 すべての電子メールには一意のメッセージIDが含まれており、このIDを使用して、最適な返信追跡をいくつか行うことができます。

>[!NOTE]
>
>**前提条件**
>
>**電子メールサーバーとの接続：** 新しい返信が届いた時点を知るには、Sales Connectを受信トレイに接続する必要があります。 Gmailに [接続するSales Connectアカウントが必要です](http://docs.marketo.com/x/kYMOAQ)。 Outlookを使用している場合は、 [Exchangeサーバーとの統合が必要です](http://toutapp.com/next#settings/exchange_settings)。

Sales Connectが見込み客の電子メールへの返信を追跡できない場合、返信検出に基づくキャンペーンを停止したり、Salesforceに返信したログを記録したりすることはできません。  どの電子メールアドレスでも返信できるということですか。

つまり、メールを送信し [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#783217162b16170f3830170d0b1d2b0c190a13561b1715) て返信を行った場合、返信を追跡でき [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#c08aafae93aeafb78094a8a58ea9a7a8b4b397a1b4a3a8eea3afad)ます。 さらに、メール [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#450f2a2b162b2a32050d2a303620163124372e6b262a28) とCC [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#3e5f525f507e5b505d5153105d5153)とAlanが返信すると、返信を検出してキャンペーンを終了します。
