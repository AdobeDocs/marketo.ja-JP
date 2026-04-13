---
unique-page-id: 11386358
description: 本番稼働前にテストするためのMarketo Engage サンドボックスについて説明します。 サンドボックスインスタンスを使用して、本番環境に影響を与えることなくテストを実施できます。
title: Marketo サンドボックス
exl-id: c040fac6-2290-4de5-b27d-2c7cb28f6e30
source-git-commit: b78d943f59628b0885118f56e0875fd43217da35
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 83%

---

# Marketo サンドボックス {#marketo-sandbox}

Marketo Engage サンドボックスは、本番環境で実装する前にテスト目的で使用される追加のインスタンスです。

>[!AVAILABILITY]
>
>必ずしもすべてのお客様がこの機能を購入済みとは限りません。詳しくは、アドビのアカウントチーム（担当のアカウントマネージャー）にお問い合わせください。

Marketo サンドボックスが既に本番稼働インスタンスと同期されている場合、通常の CRM に同期することはできません。同期に CRM のサンドボックスを使用し、元の同期と同じ手順をすべて実行します。

## サンドボックスについて知っておくべきこと {#things-to-know-about-sandboxes}

* ユーザーを追加する場合のプロセスは、[本番環境にユーザーを追加する](/help/marketo/product-docs/administration/users-and-roles/add-or-remove-a-user#add-a-user)場合のプロセスと同じです。既に Marketo ログインを持っている場合は、別のメールアドレスを使用する必要があります。
* Marketo サンドボックスは空で始まりますが、本番稼働インスタンスと同じ機能を使用できます。
* サンドボックスでプログラムを作成し、それを本番環境に移動する場合は、[プログラムの読み込み](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md)を実行できます。
* サンドボックスは調整されるので、本番稼働インスタンスがテスト環境に悪影響を及ぼすことはありません。1 回のキャンペーン実行で最大 20 通のメールを送信できます。

>[!CAUTION]
>
>現時点では、Marketo Dynamics _または_ Salesforce Syncのサンドボックス更新はサポートされていません。 CRM サンドボックスを更新する必要がある場合は、新しいMarketo サンドボックスが必要です。 詳しくは、アドビのアカウントチーム（担当のアカウントマネージャー）にお問い合わせください。

## インスタンスコピー {#instance-copy}

サポートケースを送信して、1 回限りのインスタンスコピーでサンドボックスに入力するようリクエストできます。ただし、インスタンスコピーは&#x200B;_すべて_&#x200B;を引き継ぐわけではありません。詳しくは、[Marketo サポート](https://nation.marketo.com/t5/Support/ct-p/Support)を参照してください。

>[!NOTE]
>
>ネイティブ CRM を変更する場合は、新しい Marketo インスタンスが必要になり、新しい Marketo インスタンスへのインスタンスコピーはできなくなります。代わりに、 Marketo サポートに問い合わせて、プログラムの読み込み機能を確認してください。
