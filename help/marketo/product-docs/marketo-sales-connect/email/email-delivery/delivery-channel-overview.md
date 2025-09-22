---
unique-page-id: 14352407
description: 配信チャネルの概要 - Marketo ドキュメント - 製品ドキュメント
title: 配信チャネルの概要
exl-id: 432bad1e-4eaf-4be8-b856-be364c44816e
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 100%

---

# 配信チャネルの概要 {#delivery-channel-overview}

Marketo [!DNL Sales Connect] には、メールを配信する複数のオプションが用意されています。この記事では、活用できる配信チャネル、それらの選択方法、そのチャネルを選択するタイミングを確認します。

## 推奨：メール接続を介した Gmail または [!DNL Exchange] {#recommended-gmail-or-exchange-via-email-connection}

[!DNL Sales Connect] を使用すると、メール接続サービスを通じて、合理的な設定および強化された配信品質を実現できます。[!UICONTROL メール接続]では、各ユーザの [Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md) または [Exchange](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md) アカウントを [!DNL Sales Connect] に接続し、すべての [!DNL Sales Connect] メールの配信チャネルとして利用できます。

Gmail または [!DNL Exchange] の利用には、他の配信チャネルオプションと比較して、いくつかの明確な利点があります。

* これは、定評のある配信チャネルなので、到達率を高く保つことができます。
* SPF や DKIM などの認証方法は、既に IT チームによって設定および管理されているので、追加の設定が必要ありません。
* 特定のメールネットワーク内でメールを送信すると（例：[!DNL Exchange] でメールを受信している企業に [!DNL Exchange] ユーザとしてメールを送信する）、配信品質をさらに高めることができます。

これらの配信チャネルには、Microsoft や Google によって強制される独自の送信制限があることに注意する必要があります。この問題に対処するために、調整メカニズムを利用して、ユーザが制限内に収まるようにしています。メール調整について詳しくは、[こちら](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)を参照してください。

>[!NOTE]
>
>デフォルトでは、O365 プラグインは常に Exchange 配信チャネルを使用し、Gmail プラグインは常に Gmail 配信チャネルを利用して、プラグインからのメールを配信します。

**バウンストラッキング**：MSC は、送信者のインボックスに送信されるバウンスメッセージを検出することで、[!DNL Exchange Online] または Gmail ユーザのバウンスを検出できます。これらのバウンス通知は、テンプレート分析、キャンペーン分析およびユーザへのライブフィード通知にまとめて表示されます。[!DNL Exchange] オンプレミスのお客様の場合、バウンストラッキングはサポートされていません。

## SMTP によるカスタム配信チャネル {#custom-delivery-channel-via-smtp}

[!DNL Sales Connect] には、サードパーティの SMTP サーバーを接続して、セールスチームの希望する配信チャネルとして使用するオプションも用意されています。

サードパーティの SMTP プロバイダーを利用することは、メールのボリュームを最優先するセールスチームに適したオプションです。[!DNL Sendgrid] や [!DNL Sparkpost] などの SMTP プロバイダーは、一括メール配信のニーズに対応するように最適化されており、大量のメールをデプロイするというニーズに合わせて拡張できます。

さらに、サードパーティの SMTP プロバイダーは、チームの配信ニーズ（メール配信レポートや専用 IP アドレスなど）をサポートするための様々な機能を提供しており、セールスメールの配信チャネルをより詳細にコントロールし、可視化したいと考えている方には最適な選択肢となります。

## MSC サーバー（レガシー） {#msc-servers-legacy}

MSC サーバーは、一部のレガシー ToutApp のお客様のみ使用できます。これらのお客様は、メール設定に MSC サーバーが表示されます。レガシー版以外のすべてのお客様には、MSC サーバーがオプションとして表示されないので、配信チャネルのロックを解除するには、Gmail や [!DNL Outlook] のアカウントを [!DNL Sales Connect] に接続する必要があります。

MSC サーバーは、DKIM および SPF 認証方式をサポートしていないので、配信品質が低下する可能性があります。このため、最高の配信品質を得るために、すべてのお客様に Gmail または [!DNL Outlook] に接続することをお勧めします。

## Marketo サーバー {#marketo-servers}

Marketo のメールサーバーは、[!DNL Sales Connect] と統合されていません。Marketo サーバーは、マーケターのニーズに合わせて拡張できるよう、一括配信に最適化されています。ただし、Gmail および [!DNL Exchange] は、1:1 のセールスコミュニケーションの成功率が高いので、セールスコミュニケーションにはこれらのサーバーを使用することをお勧めします。

>[!MORELIKETHIS]
>
>* [Gmail ユーザのメール接続](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [ [!DNL Outlook]  ユーザのメール接続](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
>* [カスタム配信チャネルの設定](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/setting-up-a-custom-delivery-channel.md)
>* [メール接続のスロットリング](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)
