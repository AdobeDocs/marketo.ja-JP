---
unique-page-id: 2949874
description: イベントの作成  [!DNL GotoWebinar] - Marketo ドキュメント – 製品ドキュメント
title: ' [!DNL GotoWebinar] を使用したイベントの作成'
exl-id: c0f0a202-e416-4523-b7d6-dbcfafc536cd
feature: Events
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '531'
ht-degree: 63%

---

# [!DNL GotoWebinar] を使用したイベントの作成 {#create-an-event-with-gotowebinar}

>[!PREREQUISITES]
>
>* [ サービ  [!DNL GoToWebinar]  として  [!DNL LaunchPoint]  追加 ](/help/marketo/product-docs/administration/additional-integrations/add-gotowebinar-as-a-launchpoint-service.md)
>* [新しいイベントプログラムの作成](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* 適切な[フローアクション](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)を設定して、エンゲージメントをトラック

まず、[!DNL GoToWebinar] でウェビナーを作成します。 [!DNL GoToWebinar] の作成に関する特定の設定はMarketoで使用され、その他の設定は [!DNL GoToWebinar] でのみ使用されます。

Marketo イベントを作成し、それに [!DNL GoToWebinar] ーザーを関連付けると、システムで登録と出席の情報を共有できるようになります。

以下に、Marketo で使用される設定の一覧を示します。

## タイトルと説明 {#title-and-description}

**[!UICONTROL タイトル]** - ウェビナーの名前を入力します。 この名前が Marketo で表示されます。

**[!UICONTROL 説明]**（オプション） - ウェビナーの説明を入力します。説明は Marketo で表示されます。

![](assets/image2015-5-28-15-3a1-3a36.png)

## 日時 {#date-time}

ウェビナーに関する次の情報を入力すると、アダプターを介して Marketo に取り込まれます。この情報に変更を加えた場合、Marketo で変更を表示するには「**[!UICONTROL イベントアクション]**」で「**[!UICONTROL ウェビナープロバイダーを更新]**」リンクをクリックする必要があります。

**[!UICONTROL 開始日]** – 開始日を入力します。 これは Marketo で表示できます。

**[!UICONTROL 開始時刻]** – 開始時刻を入力します。 これは Marketo で表示できます。

**[!UICONTROL 終了時刻]**  — 終了時刻を入力します。これは Marketo で表示できます。

**[!UICONTROL ウェビナータイムゾーン]** – 該当するタイムゾーンを選択します。 これは Marketo で表示できます。

**[!UICONTROL Type]** - **[!UICONTROL One Session]** に設定します。

![](assets/image2015-5-28-15-3a7-3a1.png)

>[!NOTE]
>
>Marketo は現在、定期的なウェビナーをサポートしていません。各Marketo イベントとウェビナーの間に 1 つのセッションを設定する必要 [!DNL GoToWebinar] あります。

>[!TIP]
>
>その他の [!DNL GoToWebinar] ヘルプが必要な場合は、[ ヘルプ サイト ](https://support.logmeininc.com/gotowebinar) を参照してください。

それでは、Marketo に移動しましょう。

1. イベントを選択します。「**[!UICONTROL イベントアクション]**」から、「**[!UICONTROL イベント設定]**」を選択します。

   ![](assets/image2015-5-14-14-3a53-3a10.png)

   >[!NOTE]
   >
   >選択したイベントプログラムのチャネルは&#x200B;**ウェビナー**&#x200B;である必要があります。

1. **[!UICONTROL イベントパートナー]**&#x200B;のリストから「**[!UICONTROL GoToWebinar]**」を選択します。

   ![](assets/image2015-5-14-14-3a55-3a20.png)

1. アカウントを選択します。

   ![](assets/rtaimage-2.png)

1. ウェビナーを選択します。

   ![](assets/image2015-5-14-14-3a57-3a31.png)

1. 「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2015-5-14-14-3a58-3a54.png)

1. これで完了です。これで、イベントが同期され、**[!DNL GoToWebinar]** によってスケジュールされました。

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
   >Marketo にデータが表示されるまでには、最大 48 時間かかる場合があります。その期間が経過しても何も表示されない場合は、イベントの **[!UICONTROL 概要]** タブにある [!UICONTROL &#x200B; イベントアクション &#x200B;] メニューから **[!UICONTROL ウェビナープロバイダーから更新]** を選択します。

ウェビナーに登録したユーザーは、[!UICONTROL &#x200B; 新しいステータス &#x200B;] が「登録済み」に設定されている [!UICONTROL &#x200B; プログラムステータスの変更 &#x200B;] フローステップを通じてウェビナープロバイダーにプッシュされます。 その他のステータスではプッシュされません。また、[!UICONTROL プログラムステータスを変更]フローステップ #1 と[!UICONTROL メールを送信]フローステップ #2 を必ず設定してください。

## スケジュールの表示  {#viewing-the-schedule}

プログラムスケジュール表示で、イベントのカレンダーエントリをクリックします。画面の右側にスケジュールが表示されます。

>[!NOTE]
>
>イベントスケジュールを変更するには、[!DNL GoToWebinar] でウェビナーを編集する必要があります。

![](assets/image2015-5-14-15-3a3-3a13.png)
