---
unique-page-id: 14352482
description: セールスコネクトでの返信追跡の仕組みを理解します。 返信が検出され、SalesforceまたはMarketoに記録される方法について説明します。
title: 返信トラッキングの動作方法
exl-id: 8d087014-99b7-47ba-9f08-95b13bc16438
feature: Marketo Sales Connect
source-git-commit: 240b78561db11e169188698880d4707a5c1f64de
workflow-type: tm+mt
source-wordcount: '179'
ht-degree: 62%

---

# 返信トラッキングの動作方法 {#how-reply-tracking-works}

返信トラッキングは、送信するすべてのメールに含まれるメッセージ ID を調べることで行われます。 すべてのメールには、最適な返信トラッキングに利用できる一意のメッセージ ID が含まれています。

>[!PREREQUISITES]
>
>**メールサーバーとの接続**：新しい返信が届いた日時を知るには、[!DNL Sales Connect] をインボックスに接続する必要があります。 [!DNL Sales Connect] アカウントを [Gmail に接続する](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)必要があります。 [!DNL Outlook]を使用している場合は、[exchange サーバー](https://toutapp.com/next#settings/exchange_settings)と統合する必要があります。

[!DNL Sales Connect] が送信メールに対する見込み客の返信をトラックできない場合、返信検出に基づくキャンペーンを停止したり、その返信を [!DNL Salesforce] に記録したりすることはできません。  どのメールアドレスでも返信できるとはどういう意味でしょうか？

つまり、<flynn@flynnsarcade.com>に電子メールを送信し、<kevinf@flynnsarcade.com>で返信した場合、返信を追跡できます。 さらに、<flynn@flynnsarcade.com>とCC <alan@encom.com>に電子メールを送信し、Alanが返信を書き込んだ場合、返信も検出され、キャンペーンが終了します。
