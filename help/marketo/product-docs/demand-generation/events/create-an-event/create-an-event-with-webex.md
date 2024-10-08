---
unique-page-id: 2949863
description: Webex を使用したイベントの作成 - Marketo ドキュメント - 製品ドキュメント
title: Webex を使用したイベントの作成
exl-id: 25266a6b-3951-46d1-8700-b36d7086ad2c
feature: Events
source-git-commit: 7edce24c2199a6a2eaa119d3ef77543bbd97999c
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 17%

---

# Webex を使用したイベントの作成 {#create-an-event-with-webex}

Webex でウェビナーを作成したら、イベントをMarketo Engageと同期する必要があります。

>[!PREREQUISITES]
>
>* [Webex を LaunchPoint サービスとして追加](/help/marketo/product-docs/administration/additional-integrations/add-webex-as-a-launchpoint-service.md)
>* [新しいイベントプログラムの作成](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* 適切な[フローアクション](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)を設定して、エンゲージメントをトラック

## ウェビナーのスケジュール設定 {#schedule-your-webinar}

イベントのスケジュールを設定し、[Webex](https://www.webex.com/){target="_blank"} で優先設定を選択します。 Marketoに表示できる情報は、ウェビナー名、開始日/終了日時、タイムゾーン、説明のみです。 Webex ウェビナーに関する追加情報 [ こちらを参照 ](https://help.webex.com/en-us/landing/ld-7srxjs-WebexWebinars/Webex-Webinars){target="_blank"}。

### 基本情報 {#basic-information}

![](assets/create-an-event-with-webex-1.png)

* **トピック**：これはイベント名で、Marketoで表示されます。
* **日時**：開始日/終了日、開始時刻/終了時刻、期間およびタイムゾーンはすべてMarketoで表示できます。
* **最大出席者**：出席者の最大数によって、サポートされる Webex 機能が決まります。
* **参加者向けの Web キャストビュー**：これを確認して、すべての参加者にウェビナーをライブでストリーミングします。
* **パネリスト**：ウェビナーでパネリストになる特定のユーザーを招待します。
* **ウェビナーアジェンダ**：パネリストに送信される招待メールにコンテキストを提供する場合は、この情報を入力します。

### セキュリティ {#security}

![](assets/create-an-event-with-webex-2.png)

* **ウェビナーパスワード**:（任意）このフィールドを使用する場合は、確認メールに必ず含めてください。
* **パネリストのパスワード**:（任意）このフィールドを使用する場合は、ウェビナーのアジェンダに必ず含めてください。
* **アカウントが必要**：出席者を Webex アカウントを持つユーザーのみに制限します。

### オーディオ接続オプション {#audio-connection-options}

![](assets/create-an-event-with-webex-3.png)

* **オーディオ接続タイプ**：ウェビナーの参加者がウェビナーのオーディオ部分にどのように参加するかを選択します。
* **入口と出口のトーン**：ユーザーがウェビナーに参加または離脱したときに表示されるサウンドを選択します（電話によるオーディオ接続が必要です）。
* **パネリストをミュート**：目的のパネリストのミュート設定を選択します。

### 詳細オプション {#advanced-options}

![](assets/create-an-event-with-webex-4.png)

* **自動録画**：ウェビナーを自動的に記録する場合は、これをオンにします。
* **練習セッション**：ウェビナーの開始時に練習セッションを開始するには、これをオンにします。
* **ブレイクアウトセッション**：ブレイクアウトセッションでは、ウェビナーの開始前にパネリストと出席者を事前に割り当てたり、ウェビナー中に参加したりできます。
* **ウェビナーシリーズ**：ウェビナーシリーズに追加すると、公開されているかどうかにかかわらず、ユーザーにウェビナーを表示できます。
* **登録**：出席者は、出席する前に登録してホストの承認を受ける必要があります。
* **メールリマインダー**: ウェビナー開始の 15 分前から 2 日間のメールリマインダーを選択します。
* **ウェビナーオプション**：ウェビナーの参加者が使用できる機能を決定します。
* **参加者権限**：参加者権限によって、ウェビナー参加者が使用できるアクションが決まります。

>[!NOTE]
>
>Marketo と Webex 統合では、Webex からの確認メールの送信をサポートできません。確認メールは Marketo から送信する必要があります。イベントをスケジュール設定したら、イベント情報を Marketo の確認メールにコピーし、そのメールを&#x200B;_オペレーショナル_&#x200B;に設定してください。

## イベントとMarketo Engageの同期 {#sync-your-event-with-marketo-engage}

1. Marketoで、目的のイベントプログラムを見つけて選択します。 **イベントアクション** ドロップダウンで、「**イベント設定**」を選択します。

   ![](assets/create-an-event-with-webex-5.png)

   >[!NOTE]
   >
   >選択するイベントのチャネルタイプは、**ウェビナー**&#x200B;である必要があります。

1. **イベントパートナー** ドロップダウンで、「**Webex ウェビナー**」を選択します。

   ![](assets/create-an-event-with-webex-6.png)

1. **ログイン** ドロップダウンで、Webex のログインを選択します。

   ![](assets/create-an-event-with-webex-7.png)

1. **イベント** ドロップダウンで、Webex イベントを選択します。

   ![](assets/create-an-event-with-webex-8.png)

1. ウェビナーの詳細が入力されます。 「**保存**」をクリックします。

   ![](assets/create-an-event-with-webex-9.png)

これで、Webex イベントがMarketo イベントプログラムと同期されました。 ウェビナーに登録したユーザーは、新しいステータスが「登録済み」に設定されている場合、_プログラムのステータスを変更_ フローステップを通じてウェビナープロバイダーにプッシュされます。 その他のステータスではプッシュされません。_プログラムステータスの変更_ フローステップ#1、_メールを送信_ フローステップ#2 を必ず確認してください。

## 注意事項 {#things-to-note}

* ネストされたメールプログラムを使用して確認メールを送信することは避けます。 代わりに、イベントプログラムのスマートキャンペーンを使用します。

* データがMarketoに表示されるまで、最大 48 時間かかる場合があります。 その間待っても何も表示されない場合は、イベントプログラムの **概要** タブにある **イベントアクション** ドロップダウンの **ウェビナープロバイダーから更新** をクリックします。
