---
description: Marketoとの ON24 統合の設定 – Marketo ドキュメント – 製品ドキュメント
title: Marketo との ON24 統合の設定
exl-id: 395ffa37-b87d-4eb4-bf9f-72aa96dc819c
feature: Events
source-git-commit: e3f61755dccd9bea1378a429fc428b440fc3ecb4
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 16%

---

# Marketo との ON24 統合の設定{#set-up-the-on24-integration-with-marketo}

ON24 イベント統合の設定方法を以下に示します。

## API のみの役割の作成 {#create-an-api-only-role}

1. My Marketo で、「**管理者**」をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-1.png)

1. 「セキュリティ」で「**ユーザーと役割**」をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-2.png)

1. 「**役割**」タブをクリックしてから、「**新規の役割**」をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-3.png)

1. 役割名を入力します。 **Access API** メニューを開き、「Read-Write Custom Object」および「Read-Write Person」を選択します。 「**作成**」をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-4.png)

## ユーザーを新規作成する {#create-a-new-user}

1. 「ユーザーと役割」のまま、「**ユーザー**」タブをクリックし、「**新規ユーザーを招待**」をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-5.png)

1. 新しいユーザーの情報を入力し、「**次へ**」をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-6.png)

1. 作成した ON24 API のみの役割を選択します。 「**API のみ**」チェックボックスを選択します。 「**次へ**」をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-7.png)

1. 「**送信**」をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-8.png)

>[!NOTE]
>
>API のみのユーザーの場合、招待は必要ありません。

## ON24 接続の設定 {#set-up-on24-connection}

1. 「管理者」セクションで、「**LaunchPoint**」をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-9.png)

1. **新規** / **新しいサービス** をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-10.png)

1. 表示名を選択します。 **サービス** ドロップダウンをクリックし、「**カスタム**」を選択します。 説明を入力します。 API のみのユーザーのドロップダウンをクリックし、作成したユーザーを選択します [ 上記の手順で ](#create-a-new-user)。 「**作成**」をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-11.png)

1. 作成したばかりのカスタム LaunchPoint サービスを見つけて、「詳細を表示」をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-12.png)

1. クライアント ID をハイライト表示し、右クリックしてコピーし、保存します（後で必要になります）。 クライアント秘密鍵に対して繰り返します。

   ![](assets/set-up-the-on24-integration-with-marketo-13.png)

1. 左側のツリーで、[Web サービス ] をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-14.png)

1. 「REST API」の下で、ID の最初の部分（.com の「m」まで）をハイライト表示、右クリック、コピーおよび保存します。

   ![](assets/set-up-the-on24-integration-with-marketo-15.png)

1. 保存したクライアント ID、クライアントシークレットおよび ID を使用して、ON24 アカウントに移動します。 残りの手順については、[ON24 ドキュメント ](https://support.on24.com/hc/en-us/articles/21420762650523-Data-Integration-Setup-Instructions-When-Using-Marketo-Registration-Option-1){target="_blank"} を参照してください。
