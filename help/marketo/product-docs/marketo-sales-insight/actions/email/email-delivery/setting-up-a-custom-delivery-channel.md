---
description: カスタム配信チャネルの設定 — Marketoドキュメント — 製品ドキュメント
title: カスタム配信チャネルの設定
hide: true
hidefromtoc: true
source-git-commit: 55afdc537d0a5d0b6114f478c4dd2ded09c84e34
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 11%

---

# カスタム配信チャネルの設定 {#setting-up-a-custom-delivery-channel}

Marketo Sales Connect を使用すると、カスタム SMTP サーバーと統合して E メールを配信できます。 これは、Gmail や Exchange の配信チャネルから一括 E メールを送信しない場合に最適です。

ユーザーは、個々の使用に合わせてカスタム SMTP サーバーを設定するか、管理者は、インスタンス内のすべてのセールスコネクトユーザーで共有されるチーム SMTP を設定できます。

>[!NOTE]
>
>* SMTP サーバーの設定に加えて、 [メール ID を検証する必要があります](/help/marketo/product-docs/marketo-sales-connect/getting-started/email-settings/verify-your-email.md) 電子メールを送信する前に。
>* お使いの SMTP サーバーに適したサーバー資格情報を取得するには、IT チームまたは SMTP サーバーのベンダーと協力することをお勧めします。
>* SMTP サーバーの資格情報を使用して Gmail サーバーと Exchange サーバーに接続することはできません。 これらのプロバイダとの統合には、アドビのメール接続サービスを使用してください。


## カスタム SMTP {#custom-smtp}

1. にログインします。 [web アプリケーション](https://toutapp.com/login)をクリックし、右上の歯車アイコンをクリックして、「 」を選択します。 **設定**.

PICC

1. 「マイアカウント」で、「**メール設定**」をクリックします。

PICC

1. クリック **カスタム配信チャネル**.

PICC

1. SMTP サーバーの資格情報を入力し、 **接続**.

PICC

>[!NOTE]
>
>これが唯一の配信チャネルの場合、すべての E メール ID に自動的に割り当てられ、ここで完了です。 これが唯一の配信チャネルでない場合は、手順 5 に進んでください。

1. メール設定で、 **アドレスと署名**.

PICC

1. 配信チャネルを選択する E メール ID を見つけ、 **配信チャネルを選択**.

PICC

1. 配信品質カードで、 **編集**.

PICC

1. 「チャネル」ドロップダウンをクリックし、先ほど追加したカスタム配信チャネルを選択します。 「**保存**」をクリックします。

PICC

>[!NOTE]
>
>チーム管理者がチーム SMTP サーバーを設定すると、デフォルトのメール ID にのみ自動的に適用され、他のメール ID のオプションとして使用できます。

## チーム SMTP サーバー {#team-smtp-server}

>[!NOTE]
>
>**管理者権限が必要**

1. にログインします。 [web アプリケーション](https://toutapp.com/login)をクリックし、右上の歯車アイコンをクリックして、「 」を選択します。 **設定**.

PICC

1. 「管理設定」で、「**一般**」をクリックします。

PICC

1. クリック **チーム配信チャネル**.

PICC

1. SMTP サーバーの資格情報を入力し、 **接続**.

PICC

>[!NOTE]
>
>チーム SMTP サーバーは、すべてのチームメンバーのデフォルトのメール ID のデフォルトの配信チャネルになります。 さらに、他のすべての電子メール ID の配信チャネルオプションとして使用できます。

>[!MORELIKETHIS]
>
>* [Gmail ユーザーのメール接続](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [Outlook ユーザーのメール接続](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)

