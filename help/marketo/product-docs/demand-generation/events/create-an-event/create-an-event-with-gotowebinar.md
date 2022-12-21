---
unique-page-id: 2949874
description: GotoWebinar を使用したイベントの作成 - Marketo ドキュメント - 製品ドキュメント
title: GotoWebinar を使用したイベントの作成
exl-id: c0f0a202-e416-4523-b7d6-dbcfafc536cd
source-git-commit: 8b0625a7192a80986bc4295726cd13473493ddd7
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 100%

---

# GotoWebinar を使用したイベントの作成 {#create-an-event-with-gotowebinar}

>[!PREREQUISITES]
>
>* [GoToWebinar を LaunchPoint サービスとして追加](/help/marketo/product-docs/administration/additional-integrations/add-gotowebinar-as-a-launchpoint-service.md)
>* [新しいイベントプログラムの作成](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* 適切な[フローアクション](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)を設定して、エンゲージメントをトラック


まず、GotoWebinar でウェビナーを作成します。GotoWebinar の作成機能の設定には、Marketo で使用されるものと、GotoWebinar でのみ使用されるものがあります。

Marketo イベントプログラムを作成して GotoWebinar ウェビナーを関連付けると、システムは登録情報と出席情報を共有できるようになります。

以下に、Marketo で使用される設定の一覧を示します。

## タイトルと説明 {#title-and-description}

**ウェビナー名** - ウェビナーの名前を入力します。この名前が Marketo で表示されます。

**説明**（オプション） - ウェビナーの説明を入力します。説明は Marketo で表示されます。

![](assets/image2015-5-28-15-3a1-3a36.png)

## 日時 {#date-time}

ウェビナーに関する次の情報を入力すると、アダプターを介して Marketo に取り込まれます。この情報に変更を加えた場合、Marketo で変更を表示するには「**イベントアクション**」で「**ウェビナープロバイダーを更新**」リンクをクリックする必要があります。

**開始日** - 開始日を入力します。これは Marketo で表示できます。

**開始時刻** - 開始時刻を入力します。これは Marketo で表示できます。

**終了時刻**  — 終了時刻を入力します。これは Marketo で表示できます。

**タイムゾーン** – 該当するタイムゾーンを選択します。これは Marketo で表示できます。

**タイプ** - **One Session**.に設定

![](assets/image2015-5-28-15-3a7-3a1.png)

>[!NOTE]
>
>Marketo は現在、定期的なウェビナーをサポートしていません。各 Marketo イベントと GoToWebinar ウェビナーの間に 1 つのセッションを設定する必要があります。

>[!TIP]
>
>追加の GoToWebinar ヘルプが必要な場合は、[ヘルプサイト](https://support.logmeininc.com/gotowebinar)にアクセスしてください。

それでは、Marketo に移動しましょう。

1. イベントを選択します。「**イベントアクション**」から、「**イベント設定**」を選択します。

   ![](assets/image2015-5-14-14-3a53-3a10.png)

   >[!NOTE]
   >
   >選択したイベントプログラムのチャネルは&#x200B;**ウェビナー**&#x200B;である必要があります。

1. **イベントパートナー**&#x200B;のリストから「**GoToWebinar**」を選択します。

   ![](assets/image2015-5-14-14-3a55-3a20.png)

1. アカウントを選択します。

   ![](assets/rtaimage-2.png)

1. ウェビナーを選択します。

   ![](assets/image2015-5-14-14-3a57-3a31.png)

1. 「**保存**」をクリックします。

   ![](assets/image2015-5-14-14-3a58-3a54.png)

1. これで完了です。イベントは同期され&#x200B;**GoToWebinar** でスケジュールされました。

   ![](assets/image2015-5-14-15-3a0-3a47.png)

   >[!NOTE]
   >
   >Marketo が送信するフィールドは、姓、名、メールアドレスです。これらのフィールドは必須で、空にはできません。

   >[!TIP]
   >
   >登録後の確認メールにこの固有 URL を挿入するには、メールに `{{member.webinar url}}` トークンを使います。確認 URL が送信されるときに、このトークンは各リード固有の確認 URL に自動的に変換されます。
   >
   >配信停止やマーケティング中断したリードにも届くように、確認メールは&#x200B;**オペレーショナル**&#x200B;メールに設定してください。

   ![](assets/goto-webinar.png)

   >[!CAUTION]
   >
   >ネストされたメールプログラムを使用して確認メールを送信しないでください。代わりに、上に示しているように、イベントプログラムのスマートキャンペーンを使用します。

   >[!TIP]
   >
   >Marketo にデータが表示されるまでには、最大 48 時間かかる場合があります。48 時間待っても何も表示されない場合は、イベントの「**概要**」タブの「イベントアクション」メニューから「**ウェビナープロバイダーから更新**」を選択してください。

ウェビナーに新規登録したリードは、新規ステータスが「登録」に設定されたときに、プログラムステータスを変更フローステップによってウェビナープロバイダーにプッシュされます。その他のステータスではプッシュされません。また、プログラムステータスを変更フローステップ #1 とメールを送信フローステップ #2 を必ず設定してください。

## スケジュールの表示  {#viewing-the-schedule}

プログラムスケジュール表示で、イベントのカレンダーエントリをクリックします。画面の右側にスケジュールが表示されます。

>[!NOTE]
>
>イベントのスケジュールを変更するには、GoToWebinar でウェビナーを編集する必要があります。

![](assets/image2015-5-14-15-3a3-3a13.png)
