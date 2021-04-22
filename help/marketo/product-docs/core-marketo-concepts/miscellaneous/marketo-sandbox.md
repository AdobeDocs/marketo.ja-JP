---
unique-page-id: 11386358
description: Marketoサンドボックス —Marketoドキュメント — 製品ドキュメント
title: Marketo砂場
exl-id: c040fac6-2290-4de5-b27d-2c7cb28f6e30
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---

# Marketoサンドボックス{#marketo-sandbox}

Marketoサンドボックスは、実稼働環境に実装する前にテストを行う目的で使用される追加のインスタンスです。

>[!AVAILABILITY]
>
>この機能を購入した顧客はいません。 詳しくは、カスタマーサクセスマネージャーにお問い合わせください。

Marketoサンドボックスは、既に実稼働インスタンスと同期されている場合、通常のCRMと同期できません。 CRMのサンドボックスを同期に使用し、元の同期と同じ手順に従います。

## サンドボックスに関する知識{#things-to-know-about-sandboxes}

* Customer Success ManagerがSandboxを設定し、招待を送信したら、実稼働インスタンスとは異なる電子メールアドレスを使用してログインする必要があります。
* ユーザーを追加する場合の処理は、[実稼動環境](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md#create-users)にユーザーを追加するのと同じです。 また、既にMarketoログインをお持ちの場合は、別の電子メールアドレスを使用する必要があります。
* Marketoサンドボックスは空の開始を出しますが、実稼働インスタンスと同じ機能を使用できます。
* サンドボックス内にプログラムを作成し、実稼働環境に移動する場合は、[プログラムインポート](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md)を実行できます。
* サンドボックスは制限されるので、実稼働インスタンスがテスト環境の悪影響を受けません。 1回のキャンペーンで最大30件の電子メールを送信できます。

>[!CAUTION]
>
>現在、Marketoダイナミクス同期のサンドボックス更新をサポートしていません。 Dynamics CRMサンドボックスを更新する必要がある場合は、新しいMarketoサンドボックスが必要です。 詳しくは、カスタマーサクセスマネージャーにお問い合わせください。

## インスタンスコピー{#instance-copy}

サポートケースを送信して、1回限りのインスタンスコピーをサンドボックスに入力するように要請することができます。 ただし、インスタンスコピーは、_すべて_&#x200B;を引き継ぐわけではありません。 詳しくは、[Marketoサポート](https://nation.marketo.com/t5/Support/ct-p/Support)にお問い合わせください。

>[!NOTE]
>
>* ソースインスタンスがMicrosoft Dynamicsと統合されている場合、インスタンスコピーは&#x200B;****&#x200B;サポートされていません。
>* ネイティブのCRMを変更する場合は、新しいMarketoインスタンスが必要になり、新しいMarketoインスタンスにインスタンスをコピーすることはできません。 代わりに、Marketoサポートに問い合わせて、プログラムの読み込み機能を試してください。

