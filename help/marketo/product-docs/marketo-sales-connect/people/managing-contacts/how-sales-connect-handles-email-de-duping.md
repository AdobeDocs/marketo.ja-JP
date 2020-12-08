---
unique-page-id: 14352514
description: Sales Connectが電子メールの重複排除をどのように扱うか — Marketto Docs — 製品ドキュメント
title: Sales Connectが電子メールの重複排除をどのように処理するか
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '104'
ht-degree: 0%

---


# Sales Connectが電子メールの重複排除をどのように処理するか {#how-sales-connect-handles-email-de-duping}

CSV [ファイルをSales Connectに](http://docs.marketo.com/x/VADb) アップロードする場合、インポートが行われる前に、CSV内の「いいね！」の連絡先すべてを結合します。

同様の電子メールアドレスに基づいて行います。 同じ電子メールアドレスが2つある場合は、それらを1人の連絡先に結合します。

後で同じ連絡先を手動で追加/アップロードしようとした場合、この連絡先は結合されません。

データベースに既に存在する連絡先を追加しようとすると、その連絡先を追加できなくなります。

