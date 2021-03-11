---
unique-page-id: 11386358
description: Marketo Sandbox - Marketto Docs — 製品ドキュメント
title: Marketo Sandbox
translation-type: tm+mt
source-git-commit: a7c90193e5c934119fa3b6bdf864d1458d1aad7c
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---


# Marketo Sandbox {#marketo-sandbox}

Marketo Sandboxは、実稼働環境に実装する前のテスト用に使用される追加のインスタンスです。

>[!AVAILABILITY]
>
>この機能を購入した顧客はいません。 詳しくは、カスタマーサクセスマネージャーにお問い合わせください。

Marketo Sandboxは、既に実稼働インスタンスと同期されている場合、通常のCRMと同期できません。 CRMのサンドボックスを同期に使用し、元の同期と同じ手順に従います。

## サンドボックスに関する知識{#things-to-know-about-sandboxes}

* Customer Success ManagerがSandboxを設定し、招待を送信したら、Marketo実稼働インスタンスとは異なる電子メールアドレスを使用してログインする必要があります。
* ユーザーを追加する場合の処理は、[実稼動環境](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md#create-users)にユーザーを追加するのと同じです。 再度言いますが、既にマーケティング担当者がログインしている場合は、別の電子メールアドレスを使用する必要があります。
* Marketo Sandboxは空のものを開始しますが、実稼働インスタンスと同じ機能を使用できます。
* サンドボックス内にプログラムを作成し、実稼働環境に移動する場合は、[プログラムインポート](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md)を実行できます。
* サンドボックスは制限されるので、実稼働インスタンスがテスト環境の悪影響を受けません。 1回のキャンペーンで最大30件の電子メールを送信できます。

>[!CAUTION]
>
>現在、Marketo Dynamics Syncのサンドボックス更新をサポートしていません。 Dynamics CRMサンドボックスを更新する必要がある場合は、新しいMarketo Sandboxが必要になります。 詳しくは、カスタマーサクセスマネージャーにお問い合わせください。

## インスタンスコピー{#instance-copy}

サポートケースを送信して、1回限りのインスタンスコピーをサンドボックスに入力するように要請することができます。 ただし、インスタンスコピーは、_すべて_&#x200B;を引き継ぐわけではありません。 詳しくは、[Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support)にお問い合わせください。

>[!NOTE]
>
>* ソースインスタンスがMicrosoft Dynamicsと統合されている場合、インスタンスコピーは&#x200B;****&#x200B;サポートされていません。
>* ネイティブCRMを変更する場合は、新しいMarketoのインスタンスが必要になり、新しいMarketoのインスタンスにインスタンスをコピーすることはできません。 代わりに、マーケティング担当者と協力して、プログラムのインポート機能を調査してください。

