---
unique-page-id: 11386358
description: Marketo Sandbox - Marketoドキュメント — 製品ドキュメント
title: Marketo Sandbox
exl-id: c040fac6-2290-4de5-b27d-2c7cb28f6e30
source-git-commit: 84a285974de3bbcdf33e24befae323d3d82ef239
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 7%

---

# Marketo Sandbox {#marketo-sandbox}

Marketoサンドボックスは、実稼動環境での実装前のテスト用に使用される追加のインスタンスです。

>[!AVAILABILITY]
>
>この機能を購入しているのは一部の顧客のみです。詳しくは、カスタマーサクセスマネージャーにお問い合わせください。

Marketoサンドボックスは、実稼動インスタンスと既に同期されている場合、通常の CRM と同期できません。 同期に CRM のサンドボックスを使用し、元の同期と同じ手順をすべて実行します。

## サンドボックスについて知っておくべきこと {#things-to-know-about-sandboxes}

* Customer Success Manager がサンドボックスを設定し、招待を送信したら、Marketo実稼動インスタンスとは別の電子メールアドレスを使用してログインする必要があります。
* ユーザーを追加する場合のプロセスは、実稼動環境で [ ユーザーを追加する ](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md#create-users) のプロセスと同じです。 既にMarketoログインをお持ちの場合は、別の電子メールアドレスを使用する必要があります。
* Marketoサンドボックスは空で始まりますが、実稼動インスタンスと同じ機能を使用できます。
* サンドボックスでプログラムを作成して実稼動環境に移動する場合は、[ プログラムのインポート ](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md) を実行できます。
* サンドボックスは調整されるので、実稼動インスタンスはテスト環境の悪影響を受けません。 1 回のキャンペーン実行で最大 20 個の E メールを送信できます。

>[!CAUTION]
>
>現在、Marketo Dynamics Sync のサンドボックス更新はサポートされていません。 Dynamics CRM サンドボックスを更新する必要がある場合は、新しいMarketoサンドボックスが必要です。 詳しくは、カスタマーサクセスマネージャーにお問い合わせください。

## インスタンスコピー {#instance-copy}

サポートケースを送信して、1 回限りのインスタンスコピーでサンドボックスに入力するようリクエストできます。 ただし、インスタンスコピーは _すべて_ を引き継ぎます。 詳しくは、[Marketoサポート ](https://nation.marketo.com/t5/Support/ct-p/Support) を参照してください。

>[!NOTE]
>
>* ソースインスタンスがMicrosoft Dynamics と統合されている場合、インスタンスコピーは **サポートされません**。
>* ネイティブ CRM を変更する場合は、新しいMarketoインスタンスが必要になり、新しいMarketoインスタンスにインスタンスをコピーすることはできません。 代わりに、 Marketoサポートと協力して、プログラムの読み込み機能を確認してください。

