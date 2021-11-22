---
unique-page-id: 11386358
description: Marketo サンドボックス - Marketo ドキュメント - 製品ドキュメント
title: Marketo サンドボックス
exl-id: c040fac6-2290-4de5-b27d-2c7cb28f6e30
source-git-commit: c2dc3c337cb5ea1446a2ebd6233f570025d1d986
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 100%

---

# Marketo サンドボックス {#marketo-sandbox}

Marketo サンドボックスは、実稼動環境で実装する前にテスト目的で使用される追加のインスタンスです。

>[!AVAILABILITY]
>
>すべての顧客がこの機能を購入したわけではありません。詳しくは、カスタマーサクセスマネージャーにお問い合わせください。

Marketo サンドボックスが既に実稼動インスタンスと同期されている場合、通常の CRM に同期することはできません。同期に CRM のサンドボックスを使用し、元の同期と同じ手順をすべて実行します。

## サンドボックスについて知っておくべきこと {#things-to-know-about-sandboxes}

* Customer Success Manager がサンドボックスを設定し、招待を送信したら、Marketo 実稼動インスタンスとは別のメールアドレスを使用してログインする必要があります。
* ユーザーを追加する場合のプロセスは、[実稼動環境にユーザーを追加する](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md#create-users)場合のプロセスと同じです。既に Marketo ログインを持っている場合は、別のメールアドレスを使用する必要があります。
* Marketo サンドボックスは空で始まりますが、実稼動インスタンスと同じ機能を使用できます。
* サンドボックスでプログラムを作成し、それを実稼動環境に移動する場合は、[プログラムの読み込み](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md)を実行できます。
* サンドボックスは調整されるので、実稼動インスタンスがテスト環境に悪影響を及ぼすことはありません。1 回のキャンペーン実行で最大 20 通のメールを送信できます。

>[!CAUTION]
>
>現在、Marketo Dynamics Sync のサンドボックス更新はサポートされていません。Dynamics CRM サンドボックスを更新する必要がある場合は、新しい Marketo サンドボックスが必要です。詳しくは、カスタマーサクセスマネージャーにお問い合わせください。

## インスタンスコピー {#instance-copy}

サポートケースを送信して、1 回限りのインスタンスコピーでサンドボックスに入力するようリクエストできます。ただし、インスタンスコピーは&#x200B;_すべて_&#x200B;を引き継ぐわけではありません。詳しくは、[Marketo サポート](https://nation.marketo.com/t5/Support/ct-p/Support)を参照してください。

>[!NOTE]
>
>ネイティブ CRM を変更する場合は、新しい Marketo インスタンスが必要になり、新しい Marketo インスタンスへのインスタンスコピーはできなくなります。代わりに、 Marketo サポートに問い合わせて、プログラムの読み込み機能を確認してください。
