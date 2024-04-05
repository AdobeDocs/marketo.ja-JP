---
unique-page-id: 2950682
description: プログラムチャネルの作成 - Marketo ドキュメント - 製品ドキュメント
title: プログラムチャネルの作成
exl-id: 7b4e15db-c221-45a9-9588-99eb2510cde7
feature: Tags
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: ht
source-wordcount: '428'
ht-degree: 100%

---

# プログラムチャネルの作成 {#create-a-program-channel}

プログラムは、特定のマーケティング施策の 1 つです。チャネルは、ウェビナー、スポンサーシップ、オンライン広告などの配信メカニズムを意図しています。

>[!NOTE]
>
>**管理者権限が必要**

>[!NOTE]
>
>Marketo で最も重要な要素、[プログラム](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)について詳しく説明します。

1. 「**[!UICONTROL 管理者]**」領域に移動します。

   ![](assets/create-a-program-channel-1.png)

1. 「**[!UICONTROL タグ]**」をクリックします。

   ![](assets/create-a-program-channel-2.png)

   >[!NOTE]
   >
   >なぜタグを使用するのでしょうか。チャネルは他のタグと同様に、プログラムを記述する方法です。チャネルには特別な追加機能があるだけです。

1. [!UICONTROL チャネル]の横の&#x200B;**+**&#x200B;記号をクリックして、既存のチャネルを展開して表示します。

   ![](assets/create-a-program-channel-3.png)

1. 「**[!UICONTROL 新規作成]**」で「**[!UICONTROL 新規チャネル]**」をクリックします。

   ![](assets/create-a-program-channel-4.png)

   >[!NOTE]
   >
   >**例**
   >
   >チャネル：ビルボード
   >
   >* 適用先：デフォルト
   >* 進行状況：メンバー、エンゲージ済み（不確かな場合は、これらで十分です）
   >* 成功：エンゲージ済み
   >
   >チャネル：パーティ
   >
   >* 適用先：イベント
   >* 進行状況：招待済み、登録済み、不参加、出席済み
   >* 成功：出席済み
   >
   >既存チャネルの進行状況を確認して、使用方法を確認してください。

1. パーティチャネルの例に進みます。新しい&#x200B;**チャネル**&#x200B;に名前を付けて、適用するプログラムタイプを選択します。

   ![](assets/create-a-program-channel-5.png)

   >[!NOTE]
   >
   >何に適用すればいいのでしょうか。プログラムには、いくつかのタイプがあります。チャネルを適切なタイプに合わせます。不確かな場合は、「**[!UICONTROL デフォルト]**」を選択します。

   >[!NOTE]
   >
   >「[!UICONTROL ウェビナーのあるイベント]」を使用する場合、システムマッピングは（ウェビナー統合の要件に応じて）ロックされ、編集できなくなります。

1. 最初の 2 つのプログラムのステータス名を入力し、「**[!UICONTROL ステップを追加]**」をクリックします。

   ![](assets/create-a-program-channel-6.png)

1. 別のプログラム&#x200B;**[!UICONTROL ステータス]**&#x200B;と&#x200B;**[!UICONTROL 手順]**&#x200B;番号を入力し、「**[!UICONTROL ステップを追加]**」をクリックします。

   ![](assets/create-a-program-channel-7.png)

   >[!TIP]
   >
   >**[!UICONTROL 手順]**&#x200B;番号は、プログラムステータスの並べ替えに使用されます。人物は、このような進行ステップを逆行できないことに注意してください。より大きいまたは等しいステータスにのみ変更できます。ステータスが進行と異なり、前後に切り替わる場合は、等しい値を使用します。

1. 最後のプログラム&#x200B;**[!UICONTROL ステータス]**&#x200B;と&#x200B;**[!UICONTROL 手順]**&#x200B;番号を入力します。

   ![](assets/create-a-program-channel-8.png)

   >[!NOTE]
   >
   >タイプ「[!UICONTROL イベント]」を使用する場合、登録済み、待ちリスト、出席済みステータスのシステムマッピングが必要です。したがって、これらのステータスを非表示にできません。

1. **[!UICONTROL 登録済み]**&#x200B;用に、**[!UICONTROL モバイルのチェックインステータス]**&#x200B;を選択します。

   ![](assets/create-a-program-channel-9.png)

1. **[!UICONTROL 出席済み]**&#x200B;用に、**[!UICONTROL モバイルのチェックインステータス]**&#x200B;を選択します。

   ![](assets/create-a-program-channel-10.png)

   >[!NOTE]
   >
   >「**[!UICONTROL モバイルチェックインステータス]**」オプションは、チャネルがイベントプログラムに対して使用される場合にのみ使用できます。

   >[!NOTE]
   >
   >**[!UICONTROL 登録済み]**&#x200B;および&#x200B;**[!UICONTROL 出席済み]**&#x200B;の&#x200B;**[!UICONTROL モバイルのチェックインステータス]**&#x200B;を持つ人物のみが、[モバイルチェックインアプリ](/help/marketo/product-docs/core-marketo-concepts/mobile-apps/event-check-in/event-check-in-overview.md)で表示されます。

   >[!TIP]
   >
   >モバイルチェックインアプリで新しいユーザーを作成すると、イベントプログラムで「登録済み」に設定されます。人物がアプリのイベントにチェックインされると、イベントプログラムで「出席済み」に設定されます。

1. 「**[!UICONTROL 成功]**」プログラムステータスを選択し、「**[!UICONTROL 作成]**」をクリックします。

   ![](assets/create-a-program-channel-11.png)

   これで完了です。このタイプの新しいプログラムを作成する場合、この新しいチャネルは選択肢の 1 つになります。
