---
unique-page-id: 2949865
description: Adobe Connectとのイベントの作成 — Marketto Docs — 製品ドキュメント
title: Adobe Connectとのイベントの作成
translation-type: tm+mt
source-git-commit: c8a77dc84c023e05fbb442f575269aac108ffb29
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 0%

---


# Adobe Connectとのイベントの作成{#create-an-event-with-adobe-connect}

Adobe Connectとの同期により、Marketor内でウェビナーの登録と出欠の管理が可能になり、エンゲージメントの追跡が行われなくなります。

>[!PREREQUISITES]
>
>* [Adobe Connectとマーケットのリンク](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
>* [新しいイベントプログラムの作成](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)


まず、Adobe Connectで会議またはセミナーを作成済みであることを確認してください。 ヘルプが必要な場合は、『[Adobe Connectユーザガイド](http://help.adobe.com/en_US/connect/9.0/using/index.html)』を参照してください。 Adobe Connectで作成する会議とセミナーは、Marketoで資格情報を入力したときに指定したフォルダーの下に作成する必要があります。 会議やセミナーを作成した後、確認用の電子メールやICSファイルで使用する、関連するロジスティック情報（電話番号など）をメモしておきます。

>[!NOTE]
>
>現時点では、Adobe Connectオンサイトを&#x200B;**サポートしていません。**

1. 新しいイベントのホームで、「**イベントアクション**」を選択し、「**イベント設定**」を選択します。

   ![](assets/image2015-1-30-15-3a34-3a28.png)

   >[!NOTE]
   >
   >ドロップダウンに&#x200B;**イベント設定**&#x200B;が表示されない場合は、イベントのチャネルーで、「適用先」で「ウェビナー&#x200B;**」が選択された**&#x200B;イベントがあることを確認してください。

1. **イベントパートナー**&#x200B;の下で、**Adobe Connect**&#x200B;を選択します。

   ![](assets/event-settings-adobe-connect.png)

1. **ログイン** IDを選択し、**イベント**&#x200B;を選択します。

   ![](assets/event-settings-select-event-adobe-connect.png)

1. 「**保存**」をクリックします。

   ![](assets/event-settings-overview.png)

   ナイス！ これで、Adobe ConnectイベントはMarketoイベントと同期されます。

   >[!NOTE]
   >
   >Marketorが送信するフィールドは次のとおりです。名、姓、電子メールアドレス。

   >[!TIP]
   >
   >ユーザー固有のURLを電子メールに挿入するには、次のトークンを使用します。`{{member.webinar url}}`. 電子メールが送信されると、このトークンは、Adobe Connectからのユーザー固有の確認URLを自動的に解決します。
   >
   >確認の電子メールを&#x200B;**操作**&#x200B;に設定し、登録済みで登録を取り消している可能性のあるユーザーが、確認情報を引き続き受け取るようにします。

   ![](assets/adobe.png)

   >[!CAUTION]
   >
   >確認電子メールを送信する際に、ネストされた電子メールプログラムを使用しないでください。 代わりに、イベントプログラムのスマートキャンペーンを使用します。

   >[!TIP]
   >
   >データがマーケティング担当者に表示されるまで、最大48時間かかる場合があります。 それでも何も表示されない状態が続くまで待った後で、イベントの「概要」タブにある「イベントの操作」メニューから「ウェビナープロバイダーから更新」**を選択します。**

   >[!MORELIKETHIS]
   >
   > * [LaunchPointサ追加ービスとしてのAdobe Connect](../../../../product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
   > * [イベントチャネルの編集](../../../../product-docs/demand-generation/events/understanding-events/edit-an-event-channel.md)


ウェビナーにサインアップした人は、「新しいステータス」が「登録済み」に設定されている場合に、プログラムステータスの変更フローステップを通じてウェビナーのプロバイダーにプッシュされます。 その他の状態では、その人を押しのけることはありません。 また、プログラムステータスの変更のフロー手順#1と、電子メールの送信のフロー手順#2を必ず行ってください。
