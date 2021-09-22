---
unique-page-id: 10096656
description: Marketo ON24 アダプターを使用したイベントの作成 - Marketo ドキュメント - 製品ドキュメント
title: Marketo ON24 アダプターを使用したイベントの作成
exl-id: a240ff72-b12f-4e3a-8e14-94fddb02f944
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '296'
ht-degree: 100%

---

# Marketo ON24 アダプターを使用したイベントの作成 {#create-an-event-with-the-marketo-on-adapter}

## 始める前に {#before-you-begin}

Marketo でイベントを作成するための構成要素と推奨されるシーケンスについて理解しておく必要があります。また、次の Marketo のコンセプトに関する実務知識も必要です。

* [Marketo Program](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md) とイベントおよびそれらの違い
* [チャネル](/help/marketo/product-docs/administration/tags/create-a-program-channel.md)
* [ローカルアセット](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-local-assets-in-a-program.md)
* [子キャンペーン](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md)と[プログラムのステータス](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md)

>[!NOTE]
>
>Marketo API について詳しくは、[Marketo API のドキュメント](https://developers.marketo.com/documentation/rest/)を参照してください。

## 前提条件 {#prerequisites}

Marketo ON24 統合を使用するには、次の操作が必要です。

* **ON24 webcast のサブスクリプション** - 現在のサブスクリプションをお持ちでない場合は、ON24 に直接お問い合わせください。**注意**:ON24 Hosted Edition が必要です。ON24 イベント管理は不要です。

* **ON24 の管理者権限** - このコネクタを使用して ON24 システムでゲストを作成するには、この権限が必要です。
* **ON24 接続認証情報** - 統合を有効にするには、ユーザー名、パスワード、クライアント ID、クライアントキーを Marketo に入力する必要があります。認証情報に関してサポートが必要な場合は、ON24 アカウントマネージャーまたは ON24 サポートにお問い合わせください。
* **登録フォーム** - Marketo フォームまたは Marketo 以外のフォームと適切な API を使用して、登録データおよび登録者情報が Marketo に渡されるようにします。
* **登録子キャンペーン** - Marketo イベントで登録子キャンペーンを適切に作成し、設定して、イベントパートナー統合が機能するようにする必要があります。

## プロセスフロー {#process-flow}

Marketo On24 アダプターを使用してイベントを作成するには、次の手順に従います。

1. [Marketo での ON24 認証情報の入力](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/enter-your-on24-credentials-in-marketo.md)
1. [ON24 でのウェビナーイベントの作成](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-your-webinar-event-in-on24.md)
1. [イベントの設定と Marketo とウェビナーの同期](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md)
1. [子キャンペーンとローカルアセットの作成](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-child-campaigns-and-local-assets.md)
1. [ON24 イベント統合のテスト](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md)
1. [ON24 イベント統合の例](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md)
1. [ウェビナープログラムのステータスについて](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md)
1. [ON24 イベント登録の更新](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md)
