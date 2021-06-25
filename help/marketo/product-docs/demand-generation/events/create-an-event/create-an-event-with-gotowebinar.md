---
unique-page-id: 2949874
description: GotoWebセミナーを使用したイベントの作成 — Marketoドキュメント — 製品ドキュメント
title: GotoWebセミナーを使用したイベントの作成
exl-id: c0f0a202-e416-4523-b7d6-dbcfafc536cd
source-git-commit: 8b0625a7192a80986bc4295726cd13473493ddd7
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 0%

---

# GotoWebセミナーを使用したイベントの作成 {#create-an-event-with-gotowebinar}

>[!PREREQUISITES]
>
>* [GoToWebセミナーをLaunchPointサービスとして追加](/help/marketo/product-docs/administration/additional-integrations/add-gotowebinar-as-a-launchpoint-service.md)
* [新しいイベントプログラムの作成](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
* 適切な[フローアクション](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)を設定して、エンゲージメントを追跡します。


まず、GoToWebセミナーでウェビナーを作成します。 GoToWebセミナーの作成時の特定の設定はMarketoで使用され、一部はGoToWebinarでのみ使用されます。

Marketoイベントを作成し、GoToWebセミナーを関連付けると、登録情報と出席情報をシステムで共有できるようになります。

以下に、Marketoで使用される設定の一覧を示します。

## タイトルと説明 {#title-and-description}

**ウェビナー名**  — ウェビナーの名前を入力します。この名前はMarketoで表示できます。

**説明** （オプション） — ウェビナーの説明を入力します。説明はMarketoで表示できます。

![](assets/image2015-5-28-15-3a1-3a36.png)

## 日時 {#date-time}

ウェビナーの次の情報を入力すると、アダプターを介してMarketoに取り込まれます。 この情報に変更を加えた場合、Marketoに変更を表示するには、**イベントアクション**&#x200B;の下の「**ウェビナープロバイダーから更新**」リンクをクリックする必要があります。

**開始日**  — 開始日を入力します。これはMarketoで表示できます。

**開始時間**  — 開始時間を入力します。これはMarketoで表示できます。

**終了時間**  — 終了時間を入力します。これはMarketoで表示できます。

**タイムゾーン**  — 適切なタイムゾーンを選択します。Marketoで表示できます。

**「 —** 」を「 **One Session**」に設定します。

![](assets/image2015-5-28-15-3a7-3a1.png)

>[!NOTE]
Marketoは、現在、繰り返しウェビナーをサポートしていません。 Marketo EventとGoToWebセミナーの各ウェビナー間で1回のセッションを設定する必要があります。

>[!TIP]
追加のGoToウェビナーのヘルプが必要な場合は、[ヘルプサイト](https://support.logmeininc.com/gotowebinar)を参照してください。

さあ、Marketoに飛び込もう！

1. イベントを選択します。 「**イベントアクション**」をクリックし、「**イベント設定**」を選択します。

   ![](assets/image2015-5-14-14-3a53-3a10.png)

   >[!NOTE]
   選択するイベントのチャネルタイプは、**ウェビナー**&#x200B;にする必要があります。

1. 「**イベントパートナー**」リストから「**GoToWebinar**」を選択します。

   ![](assets/image2015-5-14-14-3a55-3a20.png)

1. アカウントを選択します。

   ![](assets/rtaimage-2.png)

1. ウェビナーを選択します。

   ![](assets/image2015-5-14-14-3a57-3a31.png)

1. 「**保存**」をクリックします。

   ![](assets/image2015-5-14-14-3a58-3a54.png)

1. 素晴らしい！ これで、イベントは&#x200B;**GoToWebinar**&#x200B;によって同期され、スケジュールされます。

   ![](assets/image2015-5-14-15-3a0-3a47.png)

   >[!NOTE]
   Marketoが送信するフィールドは次のとおりです。名、姓、電子メールアドレス。 これらのフィールドは必須で、空にすることはできません。

   >[!TIP]
   この一意のURLを確認Eメールに入力するには、Eメールで次のトークンを使用します。`{{member.webinar url}}`. 確認URLが送信されると、このトークンは自動的にユーザーの一意の確認URLに解決されます。
   確認メールを&#x200B;**Operational**&#x200B;に設定して、登録者および購読解除の可能性があるユーザーが引き続き確認情報を受け取るようにします。

   ![](assets/goto-webinar.png)

   >[!CAUTION]
   ネストされた電子メールプログラムを使用して確認電子メールを送信しないでください。 上に示すように、代わりに、イベントプログラムのスマートキャンペーンを使用します。

   >[!TIP]
   データがMarketoに表示されるまでに最大48時間かかる場合があります。 その時間待っても何も表示されない場合は、イベントの「**概要**」タブのイベントアクションメニューで「**ウェビナープロバイダーから更新**」を選択します。

「新しいステータス」が「登録済み」に設定されている場合、ウェビナーに登録した人は、プログラムステータスの変更フローステップを通じてウェビナープロバイダーにプッシュされます。 他のステータスでは、ユーザーを押し越すことはできません。 また、プログラムステータスの変更のフロー手順#1、電子メールの送信のフロー手順#2を必ず実行してください。

## スケジュールの表示  {#viewing-the-schedule}

プログラムスケジュールビューで、イベントのカレンダーエントリをクリックします。 画面の右側にスケジュールが表示されます。

>[!NOTE]
イベントのスケジュールを変更するには、GoToWebセミナーでウェビナーを編集する必要があります。

![](assets/image2015-5-14-15-3a3-3a13.png)
