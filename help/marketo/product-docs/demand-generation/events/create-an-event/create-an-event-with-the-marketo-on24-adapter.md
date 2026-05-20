---
unique-page-id: 10096656
description: Marketo ON24 アダプタを使用してイベントを作成する方法を説明します。 ON24 ウェビナーをMarketoと連携させ、登録と出席を同期できます。
title: Marketo ON24 アダプターを使用したイベントの作成
exl-id: a240ff72-b12f-4e3a-8e14-94fddb02f944
feature: Events
TQID: https://experienceleague.adobe.com/LlMV9lfVxqvMh0E-6K3aStBiqOERGIKJOYSyJdaBvFw
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 303
ht-degree: 75%

---

# Marketo ON24 アダプターを使用したイベントの作成 {#create-an-event-with-the-marketo-on-adapter}

Marketo でイベントを作成するための構成要素と推奨されるシーケンスについて理解しておく必要があります。 また、次の Marketo のコンセプトに関する実務知識も必要です。

* [Marketo Program](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md){target="_blank"} とイベントおよびそれらの違い
* [チャネル](/help/marketo/product-docs/administration/tags/create-a-program-channel.md){target="_blank"}
* [ローカルアセット](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-local-assets-in-a-program.md){target="_blank"}
* [子キャンペーン](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md){target="_blank"}と[プログラムのステータス](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md){target="_blank"}

>[!NOTE]
>
>Marketo APIについて詳しくは、[Marketo API ドキュメント &#x200B;](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}を参照してください。

## 前提条件 {#prerequisites}

Marketo ON24 統合を使用するには、次の操作が必要です。

* **ON24 webcast のサブスクリプション** - 現在のサブスクリプションをお持ちでない場合は、ON24 に直接お問い合わせください。 **注意**:ON24 Hosted Edition が必要です。 ON24 イベント管理は不要です。

* **ON24**&#x200B;への管理者権限 – このコネクタを使用してON24 システムでゲストを作成するには、この権限が必要です。
* **ON24接続資格情報** – 統合を有効にするには、この情報をMarketoに入力する必要があります（ユーザー名、パスワード、クライアント ID、クライアントキー）。 資格情報に関してサポートが必要な場合は、ON24 アカウントマネージャーまたは ON24 サポートにお問い合わせください。
* **登録フォーム** - Marketo フォームまたは Marketo 以外のフォームと適切な API を使用して、登録データおよび登録者情報が Marketo に渡されるようにします。
* **登録子キャンペーン** - Marketo イベントで登録子キャンペーンを適切に作成し、設定して、イベントパートナー統合が機能するようにする必要があります。

## プロセスフロー {#process-flow}

Marketo ON24 アダプターを使用してイベントを作成するには、次の手順に従います。

1. [ON24 でのウェビナーイベントの作成](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-your-webinar-event-in-on24.md){target="_blank"}
1. [イベントの設定と Marketo とウェビナーの同期](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md){target="_blank"}
1. [子キャンペーンとローカルアセットの作成](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-child-campaigns-and-local-assets.md){target="_blank"}
1. [ON24 イベント統合のテスト](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md){target="_blank"}
1. [ON24 イベント統合の例](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target="_blank"}
1. [ウェビナープログラムのステータスについて](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md){target="_blank"}
1. [ON24 イベント登録のアップデート](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md){target="_blank"}
