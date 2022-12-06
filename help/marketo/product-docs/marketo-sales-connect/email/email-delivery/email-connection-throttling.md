---
description: メール接続のスロットリング - Marketo ドキュメント - 製品ドキュメント
title: メール接続のスロットリング
exl-id: 093f5459-1bbb-45dd-8590-71ea4e1168d4
source-git-commit: ad7b222c2da937474565729a09a559fbcd722280
workflow-type: ht
source-wordcount: '394'
ht-degree: 100%

---

# メール接続のスロットリング {#email-connection-throttling}

Sales Connect アカウントを統合して、Exchange または Gmail のメールプロバイダーを通じて送信すると、1:1 のセールス通信のための合理化された設定とメール配信品質の最適化が可能です。ただし、システムの健全性とアカウントの安全性を維持するために、Gmail と Exchange ではメール送信の制限が実施されます。これらの制限は、プロバイダーの裁量によって増減することができます。

## 概要 {#overview}

メール接続のスロットリングを使用すると、Sales Connect 管理者は、Gmail または Exchange を配信チャネルとして使用する場合に、配信チャネルプロバイダーに引き渡されるメールの割合が強制的な制限を超えないように、メールの送信率を設定できます。

制限を継続的に超えると、配信チャネルプロバイダーが疑わしい動作と見なし、メール送信が失敗したり、アカウントが無効になったりする場合があります。

**メモ／ハイライト**

* ユーザが Gmail または Exchange に接続すると自動的に有効化されます
* ニーズに合わせてレコメンデーションの設定を増減する場合は、カスタマイズ可能です
* Gmail または Exchange を通じて送信されるメールのみスロットリングし、カスタム配信チャネルをスロットリングしません
* メール接続のスロットリングは、各ユーザがメールプロバイダーと独自に接続しているため、各ユーザのメールを個別にキューイングします

**メール接続のスロットリングの設定**

1. 歯車アイコンをクリックし、「**設定**」を選択します。

   ![](assets/email-connection-throttling-1.png)

1. 「**一般**」をクリックします。

   ![](assets/email-connection-throttling-2.png)

1. 「メール接続のスロットリング」カードで、メールチャネルプロバイダーに送信するメールのバッチサイズを入力します。

   ![](assets/email-connection-throttling-3.png)

1. 各バッチが送信されるまでの待機時間を設定します。この例では、45 秒ごとに 25 通のメールを選択します。

   ![](assets/email-connection-throttling-4.png)

1. 「**保存**」をクリックします。

   ![](assets/email-connection-throttling-5.png)

変更を保存すると、すべてのユーザは、接続された Gmail または Exchange アカウントに一括でメールを送信して配信できます。

## メールプロバイダーの制限 {#email-provider-limits}

**Outlook 365**

ビジネス／エンタープライズ

* 1 日あたり 10,000 件
* 1 分あたり 30 件
* 1 件のメールあたり 500 人の受信者

詳しくは[こちら](https://docs.microsoft.com/ja-jp/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#RecipientLimits)をご覧さい。

**Gmail**

* 1 日あたり 2,000 件（体験版およびフラグ付きアカウントの場合は 500 件）
* 1 秒あたり 2 件のメール（API の上限）
* 1 メッセージあたり 2,000 人（外部受信者の場合は最大 500 人）

詳しくは[こちら](https://support.google.com/a/answer/166852?hl=jp)をご覧さい。

**Microsoft Exchange Server（2010、2013）**

サーバーが組織でホストされるので、制限は組織の IT 部門によって設定されます。必要に応じて、ネットワーク管理者またはシステム管理者に問い合わせてください。

>[!MORELIKETHIS]
>
>* [配信チャネルの概要](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/delivery-channel-overview.md)
>* [Gmail ユーザのメール接続](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [Outlook ユーザのメール接続](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)

