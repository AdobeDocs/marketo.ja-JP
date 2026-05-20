---
unique-page-id: 10096677
description: MarketoでON24 イベント統合をテストする方法について説明します。 同期、登録フロー、ステータスの更新が正しく機能することを確認します。
title: ON24 イベント統合のテスト
exl-id: 8326b81e-abf7-4615-9a0b-b0a579be8bb8
feature: Events
TQID: https://experienceleague.adobe.com/u5RzlTajaIZk5-9ESOX2LPYAj9bmbmMdJdraLwFlFqM
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 201
ht-degree: 82%

---

# ON24 イベント統合のテスト {#test-your-on-event-integration}

イベント統合を徹底的にテストします。

## 最初のキャンペーンを実行する前に推奨されるテストシーケンス {#recommended-test-sequence-before-running-your-first-campaign}

1. イベントの登録フォームに入力し、有効なメールアドレスを使用してテストします。
1. Marketo イベントのメンバーシップグリッドに、テスト名が「**登録済み**」ステータスで表示されることを確認します。
1. また、ON24 でテスト名が「**登録済み**」と表示されることを確認します。
1. テスト名の登録に使用した有効なメールアドレスで、イベント確認メールが受信されており、メールで一意の URL が解決されたことを確認します。

   >[!NOTE]
   >
   >各登録者のメールに一意の URL を表示するには、確認メールで `{{member.webinar url}}` トークンを使用する必要があります。

## イベント後 {#after-the-event}

イベントが発生した後にデータがどのように更新されるかを以下に示します。

* Marketo では、毎晩 ON24 から出席者データを取得します。
* Marketo と ON24 の間で出席者のデータ同期が完了すると、Marketo はメンバーシップのステータスを「[!UICONTROL 出席]」、「[!UICONTROL オンデマンドで出席]」、「[!UICONTROL 欠席]」に更新します。 イベントの「**[!UICONTROL 概要]**」タブで、イベントのステータスが「**[!UICONTROL イベント完了]**」に更新されます。

>[!MORELIKETHIS]
>
>* [ON24 イベント統合の例](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target="_blank"}
>* [Marketo ON24 アダプターイベントについて](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
