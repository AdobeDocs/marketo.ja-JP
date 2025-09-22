---
description: ON24 と Marketo の統合設定 - Marketo ドキュメント - 製品ドキュメント
title: ON24 と Marketo の統合設定
exl-id: 395ffa37-b87d-4eb4-bf9f-72aa96dc819c
feature: Events
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 100%

---

# ON24 と Marketo の統合設定{#set-up-the-on24-integration-with-marketo}

ON24 イベント統合の設定方法を以下に示します。

## API 専用ロールの作成 {#create-an-api-only-role}

1. My Marketo で、「**[!UICONTROL 管理者]**」をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-1.png)

1. 「[!UICONTROL セキュリティ]」で「**[!UICONTROL ユーザとロール]**」をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-2.png)

1. 「**[!UICONTROL ロール]**」タブをクリックしてから、「**[!UICONTROL 新規ロール]**」をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-3.png)

1. [!UICONTROL ロール名]を入力します。**[!UICONTROL Access API]** メニューを開き、「[!UICONTROL 読み取り／書き込みカスタムオブジェクト]」および「[!UICONTROL 読み取り／書き込み担当者]」を選択します。「**[!UICONTROL 作成]**」をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-4.png)

## 新規ユーザを作成 {#create-a-new-user}

1. 「[!UICONTROL ユーザ＆ロール]」で、「**[!UICONTROL ユーザ]**」タブをクリックし、「**[!UICONTROL 新規ユーザを招待]**」をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-5.png)

1. 新規ユーザの情報を入力し、「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-6.png)

1. 作成した [!UICONTROL ON24 API 専用ロール（すべてのワークスペース）]を選択します。「**[!UICONTROL API 専用]**」チェックボックスを選択します。「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-7.png)

1. 「**[!UICONTROL 送信]**」をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-8.png)

>[!NOTE]
>
>API 専用ユーザの場合、招待は必要ありません。

## ON24 接続の設定 {#set-up-on24-connection}

1. 「[!UICONTROL 管理者]」セクションで、「**[!UICONTROL LaunchPoint]**」をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-9.png)

1. 「**[!UICONTROL 新規]**」をクリックしてから、「**[!UICONTROL 新規サービス]**」をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-10.png)

1. [!UICONTROL 表示名]を選択します。「**[!UICONTROL サービス]**」ドロップダウンをクリックし、「**[!UICONTROL カスタム]**」を選択します。[!UICONTROL 説明]を入力します。[!UICONTROL API 専用ユーザ]ドロップダウンをクリックし、[上記の手順](#create-a-new-user)で作成したユーザを選択します。「**[!UICONTROL 作成]**」をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-11.png)

1. 作成したカスタム [!DNL LaunchPoint] サービスを探し、「[!UICONTROL 詳細を表示]」をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-12.png)

1. [!UICONTROL クライアント ID] をハイライト表示し、右クリックしてコピーし、保存します（後で必要になります）。[!UICONTROL クライアント秘密鍵]に対して繰り返します。

   ![](assets/set-up-the-on24-integration-with-marketo-13.png)

1. 左側のツリーで、「**[!UICONTROL web サービス]**」をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-14.png)

1. 「[!UICONTROL REST API]」で、[!UICONTROL ID] の最初の部分（.com の「m」まで）をハイライト表示、右クリック、コピーおよび保存します。

   ![](assets/set-up-the-on24-integration-with-marketo-15.png)

1. 保存したクライアント ID、クライアント秘密鍵および ID を使用して、ON24 アカウントに移動します。残りの手順はそこで実行します。[ON24 ドキュメント](https://support.on24.com/hc/ja-jp/articles/21420762650523-Data-Integration-Setup-Instructions-When-Using-Marketo-Registration-Option-1){target="_blank"}を参照してください。
