---
description: 手順 1／4 - リソース所有者のパスワード制御接続を使用した Marketo ソリューションのインストール - Marketo ドキュメント - 製品ドキュメント
title: 手順 1／4 - リソース所有者のパスワード制御接続を使用した Marketo ソリューションのインストール
exl-id: aab3bbb8-4e52-4c40-94d1-631af1d63f9f
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 77%

---

# 手順 1／4：リソース所有者のパスワード制御接続を使用した Marketo ソリューションのインストール {#step-1-of-4-install-the-marketo-solution-ropc}

[!DNL Microsoft Dynamics] 365 とMarketoを同期する前に、まず [!DNL Dynamics] にMarketo ソリューションをインストールする必要があります。 **[!DNL Dynamics]の管理者権限が必要です。**

>[!CAUTION]
>
>* 初期同期が完了する前にカスタムエンティティの同期を有効にしないでください。初回同期が完了すると、電子メールで通知されます。
>* [!DNL Dynamics] Sync で Multi-Factor Authentication （MFA）を有効にしている場合、[!DNL Dynamics] がMarketoと正しく同期するには、これを無効にする必要があります。 詳しくは、[Marketo サポート](https://nation.marketo.com/t5/Support/ct-p/Support)にお問い合わせください。

>[!NOTE]
>
>Marketo を CRM に同期した後は、インスタンスを置き換えないと、新しい同期を実行できません。

>[!PREREQUISITES]
>
>[Marketo リード管理ソリューションのダウンロード](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)

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

1. 次に、ソリューション情報ページに戻り、「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/image2015-10-9-14-3a59-3a24.png)

1. 「SDK オプション」のチェックがオンになっていることを確認します。「**[!UICONTROL インポート]**」をクリックします。

   ![](assets/image2015-10-9-15-3a7-3a12.png)

   >[!TIP]
   >
   >インストールプロセスを完了するには、ブラウザーでポップアップを有効にする必要があります。

1. インポートが完了するまで待ちます。ストレッチでもしながらお待ちください。

   ![](assets/image2015-3-11-11-3a34-3a9.png)

1. 「**[!UICONTROL 閉じる]**」をクリックします。

   >[!NOTE]
   >
   >「Marketo Lead Management completed with warning」というメッセージが表示される場合があります。これは十分予期されているものです。

   ![](assets/image2015-3-13-9-3a54-3a39.png)

1. 「Marketo Lead Management」がソリューションのリストに表示されます。

   ![](assets/image2015-3-19-8-3a40-3a38.png)

1. **[!UICONTROL Marketo リード管理]** を選択し、「**[!UICONTROL すべてのカスタマイズを公開]**」をクリックします。

   ![](assets/image2015-3-19-8-3a41-3a21.png)

   お疲れさまでした。インストールが完了しました。

   >[!MORELIKETHIS]
   >
   >[手順 2／4：リソース所有者のパスワード制御接続を使用した Marketo ソリューションの設定](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md){target="_blank"}
