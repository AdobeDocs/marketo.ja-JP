---
unique-page-id: 10096656
description: MarketoON24アダプタ —Marketoドキュメント — 製品ドキュメントを使用してイベントを作成する
title: MarketoON24アダプタを使用したイベントの作成
exl-id: a240ff72-b12f-4e3a-8e14-94fddb02f944
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 1%

---

# MarketoON24アダプタ{#create-an-event-with-the-marketo-on-adapter}を使用してイベントを作成する

## 始める前に{#before-you-begin}

Marketoでイベントを作成する際に推奨される構成要素と順序を理解しておく必要があります。 また、次のMarketoの概念に関する実務的な知識も必要です。

* [Marketo](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md) プログラムとイベント、およびそれらの違い
* [チャネル](/help/marketo/product-docs/administration/tags/create-a-program-channel.md)
* [ローカル アセット](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-local-assets-in-a-program.md)
* [子](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md) キャンペーンと [プログラムのステータス](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md)

>[!NOTE]
>
>MarketoAPIについて詳しくは、[MarketoAPIドキュメント](https://developers.marketo.com/documentation/rest/)を参照してください。

## 前提条件{#prerequisites}

MarketoON24統合を使用するには、次が必要です。

* **ON24 Webキャストの購読**  — 現在の購読がない場合は、ON24に直接問い合わせてください。**注**:ON24 Hosted Editionが必要です。ON24イベント管理は必要ありません。

* **ON24に対する管理者権限**  — このコネクタを使用してON24システムでゲストを作成するには、この権限が必要です。
* **ON24接続資格情報**  — 統合を有効にするには、次の情報をMarketoに入力する必要があります。ユーザー名、パスワード、クライアントID、およびクライアントキー。資格情報に関するヘルプが必要な場合は、ON24アカウントマネージャーまたはON24サポートにお問い合わせください。
* **登録フォーム** -MarketoフォームまたはMarketo以外のフォームを適切なAPIと共に使用し、登録データと登録者情報がMarketoに渡されるようにします。
* **登録児童キャンペーン** -Marketoイベントで登録児童キャンペーンを作成し、イベントパートナー統合が機能するように適切に設定する必要があります。

## プロセスフロー{#process-flow}

MarketoOn24アダプタを使用してイベントを作成するには、次の手順に従います。

1. [ON24資格情報をMarketoに入力](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/enter-your-on24-credentials-in-marketo.md)
1. [ON24でのウェビナーイベントの作成](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-your-webinar-event-in-on24.md)
1. [イベント設定の指定とMarketoとウェビナーの同期](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md)
1. [子キャンペーンとローカルアセットの作成](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-child-campaigns-and-local-assets.md)
1. [ON24イベント統合のテスト](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md)
1. [ON24イベント統合の例](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md)
1. [ウェビナープログラムのステータスについて](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md)
1. [ON24イベント登録の更新](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md)
