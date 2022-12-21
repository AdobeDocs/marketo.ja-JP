---
unique-page-id: 10096656
description: Marketo ON24 アダプターを使用したイベントの作成 - Marketo ドキュメント - 製品ドキュメント
title: Marketo ON24 アダプターを使用したイベントの作成
exl-id: a240ff72-b12f-4e3a-8e14-94fddb02f944
source-git-commit: 0c6c119f5be6e2ac3db7d99f7e8623d8aaa3555c
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 100%

---

# Marketo ON24 アダプターを使用したイベントの作成 {#create-an-event-with-the-marketo-on-adapter}

Marketo でイベントを作成するための構成要素と推奨されるシーケンスについて理解しておく必要があります。また、次の Marketo のコンセプトに関する実務知識も必要です。

* [Marketo プログラム](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md){target=&quot;_blank&quot;} とイベントおよびそれらの違い
* [チャネル](/help/marketo/product-docs/administration/tags/create-a-program-channel.md){target=&quot;_blank&quot;}
* [ローカルアセット](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-local-assets-in-a-program.md){target=&quot;_blank&quot;}
* [子キャンペーン](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md){target=&quot;_blank&quot;}および[プログラムステータス](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md){target=&quot;_blank&quot;}

>[!NOTE]
>
>Marketo API について詳しくは、[Marketo API のドキュメント](https://developers.marketo.com/documentation/rest/){target=&quot;_blank&quot;}を参照してください。

## 前提条件 {#prerequisites}

Marketo ON24 統合を使用するには、次の操作が必要です。

* **ON24 webcast のサブスクリプション** - 現在のサブスクリプションをお持ちでない場合は、ON24 に直接お問い合わせください。**注意**:ON24 Hosted Edition が必要です。ON24 イベント管理は不要です。

* **ON24 の管理者権限** - このコネクタを使用して ON24 システムでゲストを作成するには、この権限が必要です。
* **ON24 接続認証情報** - 統合を有効にするには、ユーザ名、パスワード、クライアント ID、クライアントキーを Marketo に入力する必要があります。認証情報に関してサポートが必要な場合は、ON24 アカウントマネージャーまたは ON24 サポートにお問い合わせください。
* **登録フォーム** - Marketo フォームまたは Marketo 以外のフォームと適切な API を使用して、登録データおよび登録者情報が Marketo に渡されるようにします。
* **登録子キャンペーン** - Marketo イベントで登録子キャンペーンを適切に作成し、設定して、イベントパートナー統合が機能するようにする必要があります。

## プロセスフロー {#process-flow}

Marketo ON24 アダプターを使用してイベントを作成するには、次の手順に従います。

1. [ON24 でのウェビナーイベントの作成](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-your-webinar-event-in-on24.md){target=&quot;_blank&quot;}
1. [イベントの設定と Marketo とウェビナーの同期](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md){target=&quot;_blank&quot;}
1. [子キャンペーンとローカルアセットの作成](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-child-campaigns-and-local-assets.md){target=&quot;_blank&quot;}
1. [ON24 イベント統合のテスト](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md){target=&quot;_blank&quot;}
1. [ON24 イベント統合の例](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target=&quot;_blank&quot;}
1. [ウェビナープログラムのステータスについて](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md){target=&quot;_blank&quot;}
1. [ON24 イベント登録のアップデート](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md){target=&quot;_blank&quot;}
