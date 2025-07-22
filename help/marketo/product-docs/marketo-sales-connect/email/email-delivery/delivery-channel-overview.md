---
unique-page-id: 14352407
description: 配信チャネルの概要 - Marketo ドキュメント - 製品ドキュメント
title: 配信チャネルの概要
exl-id: 432bad1e-4eaf-4be8-b856-be364c44816e
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 55%

---

# 配信チャネルの概要 {#delivery-channel-overview}

Marketo [!DNL Sales Connect] には、メールを配信するための複数のオプションが用意されています。 この記事では、活用できる配信チャネル、それらの選択方法、そのチャネルを選択するタイミングを確認します。

## 推奨：メール接続による Gmail または [!DNL Exchange] {#recommended-gmail-or-exchange-via-email-connection}

[!DNL Sales Connect] れにより、メール接続サービスを通じて、設定を合理化し、配信品質を向上させることができます。 [!UICONTROL  メール接続 ] を使用すると、各ユーザーは [Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md) または [Exchange](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md) アカウントに接続し、すべてのメールの配信チャネル [!DNL Sales Connect] して利用で [!DNL Sales Connect] ます。

Gmail や [!DNL Exchange] を利用すると、他の配信チャネルオプションに比べて明らかなメリットが得られます。

* これは、定評のある配信チャネルなので、到達率を高く保つことができます。
* SPF や DKIM などの認証方法は、既に IT チームによって設定および管理されているので、追加の設定が必要ありません。
* 特定のメールネットワーク内でメールを送信（つまり、[!DNL Exchange] を通じてメールを受信する会社に [!DNL Exchange] ユーザーとしてメールを送信）すると、配信品質をさらに高めることができます。

これらの配信チャネルには、Microsoft や Google によって強制される独自の送信制限があることに注意する必要があります。この問題に対処するために、調整メカニズムを利用して、ユーザが制限内に収まるようにしています。メール調整について詳しくは、[こちら](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)を参照してください。

>[!NOTE]
>
>デフォルトでは、O365 プラグインは常に Exchange 配信チャネルを使用し、Gmail プラグインは常に Gmail 配信チャネルを利用して、プラグインからのメールを配信します。

**バウンストラッキング**:MSC は、送信者の受信ボックスに送信されるバウンスメッセージを検出することで、[!DNL Exchange Online] または Gmail ユーザーのバウンスを検出できます。 これらのバウンス通知は、テンプレート分析、キャンペーン分析およびユーザへのライブフィード通知にまとめて表示されます。バウンスのトラッキングは、オンプレミスのお客様 [!DNL Exchange] はサポートされていません。

## SMTP によるカスタム配信チャネル {#custom-delivery-channel-via-smtp}

[!DNL Sales Connect] では、セールスチームの優先配信チャネルとして使用するサードパーティの SMTP サーバーに接続する追加オプションを提供しています。

サードパーティの SMTP プロバイダーを利用することは、メールのボリュームを最優先するセールスチームに適したオプションです。[!DNL Sendgrid] や [!DNL Sparkpost] などの SMTP プロバイダーは、一括メール配信のニーズに対応するように最適化されており、大量のメールをデプロイしようとするユーザーのニーズに応じて拡張できます。

さらに、サードパーティの SMTP プロバイダーは、チームの配信ニーズ（メール配信レポートや専用 IP アドレスなど）をサポートするための様々な機能を提供しており、セールスメールの配信チャネルをより詳細にコントロールし、可視化したいと考えている方には最適な選択肢となります。

## MSC サーバー（レガシー） {#msc-servers-legacy}

MSC サーバーは、一部のレガシー ToutApp のお客様のみ使用できます。これらのお客様は、メール設定に MSC サーバーが表示されます。レガシー以外のお客様は、MSC をオプションとして見ることはできません。また、Gmail または [!DNL Outlook] アカウントを [!DNL Sales Connect] に接続して、配信チャネルのロックを解除する必要があります。

MSC サーバーは、DKIM および SPF 認証方式をサポートしていないので、到達率が低下する可能性があります。このため、最高の配信品質を得るには、すべてのお客様に Gmail または [!DNL Outlook] に接続することをお勧めします。

## Marketo サーバー {#marketo-servers}

Marketo メールサーバーは [!DNL Sales Connect] と統合されません。 Marketo サーバーは、マーケターのニーズに合わせて拡張できるよう、一括配信に最適化されています。ただし、Gmail と [!DNL Exchange] は 1:1 のセールスコミュニケーションの成功率が高いため、これらのサーバーをセールスコミュニケーションに使用することをお勧めします。

>[!MORELIKETHIS]
>
>* [Gmail ユーザのメール接続](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [ ユーザー  [!DNL Outlook]  メール接続 ](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
>* [カスタム配信チャネルの設定](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/setting-up-a-custom-delivery-channel.md)
>* [メール接続のスロットリング](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)
