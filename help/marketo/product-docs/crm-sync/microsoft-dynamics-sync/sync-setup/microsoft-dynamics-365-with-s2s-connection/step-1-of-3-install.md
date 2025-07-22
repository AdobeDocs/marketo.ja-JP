---
description: 手順 1／3 - サーバー間接続を使用した Marketo ソリューションのインストール - Marketo ドキュメント - 製品ドキュメント
title: 手順 1／3 - サーバー間接続を使用した Marketo ソリューションのインストール
exl-id: bf6f87c1-5ba5-490b-bcce-365120af3730
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 78%

---

# 手順 1／3：サーバー間接続を使用した Marketo ソリューションのインストール {#step-1-of-3-install-the-marketo-solution-s2s}

[!DNL Microsoft Dynamics 365] とMarketoを同期する前に、まず [!DNL Dynamics] にMarketo ソリューションをインストールする必要があります。 **[!DNL Dynamics]の管理者権限が必要です。**

>[!CAUTION]
>
>初期同期が完了する前にカスタムエンティティの同期を有効にしないでください。初回同期が完了すると、電子メールで通知されます。

>[!NOTE]
>
>Marketo を CRM に同期した後は、インスタンスを置き換えないと、新しい同期を実行できません。

>[!PREREQUISITES]
>
>[Marketo リード管理ソリューションのダウンロード](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}

1. **[[!DNL Microsoft Office 365]](https://login.microsoftonline.com/)** にログインします。

   ![](assets/image2015-3-16-15-3a58-3a55.png)

1. ![](assets/image2015-3-16-16-3a1-3a13.png) メニューをクリックして、「**[!UICONTROL CRM]**」を選択します。

   ![](assets/image2015-3-16-16-3a0-3a10.png)

1. ![](assets/image2015-5-13-10-3a5-3a8.png) メニューをクリックします。ドロップダウンメニューで、**[!UICONTROL 設定]**／**[!UICONTROL ソリューション]**&#x200B;を選択します。

   ![](assets/image2015-5-13-10-3a4-3a1.png)

1. 「**[!UICONTROL インポート]**」をクリックします。

   ![](assets/image2015-3-19-8-3a34-3a8.png)

1. **[!UICONTROL ファイルを選択]** をクリックします。 [ダウンロードした](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) Marketo リード管理ソリューションを選択します。「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/image2015-10-9-14-3a44-3a14.png)

1. ソリューション情報を表示し、「**[!UICONTROL ソリューションパッケージ詳細を表示]**」をクリックします。

   ![](assets/image2015-10-9-15-3a4-3a16.png)

1. すべての詳細を確認したら、「**[!UICONTROL 閉じる]**」をクリックします。

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. [!UICONTROL  ソリューション情報 ] ページに戻り、「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/image2015-10-9-14-3a59-3a24.png)

1. 「SDK」オプションチェックボックスがオンになっていることを確認します。「**[!UICONTROL インポート]**」をクリックします。

   ![](assets/image2015-10-9-15-3a7-3a12.png)

   >[!TIP]
   >
   >インストールプロセスを完了するには、ブラウザーでポップアップを有効にする必要があります。

1. インポートが完了するまで待ちます。

   ![](assets/image2015-3-11-11-3a34-3a9.png)

1. 「**[!UICONTROL 閉じる]**」をクリックします。

   >[!NOTE]
   >
   >「Marketo Lead Management completed with warning」というメッセージが表示される場合があります。これは十分予期されているものです。

   ![](assets/image2015-3-13-9-3a54-3a39.png)

1. [!UICONTROL Marketoのリード管理 ] がソリューションのリストに表示されます。

   ![](assets/image2015-3-19-8-3a40-3a38.png)

1. **[!UICONTROL Marketo リード管理]** を選択し、「**[!UICONTROL すべてのカスタマイズを公開]**」をクリックします。

   ![](assets/image2015-3-19-8-3a41-3a21.png)

   完成です。インストールが完了しました。

   >[!MORELIKETHIS]
   >
   >[手順 2／3：S2S 接続を使用した Marketo ソリューションのセットアップ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up.md){target="_blank"}
