---
unique-page-id: 2949865
description: Adobe Connectとのイベントの作成 —Marketoドキュメント — 製品ドキュメント
title: Adobe Connectとのイベントの作成
exl-id: 196b1640-9cfd-4485-9bc4-e907d3ac1f16
translation-type: tm+mt
source-git-commit: d81a4a3caa12c5ec642afadf9328b3825bde6fed
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# Adobe Connectとのイベントの作成{#create-an-event-with-adobe-connect}

Adobe Connectとの同期により、Marketo内でのウェビナーの登録と出欠の管理が可能になり、エンゲージメントが追跡されないようになります。

>[!PREREQUISITES]
>
>* [Adobe ConnectとMarketoを結ぶ](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
>* [新しいイベントプログラムの作成](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)


まず、Adobe Connectで会議またはセミナーを作成済みであることを確認してください。 ヘルプが必要な場合は、『[Adobe Connectユーザガイド](https://help.adobe.com/en_US/connect/9.0/using/index.html)』を参照してください。

Adobe Connectで作成するミーティングとセミナーは、Marketoで資格情報を入力したときに指定したフォルダーの下に作成する必要があります。 会議やセミナーを作成した後、確認用の電子メールやICSファイルで使用する、関連するロジスティック情報（電話番号など）をメモしておきます。

>[!CAUTION]
>
>イベントホストは必ずアプリ内から参加し、出席者に送信されるリンクを介して&#x200B;****&#x200B;に参加しないでください。

>[!NOTE]
>
>現時点では、Adobe Connectオンサイトをサポートしていません。

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

   ナイス！ Adobe Connectイベントは、Marketoイベントと同期されました。

   >[!NOTE]
   >
   >Marketoが送り込むフィールドは次のとおりです。名、姓、電子メールアドレス。

   >[!TIP]
   >
   >ユーザー固有のURLを電子メールに挿入するには、次のトークンを使用します。`{{member.webinar url}}`. 電子メールが送信されると、このトークンは、Adobe Connectからのユーザー固有の確認URLを自動的に解決します。
   >
   >確認の電子メールを&#x200B;**操作**&#x200B;に設定し、登録済みで登録を取り消している可能性のあるユーザーが、確認情報を引き続き受け取るようにします。

   ウェビナーにサインアップした人は、「新しいステータス」が「登録済み」に設定されている場合に、プログラムステータスの変更フローステップを通じてウェビナーのプロバイダーにプッシュされます。 その他の状態では、その人を押しのけることはありません。 また、プログラムステータスの変更のフロー手順#1と、電子メールの送信のフロー手順#2を必ず行ってください。

   ![](assets/adobe.png)

   >[!CAUTION]
   >
   >確認電子メールを送信する際に、ネストされた電子メールプログラムを使用しないでください。 代わりに、イベントプログラムのスマートキャンペーンを使用します。

   >[!TIP]
   >
   >データがMarketoに表示されるまで、最大48時間かかる場合があります。 それでも何も表示されない状態が続くまで待った後で、イベントの「概要」タブにある「イベントの操作」メニューから「ウェビナープロバイダーから更新」**を選択します。**

   >[!MORELIKETHIS]
   >
   >* [LaunchPointサ追加ービスとしてのAdobe Connect](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
   >* [イベントチャネルの編集](/help/marketo/product-docs/demand-generation/events/understanding-events/edit-an-event-channel.md)

