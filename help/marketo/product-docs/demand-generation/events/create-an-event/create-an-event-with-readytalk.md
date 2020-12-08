---
unique-page-id: 2949870
description: ReadyTalk - Marketto Docs — 製品ドキュメントを使用してイベントを作成する
title: ReadyTalkを使用したイベントの作成
translation-type: tm+mt
source-git-commit: c8a77dc84c023e05fbb442f575269aac108ffb29
workflow-type: tm+mt
source-wordcount: '444'
ht-degree: 0%

---


# ReadyTalkを使用したイベントの作成 {#create-an-event-with-readytalk}

>[!PREREQUISITES]
>
>* [LaunchPointサー追加ビスとしてのReadyTalk](/help/marketo/product-docs/administration/additional-integrations/add-readytalk-as-a-launchpoint-service.md)
>* [新しいイベントプログラムの作成](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* 適切な [フロー](http://docs.marketo.com/display/DOCS/Flow+Actions)アクションを設定して、エンゲージメントを追跡する


最初に、ReadyTalkコンファレンスセンターでイベントをセットアップします。 ヘルプが必要な場合は、ReadyTalkリソースセンターを [ご覧ください。](https://www.readytalk.com/resources/readytalk)  登録の種類を選択する場合は、会議の前に **事前登録を選択します**。 会議時に *登録を選択した場合*、Marketorはユーザーの登録済みステータスを取り込ま **ず** 、ウェビナーが終了した後に「出席済み ** 」という個人ステータスを取り込みます。

[電子メールを使用して新規登録を **通知する** ]はオフのままにします。

![](assets/image2015-5-28-21-3a18-3a39.png)

ReadyTalkを使用して確認メールを送信する場合は、説明も追加する必要があります。 完了したら、ReadyTalkでイベントを保存します。

>[!NOTE]
>
>オペレーター支援イベントをスケジュールするには、Conference Centerのホーム画面の左側にある「 **イベントサービスの要求** 」リンクをクリックして、イベントチームとのイベントをスケジュールします。

これで、イベントをMarketoにリンクする準備ができました。

1. イベントを選択し、「 **イベントの操作**」をクリックして、最後に「 **イベントの設定」をクリックします。**

   ![](assets/image2015-5-18-12-3a46-3a47.png)

   >[!NOTE]
   >
   >選択するイベントのチャネルタイプは **ウェビナーにする必要があります。**

1. 「 **イベントパートナー」で** 「ReadyTalk ****」を選択します。

   ![](assets/image2015-5-18-12-3a47-3a59.png)

1. 「 **Login」で、** ReadyTalkログインを選択します。

   ![](assets/image2015-5-18-12-3a48-3a48.png)

1. 「 **イベント**」でリンクするイベントを選択し、「 **保存**」をクリックします。

   ![](assets/image2015-5-18-12-3a51-3a35.png)

   ナイス！ イベントが同期されました。

   >[!NOTE]
   >
   >Marketorが送信するフィールドは次のとおりです。名、姓、電子メールアドレス。

   >[!TIP]
   >
   >この一意のURLを確認電子メールに入力するには、電子メールで次のトークンを使用します。 `{{member.webinar url}}`. 確認URLが送信されると、このトークンは、ユーザー固有の確認URLに自動的に解決されます。
   >
   >確認の電子メールを「運用」に設定し、登録者（登録を取り消された可能性がある人）が確認情報を受け取るようにします。

   ![](assets/readytalk.png)

   >[!CAUTION]
   >
   >確認電子メールを送信する際に、ネストされた電子メールプログラムを使用しないでください。 代わりに、イベントプログラムのスマートキャンペーンを使用します。

   >[!TIP]
   >
   >データがマーケティング担当者に表示されるまで、最大48時間かかる場合があります。 それでも何も表示されない状態が続く場合は、イベントの「 **概要** 」タブにある「イベントの操作」メニューから「ウェビナープロバイダーから **** 更新」を選択します。

## スケジュールの表示  {#viewing-the-schedule}

[ [プログラムスケジュール表示](http://docs.marketo.com/display/docs/program+schedule+view)]で、イベントのカレンダーエントリをクリックします。 画面の右側にスケジュールが表示されます。

![](assets/image2015-5-18-12-9-58.png)

ウェビナーにサインアップした人は、「新しいステータス」が「登録済み」に設定されている場合に、プログラムステータスの変更フローステップを通じてウェビナーのプロバイダーにプッシュされます。 その他の状態では、その人を押しのけることはありません。 また、プログラムステータスの変更のフロー手順#1と、電子メールの送信のフロー手順#2を必ず行ってください。
