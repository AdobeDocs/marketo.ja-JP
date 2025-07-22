---
description: 配信チャネルの概要 - Marketo ドキュメント - 製品ドキュメント
title: 配信チャネルの概要
exl-id: 8dd6fe3e-86ae-4361-bc0a-6488dc1df9fa
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '660'
ht-degree: 76%

---

# 配信チャネルの概要 {#delivery-channel-overview}

Marketo Sales には、メールを配信するための複数のオプションが用意されています。この記事では、活用できる配信チャネル、それらの選択方法、そのチャネルを選択するタイミングを確認します。

## 推奨：メール接続を介した Gmail または Exchange {#recommended-gmail-or-exchange-via-email-connection}

Marketo Sales を使用すると、メール接続サービスを通じて、合理的な設定および強化された到達率を実現できます。メール接続を使用すると、各ユーザーは [Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md) またはアカウントをMarketo Sales に接続し、すべてのMarketo Sales のメールの配信チャネルとして利用で [[!DNL Exchange]](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md) ます。

Gmail や [!DNL Exchange] を利用すると、他の配信チャネルオプションに比べて明らかなメリットが得られます。

* これは、定評のある配信チャネルなので、到達率を高く保つことができます。
* SPF や DKIM などの認証方法は、既に IT チームによって設定および管理されているので、追加の設定が必要ありません。
* 特定のメールネットワーク内でメールを送信（つまり、[!DNL Exchange] を通じてメールを受信する会社に [!DNL Exchange] ユーザーとしてメールを送信）すると、配信品質をさらに高めることができます。

これらの配信チャネルには、Microsoft や Google によって強制される独自の送信制限があることに注意する必要があります。この問題に対処するために、調整メカニズムを利用して、ユーザが制限内に収まるようにしています。メール調整について詳しくは、[こちら](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)を参照してください。

>[!NOTE]
>
>デフォルトでは、O365 プラグインは常に Exchange 配信チャネルを使用し、Gmail プラグインは常に Gmail 配信チャネルを利用して、プラグインからのメールを配信します。

**バウンストラッキング**：Marketo Sales は、送信者の受信トレイに送信されるバウンスメッセージを検出することで、Exchange Online または Gmail ユーザのバウンスを検出できます。これらのバウンス通知は、テンプレート分析、キャンペーン分析およびユーザへのライブフィード通知にまとめて表示されます。Exchange オンプレミスのお客様の場合、バウンストラッキングはサポートされていません。

## SMTP によるカスタム配信チャネル {#custom-delivery-channel-via-smtp}

Marketo Sales には、サードパーティの SMTP サーバーを接続して、セールスチームの希望する配信チャネルとして使用するオプションも用意されています。

サードパーティの SMTP プロバイダーを利用することは、メールのボリュームを最優先するセールスチームに適したオプションです。SendGrid や SparkPost などの SMTP プロバイダーは、一括メール配信のニーズに対応するように最適化されており、大量の電子メールを展開したいというニーズに合わせて拡張できます。

さらに、サードパーティの SMTP プロバイダーは、チームの配信ニーズ（メール配信レポートや専用 IP アドレスなど）をサポートするための様々な機能を提供しており、セールスメールの配信チャネルをより詳細にコントロールし、可視化したいと考えている方には最適な選択肢となります。

## Marketo Sales サーバー（レガシー） {#marketo-sales-servers-legacy}

Marketo Sales サーバーは、一部のレガシー ToutApp のお客様のみ使用できます。これらのお客様のメール設定には Marketo Sales サーバーが表示されます。従来のバージョン以外のお客様の場合、Marketo Sales が選択肢として表示されるわけではありません。Gmail または [!DNL Outlook] アカウントをMarketo Sales に接続して、配信チャネルのロックを解除する必要があります。

Marketo Sales サーバーは、DKIM および SPF 認証方式をサポートしていないので、到達率が低下する可能性があります。このため、最高の配信品質を得るには、すべてのお客様に Gmail または [!DNL Outlook] に接続することをお勧めします。

## MSC サーバー（レガシー） {#msc-servers-legacy}

MSC サーバーは、一部のレガシー ToutApp のお客様のみ使用できます。これらのお客様は、メール設定に MSC サーバーが表示されます。レガシー版以外のすべてのお客様には、MSC サーバーがオプションとして表示されないので、配信チャネルのロックを解除するには、Gmail や Outlook のアカウントを Sales Connect に接続する必要があります。

MSC サーバーは、DKIM および SPF 認証方式をサポートしていないので、到達率が低下する可能性があります。このため、最高の配信品質を得るには、すべてのお客様に Gmail または [!DNL Outlook] に接続することをお勧めします。

## Marketo サーバー {#marketo-servers}

Marketo のメールサーバーは、Marketo Sales と統合されていません。Marketo サーバーは、マーケターのニーズに合わせて拡張できるよう、一括配信に最適化されています。ただし、Gmail と [!DNL Exchange] は 1:1 のセールスコミュニケーションの成功率が高いため、これらのサーバーをセールスコミュニケーションに使用することをお勧めします。

>[!MORELIKETHIS]
>
>* [Gmail ユーザのメール接続](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [ ユーザー  [!DNL Outlook]  メール接続 ](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
>* [カスタム配信チャネルの設定](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/setting-up-a-custom-delivery-channel.md)
>* [メール接続のスロットリング](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)
