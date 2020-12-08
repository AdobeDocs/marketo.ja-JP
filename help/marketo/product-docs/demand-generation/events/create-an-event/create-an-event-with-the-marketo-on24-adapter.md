---
unique-page-id: 10096656
description: Marketo ON24アダプタ — Marketto Docs — 製品ドキュメントを使用したイベントの作成
title: Marketo ON24アダプタを使用したイベントの作成
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---


# Marketo ON24アダプタを使用したイベントの作成 {#create-an-event-with-the-marketo-on-adapter}

## 始める前に {#before-you-begin}

Marketoでイベントを作成する際に推奨される構成要素と順序について詳しく理解する必要があります。 また、次のマーケティングの概念に関する実用的な知識も必要です。

* [マーケティングプログラム](../../../../product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md) 、イベント、およびそれらの違い
* [チャネル](../../../../product-docs/administration/tags/create-a-program-channel.md)
* [ローカルアセット](../../../../product-docs/core-marketo-concepts/programs/creating-programs/understanding-local-assets-in-a-program.md)
* [子キャンペーン](https://docs.marketo.com/x/IRCa) と [プログラムのステータス](../../../../product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md)

>[!NOTE]
>
>Marketor APIについて詳しくは、 [Marketor APIのドキュメント](http://developers.marketo.com/documentation/rest/) を参照してください。

## 前提条件 {#prerequisites}

Marketo ON24統合を使用するには、次が必要です。

* **ON24 Webキャストの購読** — 現在の購読がない場合は、ON24に直接問い合わせてください。 **注**:ON24 Hosted Editionが必要です。 ON24イベント管理は必要ありません。

* **ON24の管理者権限** — このコネクタを使用してON24システムでゲストを作成するには、この権限が必要です。
* **ON24接続資格情報** — 統合を有効にするには、次の情報をマーケティング担当者に入力する必要があります。ユーザー名、パスワード、クライアントID、およびクライアントキー。 資格情報に関するヘルプが必要な場合は、ON24アカウントマネージャーまたはON24サポートにお問い合わせください。
* **登録フォーム** - MarkettoフォームまたはMarkettoフォーム以外のフォームを適切なAPIと共に使用し、登録データと登録者情報がMarketoに確実に渡されるようにします。
* **登録の子キャンペーン- **イベントパートナーの統合が機能するには、Marketorイベントの登録の子キャンペーンを正しく作成し、設定する必要があります。

## プロセスフロー {#process-flow}

Marketo On24アダプタを使用してイベントを作成するには、次の手順に従います。

1. [MarketorにON24資格情報を入力](create-an-event-with-the-marketo-on24-adapter/enter-your-on24-credentials-in-marketo.md)
1. [ON24でのウェビナーイベントの作成](create-an-event-with-the-marketo-on24-adapter/create-your-webinar-event-in-on24.md)
1. [イベント設定の指定とマーケティングとウェビナーとの同期](create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md)
1. [子キャンペーンとローカルアセットの作成](create-an-event-with-the-marketo-on24-adapter/create-child-campaigns-and-local-assets.md)
1. [ON24イベント統合のテスト](create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md)
1. [ON24イベント統合の例](create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md)
1. [ウェビナープログラムのステータスについて](create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md)
1. [ON24イベント登録の更新](create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md)

>[!NOTE]
>
>**関連記事**
>
>* [ON24アダプタイベントについて](create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md)

>



