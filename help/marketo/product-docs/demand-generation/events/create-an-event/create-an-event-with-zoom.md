---
unique-page-id: 17728023
description: イベントの作成  [!DNL Zoom] - Marketo ドキュメント – 製品ドキュメント
title: ' [!DNL Zoom] を使用したイベントの作成'
exl-id: 6a2aec58-902c-4e40-ab59-9cc33ec83cea
feature: Events
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '549'
ht-degree: 65%

---

# [!DNL Zoom] を使用したイベントの作成 {#create-an-event-with-zoom}

>[!PREREQUISITES]
>
>* [Add [!DNL Zoom] as [!DNL LaunchPoint] Service](/help/marketo/product-docs/administration/additional-integrations/add-zoom-as-a-launchpoint-service.md)
>* [新しいイベントプログラムの作成](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* 適切な[フローアクション](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)を設定して、エンゲージメントをトラック

まず、[!DNL Zoom] でウェビナーを作成します。 [!DNL Zoom] の作成に関する特定の設定はMarketoで使用され、その他の設定は [!DNL Zoom] でのみ使用されます。

Marketo イベントを作成し、それに [!DNL Zoom] ウェビナーを関連付けると、システムで登録と出席の情報を共有できるようになります。 ウェビナーの作成のヘルプについては、[&#x200B; ウェビナーの概要  [!DNL Zoom]  を参照してください &#x200B;](https://support.zoom.us/hc/ja/articles/200917029-Getting-Started-With-Webinar)。

ウェビナーに関する次の情報を入力すると、アダプターを介して Marketo に取り込まれます。この情報に変更を加えた場合、Marketo で変更を表示するには、イベントアクションで「ウェビナープロバイダーから更新」リンクをクリックする必要があります。

**タイトルと説明**

* **ウェビナー名** — ウェビナーの名前を入力します。この名前が Marketo で表示されます。

* **説明**（オプション） - ウェビナーの説明を入力します。説明は Marketo で表示されます。

**日時**

* **開始日** – 開始日を入力します。Marketo で表示されます。

* **開始時間** - 開始時間を入力します。Marketo で表示されます。

* **所要時間** – 所要時間を入力します。開始時間と終了時間は Marketo で表示されます。

* **タイムゾーン** – 該当するタイムゾーンを選択します。Marketo で表示されます。

* **定期ミーティング** – チェックは外したままにします。

* **登録** – このボックスにチェックを入れて、登録を必須にします。Marketoのフォームまたはランディングページを使用して、[!DNL Zoom] にプッシュする登録情報をキャプチャします。

>[!NOTE]
>
>Marketo は現在、定期的なウェビナーをサポートしていません。各Marketo イベントとウェビナーの間に 1 つのセッションを設定する必要 [!DNL Zoom] あります。

![](assets/overview2.png)

>[!TIP]
>
>[!DNL Zoom] で設定する追加のフィールドがあり、統合には影響しません。 これらのフィールドについて詳しくは、[[!DNL Zoom]  ウェビナーヘルプセンター &#x200B;](https://support.zoom.us/hc/ja/sections/200324965-Video-Webinar) を参照してください。

それでは、Marketo に移動しましょう。

1. イベントを選択します。「**[!UICONTROL イベントアクション]**」から、「**[!UICONTROL イベント設定]**」を選択します。

   ![](assets/image2015-5-14-14-3a53-3a10-1.png)

   >[!NOTE]
   >
   >選択したイベントプログラムのチャネルは&#x200B;**ウェビナー**&#x200B;である必要があります。

1. **[!UICONTROL イベントパートナー]** リストから **[!UICONTROL ズーム]** を選択します。

   ![](assets/eventsettings1.png)

1. イベントを関連付ける [!DNL Zoom] アカウントを選択します。

   ![](assets/selectaccount.png)

1. ウェビナーを選択します。

   ![](assets/selectevent.png)

1. 「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/eventsettingssave.png)

   これで完了です。これで、イベントが同期され、[!DNL Zoom] によってスケジュールされました。

   >[!NOTE]
   >
   >Marketo が送信するフィールドは、姓、名、メールアドレスです。

   >[!TIP]
   >
   >登録後の確認メールにこの固有 URL を挿入するには、メールに `{{member.webinar url}}` トークンを使います。確認 URL が送信されるときに、このトークンは各リード固有の確認 URL に自動的に変換されます。
   >
   >配信停止やマーケティング中断したリードにも届くように、確認メールは&#x200B;**オペレーショナル**&#x200B;メールに設定してください。

   ウェビナーに登録したユーザーは、**[!UICONTROL 新しいステータス]** が「登録済み」に設定されている [!UICONTROL &#x200B; プログラムステータスの変更 &#x200B;] フローステップを通じてウェビナープロバイダーにプッシュされます。 その他のステータスではプッシュされません。また、**[!UICONTROL プログラムステータスを変更]**&#x200B;フローステップ #1 と&#x200B;**[!UICONTROL メールを送信]**&#x200B;フローステップ #2 を必ず設定してください。

   ![](assets/goto-webinar-1.png)

   >[!CAUTION]
   >
   >ネストされたメールプログラムを使用して確認メールを送信しないでください。代わりに、上に示しているように、イベントプログラムのスマートキャンペーンを使用します。

   >[!TIP]
   >
   >Marketo にデータが表示されるまでには、最大 48 時間かかる場合があります。しばらく待っても何も表示されない場合は、イベントの「**概要**」タブのイベントアクションメニューから「**ウェビナープロバイダーから更新**」を選択し、画面の右下にある更新アイコンをクリックします。
