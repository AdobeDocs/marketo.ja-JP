---
unique-page-id: 17728023
description: ズームを使用したイベントの作成 — Marketoドキュメント — 製品ドキュメント
title: ズームを使用したイベントの作成
exl-id: 6a2aec58-902c-4e40-ab59-9cc33ec83cea
source-git-commit: 8b0625a7192a80986bc4295726cd13473493ddd7
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 0%

---

# ズームを使用したイベントの作成 {#create-an-event-with-zoom}

>[!PREREQUISITES]
>
>* [LaunchPointサービスとしてのズームの追加](/help/marketo/product-docs/administration/additional-integrations/add-zoom-as-a-launchpoint-service.md)
* [新しいイベントプログラムの作成](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
* 適切な[フローアクション](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)を設定して、エンゲージメントを追跡します。


まず、「ズーム」でウェビナーを作成します。 ズームの作成時の特定の設定はMarketoで使用され、一部はズームでのみ使用されます。

Marketoイベントを作成し、Zoom Webセミナーを関連付けると、登録と参加に関する情報をシステムが共有できるようになります。 ウェビナーの作成については、[ズームウェビナーの概要](https://support.zoom.us/hc/en-us/articles/200917029-Getting-Started-With-Webinar)を参照してください。

ウェビナーの次の情報を入力すると、アダプターを介してMarketoに取り込まれます。 この情報に変更を加えた場合、Marketoで変更を表示するには、「イベントの操作」の下の「ウェビナープロバイダーを更新」リンクをクリックする必要があります。

**タイトルと説明**

* **ウェビナー名**  — ウェビナーの名前を入力します。この名前はMarketoで表示できます。

* **説明** （オプション） — ウェビナーの説明を入力します。説明はMarketoで表示できます。

**日時**

* **開始日**  — 開始日を入力します。これはMarketoで表示できます。

* **開始時間**  — 開始時間を入力します。これはMarketoで表示できます。

* **期間**  — 期間を入力します。開始時刻と終了時刻は、Marketoで表示できます。

* **タイムゾーン**  — 適切なタイムゾーンを選択します。これはMarketoで表示できます。

* **繰り返しウェビナー** — オフのままにします。

* **登録**  — 登録を必須にするには、このチェックボックスをオンにします。Marketoのフォーム/ランディングページを使用して、ズームにプッシュされる登録情報を取り込みます。

>[!NOTE]
Marketoは、現在、繰り返しウェビナーをサポートしていません。 Marketo EventとZoomの各ウェビナー間で1回のセッションを設定する必要があります。

![](assets/overview2.png)

>[!TIP]
統合に影響を与えない、ズームで設定する追加のフィールドがあります。 これらのフィールドについて詳しくは、 [ズームウェビナーのヘルプセンター](https://support.zoom.us/hc/en-us/sections/200324965-Video-Webinar)を参照してください。

さあ、Marketoに飛び込もう！

1. イベントを選択します。 「**イベントアクション**」をクリックし、「**イベント設定**」を選択します。

   ![](assets/image2015-5-14-14-3a53-3a10-1.png)

   >[!NOTE]
   選択するイベントのチャネルタイプは、**ウェビナー**&#x200B;にする必要があります。

1. **イベント** **パートナー**&#x200B;リストから「**ズーム**」を選択します。

   ![](assets/eventsettings1.png)

1. イベントを関連付けるZoomアカウントを選択します。

   ![](assets/selectaccount.png)

1. ウェビナーを選択します。

   ![](assets/selectevent.png)

1. 「**保存**」をクリックします。

   ![](assets/eventsettingssave.png)

   素晴らしい！ これで、イベントがズームによって同期され、スケジュールされます。

   >[!NOTE]
   Marketoが送信するフィールドは次のとおりです。名、姓、電子メールアドレス。

   >[!TIP]
   この一意のURLを確認Eメールに入力するには、Eメールで次のトークンを使用します。`{{member.webinar url}}`. 確認URLが送信されると、このトークンは自動的にユーザーの一意の確認URLに解決されます。
   確認メールを&#x200B;**Operational**&#x200B;に設定して、登録者および購読解除の可能性があるユーザーが引き続き確認情報を受け取るようにします。

   ウェビナーに新規登録した人は、「新規ステータス」が「登録済み」に設定されると、**プログラムステータスの変更**&#x200B;フローステップを通じてウェビナープロバイダーにプッシュされます。 他のステータスでは、ユーザーを押し越すことはできません。 また、**プログラムステータスの変更**&#x200B;のフロー手順#1、**電子メールの送信**&#x200B;のフロー手順#2を必ず実行してください。

   ![](assets/goto-webinar-1.png)

   >[!CAUTION]
   ネストされた電子メールプログラムを使用して確認電子メールを送信しないでください。 上に示すように、代わりに、イベントプログラムのスマートキャンペーンを使用します。

   >[!TIP]
   データがMarketoに表示されるまでに最大48時間かかる場合があります。 その時間待っても何も表示されない場合は、イベントの「**概要**」タブのイベントアクションメニューで「**ウェビナープロバイダーから更新**」を選択します。
