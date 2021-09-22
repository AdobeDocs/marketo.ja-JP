---
unique-page-id: 2949865
description: Adobe Connect を使用したイベントの作成 - Marketo ドキュメント - 製品ドキュメント
title: Adobe Connect を使用したイベントの作成
exl-id: 196b1640-9cfd-4485-9bc4-e907d3ac1f16
source-git-commit: d81a4a3caa12c5ec642afadf9328b3825bde6fed
workflow-type: ht
source-wordcount: '419'
ht-degree: 100%

---

# Adobe Connect を使用したイベントの作成 {#create-an-event-with-adobe-connect}

Adobe Connect と同期すると、ウェビナーへの登録と参加を Marketo 内部で管理できるようになるので、リードの管理を見逃す心配がありません。

>[!PREREQUISITES]
>
>* [Adobe Connect と Marketo のリンク](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
>* [新しいイベントプログラムの作成](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)


まず、Adobe Connect でミーティングまたはセミナーを作成していることを確認します。ヘルプが必要な場合は、[Adobe Connect ユーザーガイド](https://helpx.adobe.com/jp/adobe-connect/using/user-guide.html)をご覧ください。

Adobe Connect で作成するミーティングとセミナーは、Marketo で認証情報を入力するときに指定するフォルダーに作成する必要があります。ミーティングとセミナーを作成したら、確認メールや ICS ファイルで使用する関連の連絡情報（電話番号など）を書きとめておきます。

>[!CAUTION]
>
>イベントホストは、出席者に送信される&#x200B;**リンク経由ではなく**、アプリ内から参加する必要があります。

>[!NOTE]
>
>現時点では、Adobe Connect On-Site はサポートされていません。

1. 新しいイベントのホームで、「**イベントアクション**」を選択し、「**イベント設定**」を選択します。

   ![](assets/image2015-1-30-15-3a34-3a28.png)

   >[!NOTE]
   >
   >ドロップダウンに「**イベント設定**」が表示されない場合は、イベントのチャネルで「適用先」で「**Webinar を含むイベント**」が選択されていることを確認します。

1. 「**イベントパートナー**」で、「**Adobe Connect**」を選択します。

   ![](assets/event-settings-adobe-connect.png)

1. **ログイン** ID を選択し、**イベント**&#x200B;を選択します。

   ![](assets/event-settings-select-event-adobe-connect.png)

1. 「**保存**」をクリックします。

   ![](assets/event-settings-overview.png)

   作業は以上です。これで、Adobe Connect イベントが Marketo イベントと同期されました。

   >[!NOTE]
   >
   >Marketo が送信するフィールドは、姓、名、メールアドレスです。

   >[!TIP]
   >
   >個人の一意の URL をメールに挿入するには、`{{member.webinar url}}` というトークンを使用します。メールが送信されると、このトークンは、Adobe Connect からの各リード固有の確認 URL に自動的に変換されます
   >
   >配信停止やマーケティング中断したリードにも届くように、確認メールは&#x200B;**オペレーショナル**&#x200B;メールに設定してください。

   ウェビナーに新規登録したリードは、新規ステータスが「登録」に設定されたときに、プログラムステータスを変更フローステップによってウェビナープロバイダーにプッシュされます。その他のステータスではプッシュされません。また、プログラムステータスを変更フローステップ #1 とメールを送信フローステップ #2 を必ず設定してください。

   ![](assets/adobe.png)

   >[!CAUTION]
   >
   >ネストされたメールプログラムを使用して確認メールを送信しないでください。代わりに、上に示しているように、イベントプログラムのスマートキャンペーンを使用します。

   >[!TIP]
   >
   >Marketo にデータが表示されるまでには、最大 48 時間かかる場合があります。48 時間待っても何も表示されない場合は、イベントの「**概要**」タブの「イベントアクション」メニューから「ウェビナープロバイダーから更新」を選択してください。

   >[!MORELIKETHIS]
   >
   >* [Adobe Connect を LaunchPoint サービスとして追加](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
   >* [イベントチャネルの編集](/help/marketo/product-docs/demand-generation/events/understanding-events/edit-an-event-channel.md)

