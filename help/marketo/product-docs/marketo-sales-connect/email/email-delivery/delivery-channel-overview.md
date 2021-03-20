---
unique-page-id: 14352407
description: 配信チャネルの概要 — Marketto Docs — 製品ドキュメント
title: 配信チャネルの概要
translation-type: tm+mt
source-git-commit: f3e3efc1cc480e9c6501b7e808f53c3a8bdc93d8
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 0%

---


# 配信チャネルの概要{#delivery-channel-overview}

Marketo Sales Connectには、電子メールを配信する複数のオプションが用意されています。 この記事では、活用できる配信チャネル、選択方法、および選択方法について説明します。

## 推奨：Eメール接続を介したGmailまたはExchange {#recommended-gmail-or-exchange-via-email-connection}

Sales Connectを使用すると、Email Connectionサービスを通じて、セットアップの合理化と配信品質の向上が可能です。 Email Connectionを使用すると、各ユーザは[Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)または[Exchange](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)アカウントに接続して、Sales ConnectのすべてのSales Connect電子メールの配信チャネルとして利用できます。

GmailまたはExchangeの利用には、他の配信チャネルオプションと比較して、いくつかの明確な利点があります。

* これは、信頼性が確立され、配信品質を高く保つための実証済みの配信チャネルです。
* SPFやDKIMなどの認証方法は、ITチームによって既に構成および管理されているので、追加の設定は必要ありません。
* 特定の電子メールネットワーク内で電子メールを送信する(Exchange経由で電子メールを受信する会社にExchangeユーザーとして電子メールを送信する)ことで、配信品質をさらに向上できます。

これらの配信チャネルには、MicrosoftやGoogleによって適用される送信制限が独自に設けられていることに注意してください。 この問題に対処するために、スロットリングメカニズムを利用して、ユーザーがその制限内にとどまるのを支援します。 [電子メールのスロットリングについて詳しくは、](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)を参照してください。

>[!NOTE]
>
>デフォルトでは、O365プラグインは常にexchange配信チャネルを使用し、Gmailプラグインは常にGmail配信チャネルを利用してプラグインからの電子メールを配信します。

**バウンスの追跡**:MSCでは、送信者の受信トレイに送信されるバウンスメッセージを検出することで、Exchange OnlineまたはGmailユーザーのバウンスを検出できます。これらのバウンス通知は、テンプレートの分析、キャンペーンの分析およびライブフィードの通知にロールアップされます。 バウンスの追跡は、Exchange On-Premのお客様にはサポートされていません。

## SMTP {#custom-delivery-channel-via-smtp}を介したカスタム配信チャネル

Sales Connectオファーは、サードパーティのSMTPサーバーを接続して、営業チームの優先配信チャネルとして使用する追加のオプションです。

サードパーティのSMTPプロバイダーの利用は、電子メールの量が最も優先度の高い営業チームにとって非常に優れた選択肢です。 SendgridやSparkpostなどのSMTPプロバイダーは、一括電子メール配信のニーズに対応するように最適化されており、大量の電子メールをデプロイしたいユーザーのニーズに合わせて拡張できます。

さらに、サードパーティのSMTPプロバイダは、チームの配信品質のニーズ(電子メール配信レポートや専用のIPアドレスなど)をサポートするために多数の機能をオファーしており、販売用電子メール配信チャネルに関するより詳細な制御と可視性を求めるお客様にとって優れた選択肢です。

## MSCサーバー（レガシー） {#msc-servers-legacy}

MSCサーバは、一部のレガシーToutAppのお客様でのみ使用できます。 該当するユーザーの電子メール設定にMSCサーバーが表示されます。 レガシーでないお客様の場合は、MSCを選択肢として認識しないため、GmailまたはOutlookのアカウントをSales Connectに接続して、配信チャネルのロックを解除する必要があります。

MSCサーバーは、DKIMおよびSPF認証方式をサポートしていないため、配信品質が低下する可能性があります。 このため、最高の配信品質を得るには、すべてのお客様にGmailまたはOutlookに接続することをお勧めします。

## マーケティング先サーバ{#marketo-servers}

Marketorの電子メールサーバーは、Sales Connectと統合できません。 マーケティングサーバーは、一括配信に最適化され、マーケターのニーズに合わせて拡張できます。 ただし、GmailとExchangeでは、1:1の販売コミュニケーションの成功率が高いので、販売コミュニケーションにこれらのサーバーを使用することをお勧めします。

>[!MORELIKETHIS]
>
>* [Gmailユーザーの電子メール接続](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [Outlookユーザー用電子メール接続](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
>* [カスタム配信チャネルの設定](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/setting-up-a-custom-delivery-channel.md)
>* [電子メール接続のスロットリング](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)

