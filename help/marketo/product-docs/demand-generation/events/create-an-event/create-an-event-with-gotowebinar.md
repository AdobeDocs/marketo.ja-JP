---
unique-page-id: 2949874
description: GotoWebセミナー — Marketto Docs — 製品ドキュメントを使用したイベントの作成
title: GotoWebセミナーでのイベントの作成
translation-type: tm+mt
source-git-commit: c8a77dc84c023e05fbb442f575269aac108ffb29
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---


# GotoWebセミナーでのイベントの作成 {#create-an-event-with-gotowebinar}

>[!PREREQUISITES]
>
>* [LaunchPointサービス追加としてのGoToWebセミナー](/help/marketo/product-docs/administration/additional-integrations/add-gotowebinar-as-a-launchpoint-service.md)
>* [新しいイベントプログラムの作成](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* 適切な [フロー](http://docs.marketo.com/display/DOCS/Flow+Actions)アクションを設定して、エンゲージメントを追跡する


まず、GoToWebinarでウェビナーを作成します。 GoToWebinarの作成時の設定は、Marketorが使用するものと、GoToWebinarのみが使用するものがあります。

Marketorイベントを作成し、GoToWebセミナーを関連付けると、登録情報と出席情報を共有できるようになります。 GoToWebinarの作成については、『GoToWebinarユーザガイド [](http://docs.marketo.com/display/docs/assets/gotowebinar-user-guide.pdf)』を参照してください。

以下は、Marketoが使用する設定のリストです。

## タイトルと説明 {#title-and-description}

**ウェビナー名** — ウェビナーの名前を入力します。 この名前は、Marketorで表示できます。

**説明** （オプション） — ウェビナーの説明を入力します。 説明はマーケティング担当者に表示できます。

![](assets/image2015-5-28-15-3a1-3a36.png)

## 日付と時刻 {#date-time}

`Enter the following information for your webinar and it will be pulled into Marketo via the`アダプタ。 この情報に変更を加えた場合、変更をMarketerに表示するには、「**イベントアクション****」の下の「ウェビナープロバイダーから更新**」リンクをクリックする必要があります。

**開始日** -開始日を入力します。 これは、Marketoで表示できます。

**開始時刻** -開始時刻を入力します。 これは、Marketoで表示できます。

**終了時間** — 終了時間を入力します。 これは、Marketoで表示できます。

**タイムゾーン** — 該当するタイムゾーンを選択します。 Marketoで表示できます。

**「 —** 」を「 **One Session**」に設定します。

![](assets/image2015-5-28-15-3a7-3a1.png)

>[!NOTE]
>
>マーケティング担当者は、現在、ウェビナーの繰り返しをサポートしていません。 Marketorの各イベントとGoToWebinarのウェビナーの間に、1つのセッションを設定する必要があります。

>[!TIP]
>
>GoToWebinarで設定する追加のフィールドがあり、統合に影響を与えません。 これらのフィールドの詳細については、『GoTo [ウェビナーユーザガイド](http://docs.marketo.com/display/docs/assets/gotowebinar-user-guide.pdf) 』を参照してください。この記事では説明しません。 GoToWebセミナーのヘルプが必要な場合は、その [ヘルプサイトを参照してください](http://support.logmeininc.com/gotowebinar)。

さあ、マーケットに飛び込もう！

1. イベントを選択します。 「 **イベントアクション** 」をクリックし、「 **イベント設定**」を選択します。

   ![](assets/image2015-5-14-14-3a53-3a10.png)

   >[!NOTE]
   >
   >選択するイベントのチャネルタイプは **ウェビナーである必要があります**。

1. 「 **イベント****パートナー** 」リストから「GoToWebinar **** 」を選択します。

   ![](assets/image2015-5-14-14-3a55-3a20.png)

1. アカウントを選択します。

   ![](assets/rtaimage-2.png)

1. ウェビナーを選択します。

   ![](assets/image2015-5-14-14-3a57-3a31.png)

1. 「 **保存**」をクリックします。

   ![](assets/image2015-5-14-14-3a58-3a54.png)

1. 素晴らしい！ 現在は、イベントはGoToWebセミナーによって同期およびスケジュ **ールされ**&#x200B;ます。

   ![](assets/image2015-5-14-15-3a0-3a47.png)

   >[!NOTE]
   >
   >Marketorが送信するフィールドは次のとおりです。名、姓、電子メールアドレス。 これらのフィールドは必須で、空にすることはできません。

   >[!TIP]
   >
   >この一意のURLを確認電子メールに入力するには、電子メールで次のトークンを使用します。 `{{member.webinar url}}`. 確認URLが送信されると、このトークンは、ユーザー固有の確認URLに自動的に解決されます。
   >
   >確認の電子メールを「 **Operational** 」に設定して、登録済みで登録が取り消されている可能性のあるユーザーが確認情報を引き続き受け取るようにします。

   ![](assets/goto-webinar.png)

   >[!CAUTION]
   >
   >確認電子メールを送信する際に、ネストされた電子メールプログラムを使用しないでください。 代わりに、イベントプログラムのスマートキャンペーンを使用します。

   >[!TIP]
   >
   >データがマーケティング担当者に表示されるまで、最大48時間かかる場合があります。 それでも何も表示されない状態が続く場合は、イベントの「 **概要** 」タブにある「イベントの操作」メニューから「ウェビナープロバイダーから **** 更新」を選択します。

ウェビナーにサインアップした人は、「新しいステータス」が「登録済み」に設定されている場合に、プログラムステータスの変更フローステップを通じてウェビナーのプロバイダーにプッシュされます。 その他の状態では、その人を押しのけることはありません。 また、プログラムステータスの変更のフロー手順#1と、電子メールの送信のフロー手順#2を必ず行ってください。

## スケジュールの表示  {#viewing-the-schedule}

[ [プログラムスケジュール表示](http://docs.marketo.com/display/docs/program+schedule+view)]で、イベントのカレンダーエントリをクリックします。 スケジュールは、画面の右側に表示されます。

>[!NOTE]
>
>イベントのスケジュールを変更するには、GoToWebinarでウェビナーを編集する必要があります。

![](assets/image2015-5-14-15-3a3-3a13.png)
