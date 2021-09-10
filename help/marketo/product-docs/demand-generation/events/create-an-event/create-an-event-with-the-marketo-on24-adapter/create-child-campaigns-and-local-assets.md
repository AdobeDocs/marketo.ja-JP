---
unique-page-id: 10096675
description: 子キャンペーンとローカルアセットの作成 — Marketo ドキュメント — 製品ドキュメント
title: 子キャンペーンとローカルアセットの作成
exl-id: 272105e1-43d6-455c-a533-aae65e859384
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '667'
ht-degree: 100%

---

# 子キャンペーンとローカルアセットの作成 {#create-child-campaigns-and-local-assets}

Design Studio を使用して、子キャンペーンとローカルアセットを作成します。

## ランディングページとフォーム {#landing-page-and-form}

担当者が ON24 に適切に登録されるようにするには、次のフィールドを Marketo フォームに含める必要があります。

* 名
* 姓
* メールアドレス

次のフィールドを ON24 にプッシュすることもできます。

* 企業名
* 職位

登録キャンペーンに適切なフローステップが追加されると、担当者は ON24 にプッシュされ、登録済みとマークされます。その他のフィールドをフォームに追加すると、その情報が Marketo に担当者の詳細レコードの一部として取り込まれます。

>[!CAUTION]
>
>統合を成功させるには、Marketo フォームを使用してイベントに担当者を登録するか、適切な API 統合による Marketo 以外のフォームを使用して Marketo に登録データをプッシュする必要があります。

## メールと URL トークン {#emails-and-url-tokens}

Marketo を使用して、招待メール、確認メール、フォローアップメール、お礼メールを作成します。

## Marketo 確認メールと URL トークン {#marketo-confirmation-email-and-url-token}

Marketo を使用して、イベントの確認メールを送信します。担当者が登録すると、イベントへの参加に使用する一意の URL を受け取ります。

>[!NOTE]
>
>この一意の URL を確認メールに入力するには、メールでトークン `{{member.webinar url}}` を使用します。確認 URL を送信すると、このトークンは自動的に担当者の一意の確認 URL に解決されます。
>
>確認メールのタイプを&#x200B;**オペレーショナル**&#x200B;に設定して、登録する担当者がたとえ配信停止されても確実に確認情報を受け取れるようにします。

>[!TIP]
>
>確認メール、リマインダーメールまたはフォローアップメールを送信するように ON24 を設定できます。詳しくは、[ON24 のヘルプサイト](https://webcastelitehelp.on24.com)を参照してください。

## 登録の子キャンペーンの要件 {#registration-child-campaign-requirements}

イベントには、1 つ以上の子キャンペーンが含まれます。これらのキャンペーンがすべて連携して、プログラムステータスに担当者を導き、イベントのパフォーマンスをトラッキングできます。

子キャンペーンの例としては、招待キャンペーン、登録キャンペーン、フォローアップキャンペーンなどがあります。

>[!CAUTION]
>
>アダプターがジョブを実行するには、登録キャンペーンを作成する必要があります。このキャンペーンは、フォームの入力者によってトリガーされ、最初の手順で、担当者のプログラムステータスを&#x200B;**登録済み**&#x200B;に変更する必要があります。次に、キャンペーンが確認メールを送信します。詳しくは、この記事の残りの部分を参照してください。

**登録／確認（トリガーキャンペーン）**

* スマートリスト
* **フォームへの記入**&#x200B;に基づくトリガー。特に同じフォームが複数のランディングページで使用される場合は、「**制約の追加**」を使用して、フォームが存在するランディングページを必ず含めてください。

>[!CAUTION]
>
>Marketo フォームを使用してイベントに担当者を登録するか、適切な API 統合による Marketo 以外のフォームを使用して Marketo に登録データをプッシュする必要があります。これは、イベントパートナー統合を成功させるうえで重要です。

>[!NOTE]
>
>Marketo 以外のランディングページで Marketo フォームを使用している場合、トリガーは、フォーム名を含む&#x200B;**フォームへの記入**&#x200B;になります。

![](assets/image2015-12-22-15-3a20-3a51.png)

**フロー**

* **プログラムステータスの変更** — ウェビナー／登録済みに設定します。

このフローステップは、子キャンペーンを設定する際の最初のフローステップとして必要です。担当者のプログラムステータスが「登録済み」に変更されると、Marketo は登録情報を ON24 にプッシュします。他のステータスでは、担当者をプッシュすることはできません。

* **メールの送信** — 確認メール。このメールを&#x200B;**オペレーショナル**&#x200B;に設定して、登録した配信停止済みの担当者が引き続きメールを受け取れるようにします。

**メールの送信**&#x200B;フローステップは、2 番目のステップである必要があります。確認メールには、ON24 から Marketo に送信された情報が入力された `{{member.webinar url}}` が含まれます。

![](assets/image2015-12-22-15-3a29-3a50.png)

>[!NOTE]
>
>これらのフローステップの順序は、Marketo でアクションが実行される順序なので、重要です。**プログラムステータスの変更**&#x200B;ステップでは、登録のために ON24 に担当者を送信して、一意の URL が生成されます。この後、`{{member.webinar URL}}` トークンを使用して、この一意の URL を含む確認メールを送信できます。
>
>登録エラーが発生した場合、その担当者には確認メールは送信されません。

次のステップは、[ON24 イベント統合のテスト](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md)です。

>[!MORELIKETHIS]
>
>* [Marketo ON24 アダプターイベントについて](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md)
>* [ON24 イベント統合の例](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md)
>* [ウェビナープログラムステータスについて](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md)

