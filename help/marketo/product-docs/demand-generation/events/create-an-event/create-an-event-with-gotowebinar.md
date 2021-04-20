---
unique-page-id: 2949874
description: GotoWebセミナー —Marketoドキュメント — 製品ドキュメントでイベントを作成する
title: GotoWebセミナーでのイベントの作成
exl-id: c0f0a202-e416-4523-b7d6-dbcfafc536cd
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 0%

---

# GotoWebinar {#create-an-event-with-gotowebinar}を使用してイベントを作成

>[!PREREQUISITES]
>
>* [LaunchPointサービス追加としてのGoToWebセミナー](/help/marketo/product-docs/administration/additional-integrations/add-gotowebinar-as-a-launchpoint-service.md)
>* [新しいイベントプログラムの作成](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* 適切な[フローアクション](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)を設定して、エンゲージメントを追跡します。


まず、GoToWebinarでウェビナーを作成します。 GoToWebinarの作成時の設定は、Marketoが使用する設定と、GoToWebinarのみが使用する設定があります。

Marketoイベントを作成し、GoToWebセミナーを関連付けると、登録情報と出席情報を共有できるようになります。

以下はMarketoが使用する設定のリストです。

## タイトルと説明{#title-and-description}

**ウェビナー名**  — ウェビナー名を入力します。この名前はMarketoで表示できます。

**説明** （オプション） — ウェビナーの説明を入力します。説明はMarketoで表示できます。

![](assets/image2015-5-28-15-3a1-3a36.png)

## 日時 {#date-time}

ウェビナーの次の情報を入力すると、アダプタを介してMarketoに取り込まれます。 この情報に変更を加えた場合、Marketoが変更を確認できるようにするには、**イベントアクション**&#x200B;の下の「ウェビナープロバイダーから更新&#x200B;**」リンクをクリックする必要があります。**

**開始日** -開始日を入力します。これはMarketoで見ることができます。

**開始時刻** -開始時刻を入力します。これはMarketoで見ることができます。

**終了時間**  — 終了時間を入力します。これはMarketoで見ることができます。

**タイムゾーン**  — 該当するタイムゾーンを選択します。Marketoで見ることができます。

**「 —** set」を「 **One Session**」に設定します。

![](assets/image2015-5-28-15-3a7-3a1.png)

>[!NOTE]
>
>Marketoは現在、ウェビナーの定期的な使用をサポートしていません。 各MarketoイベントとGoToWebセミナーの間に、1回のセッションを設定する必要があります。

>[!TIP]
>
>追加のGoToWebセミナーのヘルプが必要な場合は、[ヘルプサイト](https://support.logmeininc.com/gotowebinar)を参照してください。

さあMarketoに飛び込もう！

1. イベントを選択します。 「**イベントアクション**」をクリックし、「**イベント設定**」を選択します。

   ![](assets/image2015-5-14-14-3a53-3a10.png)

   >[!NOTE]
   >
   >選択するイベントのチャネルタイプは、**ウェビナー**&#x200B;でなければなりません。

1. **イベントパートナー**&#x200B;リストから&#x200B;**GoToWebinar**&#x200B;を選択します。

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
   >
   >Marketoが送り込むフィールドは次のとおりです。名、姓、電子メールアドレス。 これらのフィールドは必須で、空にすることはできません。

   >[!TIP]
   >
   >この一意のURLを確認電子メールに入力するには、電子メールで次のトークンを使用します。`{{member.webinar url}}`. 確認URLが送信されると、このトークンは、ユーザー固有の確認URLに自動的に解決されます。
   >
   >確認の電子メールを&#x200B;**操作**&#x200B;に設定し、登録済みで登録を取り消している可能性のあるユーザーが、確認情報を引き続き受け取るようにします。

   ![](assets/goto-webinar.png)

   >[!CAUTION]
   >
   >確認電子メールを送信する際に、ネストされた電子メールプログラムを使用しないでください。 代わりに、イベントプログラムのスマートキャンペーンを使用します。

   >[!TIP]
   >
   >データがMarketoに表示されるまで、最大48時間かかる場合があります。 それでも何も表示されない状態が続くのを待った後で、イベントーの&#x200B;**概要**&#x200B;タブにあるイベントの操作メニューから、「ウェビナープロバイダーから更新&#x200B;**」を選択します。**

ウェビナーにサインアップした人は、「新しいステータス」が「登録済み」に設定されている場合に、プログラムステータスの変更フローステップを通じてウェビナーのプロバイダーにプッシュされます。 その他の状態では、その人を押しのけることはありません。 また、プログラムステータスの変更のフロー手順#1と、電子メールの送信のフロー手順#2を必ず行ってください。

## スケジュールの表示{#viewing-the-schedule}

プログラムスケジュール表示で、イベントのカレンダーエントリをクリックします。 スケジュールは、画面の右側に表示されます。

>[!NOTE]
>
>イベントのスケジュールを変更するには、GoToWebinarでウェビナーを編集する必要があります。

![](assets/image2015-5-14-15-3a3-3a13.png)
