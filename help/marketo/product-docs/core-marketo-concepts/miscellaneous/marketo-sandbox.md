---
unique-page-id: 11386358
description: 本番稼働前にテストするためのMarketo Engage サンドボックスについて説明します。 サンドボックスインスタンスを使用して、本番環境に影響を与えることなくテストを実施できます。
title: Marketo サンドボックス
exl-id: c040fac6-2290-4de5-b27d-2c7cb28f6e30
TQID: https://experienceleague.adobe.com/Cb1H0PKG-G0c4FkIcjI-erNzR0dwRtj7TwfqtwhFFMI
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: e2290edd-b061-4880-9d79-dee306cf5aa9
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 306
ht-degree: 59%

---

# Marketo サンドボックス {#marketo-sandbox}

Marketo Engage サンドボックスは、本番環境で実装する前にテスト目的で使用される追加のインスタンスです。

>[!AVAILABILITY]
>
>必ずしもすべてのお客様がこの機能を購入済みとは限りません。 詳しくは、アドビのアカウントチーム（担当のアカウントマネージャー）にお問い合わせください。

Marketo サンドボックスが実稼動インスタンスに既に同期されている場合、通常のCRMに同期することはできません。 同期に CRM のサンドボックスを使用し、元の同期と同じ手順をすべて実行します。

## サンドボックスについて知っておくべきこと {#things-to-know-about-sandboxes}

* ユーザーを追加する場合のプロセスは、[本番環境にユーザーを追加する](/help/marketo/product-docs/administration/users-and-roles/add-or-remove-a-user.md#add-a-user)場合のプロセスと同じです。 既に Marketo ログインを持っている場合は、別のメールアドレスを使用する必要があります。
* Marketo サンドボックスは空で始まりますが、本番稼働インスタンスと同じ機能を使用できます。
* サンドボックスでプログラムを作成し、それを本番環境に移動する場合は、[プログラムの読み込み](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md)を実行できます。
* サンドボックスは調整されるので、実稼動インスタンスはテスト環境の影響を受けません。 1 回のキャンペーン実行で最大 20 通のメールを送信できます。

>[!CAUTION]
>
>Marketo Dynamics _または_ Salesforce Syncのサンドボックスの更新は、現時点ではサポートされていません。 CRM サンドボックスを更新する必要がある場合は、新しいMarketo サンドボックスが必要です。 詳しくは、アドビのアカウントチーム（担当のアカウントマネージャー）にお問い合わせください。

## インスタンスコピー {#instance-copy}

サポートケースを送信して、1 回限りのインスタンスコピーでサンドボックスに入力するようリクエストできます。 ただし、インスタンスコピーは&#x200B;_すべて_&#x200B;を引き継ぐわけではありません。 詳しくは、[Marketo サポート &#x200B;](https://nation.marketo.com/t5/Support/ct-p/Support)にお問い合わせください。

>[!NOTE]
>
>ネイティブ CRMを変更する場合は、新しいMarketo インスタンスが必要になり、新しいMarketo インスタンスへのインスタンスのコピーは不可能になります。 代わりに、Marketo サポートと連携して、プログラムの読み込み機能を確認してください。
