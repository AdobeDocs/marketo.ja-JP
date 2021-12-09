---
description: 配信チャネルの概要 - Marketo ドキュメント - 製品ドキュメント
title: 配信チャネルの概要
hide: true
hidefromtoc: true
exl-id: 8dd6fe3e-86ae-4361-bc0a-6488dc1df9fa
source-git-commit: fda1bf51d4016a61c41be9acba4771db1797a552
workflow-type: tm+mt
source-wordcount: '668'
ht-degree: 73%

---

# 配信チャネルの概要 {#delivery-channel-overview}

Marketo Sales には、メールを配信するための複数のオプションが用意されています。この記事では、活用できる配信チャネル、それらの選択方法、そのチャネルを選択するタイミングを確認します。

## 推奨：メール接続を介した Gmail または Exchange {#recommended-gmail-or-exchange-via-email-connection}

Marketo Sales では、E メール接続サービスを通じて、合理化された設定と配信品質の向上が可能です。 メール接続を使用すると、各ユーザーは [Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md) または [Exchange](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md) Marketo Sales へのアカウント。Marketo Sales のすべての E メールの配信チャネルとして使用します。

Gmail または Exchange の利用には、他の配信チャネルオプションと比較して、いくつかの明確な利点があります。0

* これは、定評のある配信チャネルなので、到達率を高く保つことができます。
* SPF や DKIM などの認証方法は、既に IT チームによって設定および管理されているので、追加の設定が必要ありません。
* 特定のメールネットワーク内でメールを送信すると（例：Exchange でメールを受信している企業に Exchange ユーザーとしてメールを送信する）、到達率をさらに高めることができます。

これらの配信チャネルには、Microsoft や Google によって強制される独自の送信制限があることに注意する必要があります。この問題に対処するために、調整メカニズムを利用して、ユーザーが制限内に収まるようにしています。メール調整について詳しくは、[こちら](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)を参照してください。

>[!NOTE]
>
>デフォルトでは、O365 プラグインは常に Exchange 配信チャネルを使用し、Gmail プラグインは常に Gmail 配信チャネルを利用して、プラグインからのメールを配信します。

**バウンスの追跡**:Marketoセールスは、送信者の受信ボックスに送信されたバウンスメッセージを検出することで、Exchange Online または Gmail ユーザーのバウンスを検出できます。 これらのバウンス通知は、テンプレート分析、キャンペーン分析およびユーザーへのライブフィード通知にまとめて表示されます。Exchange オンプレミスのお客様の場合、バウンストラッキングはサポートされていません。

## SMTP によるカスタム配信チャネル {#custom-delivery-channel-via-smtp}

Marketo Sales には、サードパーティの SMTP サーバーを接続して、セールスチームの優先する配信チャネルとして使用する追加のオプションが用意されています。

サードパーティの SMTP プロバイダーを利用することは、メールのボリュームを最優先するセールスチームに適したオプションです。SendGrid や SparkPost などの SMTP プロバイダーは、一括メール配信のニーズに対応するように最適化されており、大量の電子メールを展開したいというニーズに合わせて拡張できます。

さらに、サードパーティの SMTP プロバイダーは、チームの配信ニーズ（メール配信レポートや専用 IP アドレスなど）をサポートするための様々な機能を提供しており、セールスメールの配信チャネルをより詳細にコントロールし、可視化したいと考えている方には最適な選択肢となります。

## Marketoセールスサーバー（レガシー） {#marketo-sales-servers-legacy}

Marketoセールスサーバーは、一部のレガシー ToutApp のお客様のみご利用いただけます。 これらのお客様の電子メール設定には、Marketo Sales サーバーが表示されます。 従来のお客様以外のお客様は、Marketo Sales をオプションとして見なされず、Gmail または Outlook アカウントをMarketo Sales に接続して、配信チャネルのロックを解除する必要があります。

Marketoセールスサーバーは、DKIM および SPF 認証方式をサポートしていないので、配信品質の割合が低下する可能性があります。 このため、最高の到達率を得るために、すべてのお客様に Gmail または Outlook に接続することをお勧めします。

## MSC サーバー（レガシー） {#msc-servers-legacy}

MSC サーバーは、一部のレガシー ToutApp のお客様のみ使用できます。これらのお客様は、メール設定に MSC サーバーが表示されます。レガシー版以外のすべてのお客様には、MSC サーバーがオプションとして表示されないので、配信チャネルのロックを解除するには、Gmail や Outlook のアカウントを Sales Connect に接続する必要があります。

MSC サーバーは、DKIM および SPF 認証方式をサポートしていないので、到達率が低下する可能性があります。このため、最高の到達率を得るために、すべてのお客様に Gmail または Outlook に接続することをお勧めします。

## Marketo サーバー {#marketo-servers}

Marketo E メールサーバーはMarketo Sales と統合されません。 Marketo サーバーは、マーケターのニーズに合わせて拡張できるよう、一括配信に最適化されています。ただし、Gmail および Exchange は、1 対 1 のセールスコミュニケーションの成功率が高いので、セールスコミュニケーションにはこれらのサーバーを使用することをお勧めします。

>[!MORELIKETHIS]
>
>* [Gmail ユーザーのメール接続](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [Outlook ユーザーのメール接続](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
>* [カスタム配信チャネルの設定](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/setting-up-a-custom-delivery-channel.md)
>* [メール接続の調整](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)

