---
unique-page-id: 10096675
description: 子キャンペーンとローカルアセットの作成 —Marketoドキュメント — 製品ドキュメント
title: 子キャンペーンとローカルアセットの作成
exl-id: 272105e1-43d6-455c-a533-aae65e859384
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '667'
ht-degree: 1%

---

# 子キャンペーンとローカルアセットの作成{#create-child-campaigns-and-local-assets}

Design Studioを使用して、子キャンペーンとローカルアセットを作成します。

## ランディングページとフォーム{#landing-page-and-form}

ON24にユーザーが正しく登録されるようにするには、以下のフィールドをMarketoフォームに含める必要があります。

* 名 
* 姓
* メールアドレス

次のフィールドをON24にプッシュすることもできます。

* 企業名
* 職位

登録キャンペーンに適切なフローステップが追加されると、ユーザはON24に押され、登録済みとマークされます。 他のフィールドをフォームに追加すると、その情報がMarketoで個人の詳細レコードの一部として取り込まれます。

>[!CAUTION]
>
>統合を成功させるには、Marketoフォームを使用してイベントにユーザーを登録するか、Marketo以外のフォームを適切なAPI統合によってMarketoに登録データをプッシュする必要があります。

## 電子メールとURLトークン{#emails-and-url-tokens}

Marketoを使用して、招待、確認、フォローアップ、お礼の電子メールを作成します。

## Marketo確認電子メールとURLトークン{#marketo-confirmation-email-and-url-token}

Marketoを使用して、イベントの確認メールを送信します。 登録を行うと、イベントの入力に使用する一意のURLを受け取ります。

>[!NOTE]
>
>この一意のURLを確認電子メールに入力するには、電子メールで次のトークンを使用します。`{{member.webinar url}}`. 確認URLを送信すると、このトークンはユーザー固有の確認URLに自動的に解決されます。
>
>確認電子メールの種類を&#x200B;**操作**&#x200B;に設定し、登録したユーザーが登録を取り消しても確認情報を確実に受け取れるようにします。

>[!TIP]
>
>ON24を設定して、確認、リマインダーまたはフォローアップ電子メールを送信できます。 詳しくは、[ON24のヘルプサイト](https://webcastelitehelp.on24.com)を参照してください。

## 登録の子キャンペーン要件{#registration-child-campaign-requirements}

イベントには1つ以上の子キャンペーンが含まれており、すべてが連携してプログラムのステータス間を移動し、イベントのパフォーマンスを追跡できます。

子キャンペーンの例としては、招待キャンペーン、登録キャンペーン、フォローアップキャンペーンなどがあります。

>[!CAUTION]
>
>アダプタがそのジョブを実行するには、登録キャンペーンを作成する必要があります。 このキャンペーンは、フォームの入力者がトリガーする必要があり、最初の手順では、ユーザーのプログラムステータスを&#x200B;**登録済み**&#x200B;に変更する必要があります。 次に、キャンペーンが確認電子メールを送信します。 詳しくは、この記事の残りの部分を参照してください。

**登録/確認(トリガーキャンペーン)**

* スマートリスト
* **Fills Out Form**&#x200B;に基づくトリガー。 **制約追加**&#x200B;を使用して、フォームが存在するランディングページを必ず含めてください。特に、同じフォームが複数のランディングページで使用される場合には、この制約を使用します。

>[!CAUTION]
>
>イベント用にユーザーを登録するにはMarketoのフォームを使用する必要があります。登録データをMarketoにプッシュするには、Marketo以外のフォームを適切なAPI統合によって登録する必要があります。 これは、イベントパートナー統合を成功させるうえで重要です。

>[!NOTE]
>
>Marketo以外のランディングページでMarketoフォームを使用している場合、トリガーは「**フォーム**&#x200B;にフォーム名を入力します。

![](assets/image2015-12-22-15-3a20-3a51.png)

**フロー**

* **プログラムステータスの変更**  — ウェビナー —>登録済みに設定します。

子キャンペーンの設定時には、このフローステップがFIRST FLOW STEPとして必要になります。 個人のプログラムステータスが「登録済み」に変わると、Marketoは登録情報をON24にプッシュします。 その他の状態では、その人を押しのけることはありません。

* **電子メールの送信**  — 確認の電子メール。この電子メールを&#x200B;**Operational**&#x200B;に設定すると、登録した登録解除済みのユーザーが引き続きこの電子メールを受け取るようになります。

**電子メール**&#x200B;の送信フローステップは2番目のステップである必要があります。 確認の電子メールには`{{member.webinar url}}`が含まれており、ON24からMarketoに送り返された情報が入力されます。

![](assets/image2015-12-22-15-3a29-3a50.png)

>[!NOTE]
>
>Marketoで行われる行動の順序が重要なので、これらのフローステップの順序は重要です。 **プログラムステータスの変更**&#x200B;ステップは、ユーザーをON24に送信して登録し、一意のURLを生成します。 この問題が発生したら、`{{member.webinar URL}}`トークンを使用して、この一意のURLを含む確認電子メールを送信できます。
>
>登録エラーが発生して返品された場合、そのユーザーは電子メールによる確認を受け取りません。

次のステップは、[ON24イベント統合のテスト](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md)です。

>[!MORELIKETHIS]
>
>* [MarketoON24アダプタイベントについて](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md)
>* [ON24イベント統合の例](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md)
>* [ウェビナープログラムのステータスについて](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md)

