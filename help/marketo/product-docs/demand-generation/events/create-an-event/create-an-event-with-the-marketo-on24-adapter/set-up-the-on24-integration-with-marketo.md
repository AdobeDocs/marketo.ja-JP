---
description: ON24 と Marketo の統合設定 - Marketo ドキュメント - 製品ドキュメント
title: ON24 と Marketo の統合設定
exl-id: 395ffa37-b87d-4eb4-bf9f-72aa96dc819c
feature: Events
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 50%

---

# ON24 と Marketo の統合設定{#set-up-the-on24-integration-with-marketo}

ON24 イベント統合の設定方法を以下に示します。

## API 専用ロールの作成 {#create-an-api-only-role}

1. My Marketo で、「**[!UICONTROL 管理者]**」をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-1.png)

1. [!UICONTROL &#x200B; セキュリティ &#x200B;] の下の **[!UICONTROL ユーザーと役割]** をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-2.png)

1. 「**[!UICONTROL ロール]**」タブをクリックしてから、「**[!UICONTROL 新規ロール]**」をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-3.png)

1. [!UICONTROL &#x200B; 役割名 &#x200B;] を入力します。 **[!UICONTROL Access API]** メニューを開き、「[!UICONTROL &#x200B; 読み取り/書き込みカスタムオブジェクト &#x200B;]」および「[!UICONTROL &#x200B; 読み取り/書き込みユーザー &#x200B;]」を選択します。 「**[!UICONTROL 作成]**」をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-4.png)

## 新規ユーザを作成 {#create-a-new-user}

1. [!UICONTROL &#x200B; ユーザーと役割 &#x200B;] のまま、「**[!UICONTROL ユーザー]** タブをクリックし、「**[!UICONTROL 新規ユーザーを招待]**」をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-5.png)

1. 新規ユーザの情報を入力し、「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-6.png)

1. 作成した [!UICONTROL ON24 API のみ役割（すべてのワークスペース） &#x200B;] 選択します。 「**[!UICONTROL API 専用]**」チェックボックスを選択します。「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-7.png)

1. 「**[!UICONTROL 送信]**」をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-8.png)

>[!NOTE]
>
>API 専用ユーザの場合、招待は必要ありません。

## ON24 接続の設定 {#set-up-on24-connection}

1. 「[!UICONTROL &#x200B; 管理者 &#x200B;]」セクションで、「**[!UICONTROL LaunchPoint]**」をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-9.png)

1. 「**[!UICONTROL 新規]**」をクリックしてから、「**[!UICONTROL 新規サービス]**」をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-10.png)

1. [!UICONTROL &#x200B; 表示名 &#x200B;] を選択します。 「**[!UICONTROL サービス]**」ドロップダウンをクリックし、「**[!UICONTROL カスタム]**」を選択します。[!UICONTROL &#x200B; 説明 &#x200B;] を入力します。 [!UICONTROL API のみユーザー &#x200B;] ドロップダウンをクリックし、作成したユーザーを選択します [ 上記の手順で ](#create-a-new-user)。 「**[!UICONTROL 作成]**」をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-11.png)

1. 作成したばかりのカスタム [!DNL LaunchPoint] サービスを見つけて、「[!UICONTROL &#x200B; 詳細を表示 &#x200B;]」をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-12.png)

1. [!UICONTROL &#x200B; クライアント ID] をハイライト表示し、右クリックしてコピーし、保存します（後で必要になります）。 [!UICONTROL &#x200B; クライアント秘密鍵 &#x200B;] に対して繰り返します。

   ![](assets/set-up-the-on24-integration-with-marketo-13.png)

1. 左側のツリーで、「**[!UICONTROL Web サービス]**」をクリックします。

   ![](assets/set-up-the-on24-integration-with-marketo-14.png)

1. 「[!UICONTROL REST API]」の下で、[!UICONTROL ID] の最初の部分（.com の「m」まで）をハイライト表示し、右クリックしてコピーして保存します。

   ![](assets/set-up-the-on24-integration-with-marketo-15.png)

1. 保存したクライアント ID、クライアント秘密鍵および ID を使用して、ON24 アカウントに移動します。残りの手順はそこで実行します。[ON24 ドキュメント](https://support.on24.com/hc/ja-jp/articles/21420762650523-Data-Integration-Setup-Instructions-When-Using-Marketo-Registration-Option-1){target="_blank"}を参照してください。
