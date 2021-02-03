---
unique-page-id: 2949870
description: ReadyTalk - Marketto Docs — 製品ドキュメントを使用してイベントを作成する
title: ReadyTalkを使用したイベントの作成
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 0%

---


# ReadyTalk {#create-an-event-with-readytalk}でイベントを作成

>[!PREREQUISITES]
>
>* [LaunchPointサー追加ビスとしてのReadyTalk](/help/marketo/product-docs/administration/additional-integrations/add-readytalk-as-a-launchpoint-service.md)
>* [新しいイベントプログラムの作成](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* 適切な[フローアクション](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)を設定して、エンゲージメントを追跡します。


最初に、ReadyTalkコンファレンスセンターでイベントをセットアップします。 ヘルプが必要な場合は、[ReadyTalkリソースセンター](https://www.readytalk.com/resources/readytalk)をご覧ください。 登録の種類を選択する場合は、会議&#x200B;**の前に**&#x200B;事前登録を選択します。 _の会議時に_&#x200B;登録を選択した場合、マーケット氏は&#x200B;****&#x200B;自分の従業員の登録済みステータスを&#x200B;_締めくくりません。また、ウェビナーが終了した後は_&#x200B;出席済みの人のステータスのみを引き寄せます。

**電子メール**&#x200B;を使用して新規登録を通知しないでください。

![](assets/image2015-5-28-21-3a18-3a39.png)

ReadyTalkを使用して確認メールを送信する場合は、説明も追加する必要があります。 完了したら、ReadyTalkでイベントを保存します。

>[!NOTE]
>
>オペレーター支援イベントをスケジュールするには、Conference Centerのホーム画面の左側にある&#x200B;**イベントサービスの要請**&#x200B;リンクをクリックして、イベントチームとのイベントをスケジュールします。

これで、イベントをMarketoにリンクする準備ができました。

1. イベントーを選択し、「**イベントアクション**」をクリックし、最後に「**イベント設定**」をクリックします。

   ![](assets/image2015-5-18-12-3a46-3a47.png)

   >[!NOTE]
   >
   >選択するイベントのチャネルの種類は、**ウェビナーである必要があります。**

1. **イベントパートナーの下で、****ReadyTalk**&#x200B;を選択します。

   ![](assets/image2015-5-18-12-3a47-3a59.png)

1. 「**ログイン」で、** ReadyTalkログインを選択します。

   ![](assets/image2015-5-18-12-3a48-3a48.png)

1. **イベント**&#x200B;の下で、リンクするイベントを選択し、「**保存**」をクリックします。

   ![](assets/image2015-5-18-12-3a51-3a35.png)

   ナイス！ イベントが同期されました。

   >[!NOTE]
   >
   >Marketorが送信するフィールドは次のとおりです。名、姓、電子メールアドレス。

   >[!TIP]
   >
   >この一意のURLを確認電子メールに入力するには、電子メールで次のトークンを使用します。`{{member.webinar url}}`. 確認URLが送信されると、このトークンは、ユーザー固有の確認URLに自動的に解決されます。
   >
   >確認の電子メールを「運用」に設定し、登録者（登録を取り消された可能性がある人）が確認情報を受け取るようにします。

   ![](assets/readytalk.png)

   >[!CAUTION]
   >
   >確認電子メールを送信する際に、ネストされた電子メールプログラムを使用しないでください。 代わりに、イベントプログラムのスマートキャンペーンを使用します。

   >[!TIP]
   >
   >データがマーケティング担当者に表示されるまで、最大48時間かかる場合があります。 それでも何も表示されない状態が続くのを待った後で、イベントーの&#x200B;**概要**&#x200B;タブにあるイベントの操作メニューから、「ウェビナープロバイダーから更新&#x200B;**」を選択します。**

## スケジュールの表示{#viewing-the-schedule}

プログラムスケジュール表示で、イベントのカレンダーエントリをクリックします。 画面の右側にスケジュールが表示されます。

![](assets/image2015-5-18-12-9-58.png)

ウェビナーにサインアップした人は、「新しいステータス」が「登録済み」に設定されている場合に、プログラムステータスの変更フローステップを通じてウェビナーのプロバイダーにプッシュされます。 その他の状態では、その人を押しのけることはありません。 また、プログラムステータスの変更のフロー手順#1と、電子メールの送信のフロー手順#2を必ず行ってください。
