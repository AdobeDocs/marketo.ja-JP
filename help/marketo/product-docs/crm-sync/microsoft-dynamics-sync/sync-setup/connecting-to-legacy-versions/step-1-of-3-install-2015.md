---
unique-page-id: 7504736
description: Microsoft Dynamics 2015 オンプレミス向け Marketo インストール手順 1 / 3 - Marketo ドキュメント - 製品ドキュメント
title: Microsoft Dynamics 2015 オンプレミス向け Marketo インストール手順 1 / 3
exl-id: c9b6d365-15c1-4eff-938c-8433b1fe7f24
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 77%

---

# 手順 1 / 3：Marketo（2015 オンプレミス）の同期ユーザーの設定 {#step-of-configure-sync-user-for-marketo-on-premises-2015}

2015 オンプレミス [!DNL Microsoft Dynamics]Marketoと同期する前に、まず [!DNL Dynamics] にMarketo ソリューションをインストールする必要があります。

>[!NOTE]
>
>Marketo を CRM に同期した後は、新しい CRM を既存の Marketo インスタンスに同期できません。

>[!PREREQUISITES]
>
>[!DNL Microsoft Dynamics] オンプレミスを使用している場合は、[Active Directory フェデレーション サービス ](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) 2.0 以降（ADFS）が構成された [ インターネット接続展開 ](https://msdn.microsoft.com/en-us/library/bb897402.aspx) （IFD）が必要です。 注意：IFD ドキュメントは、リンクをクリックすると自動的にダウンロードされます。
>
>始める前に、[Marketo リード管理ソリューションをダウンロード](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}します。

>[!NOTE]
>
>**Dynamics 管理者権限が必要**&#x200B;です。
>
>この同期を実行するには、CRM 管理者権限が必要です。

1. **[!DNL Dynamics]にログインします。**「**[!UICONTROL Microsoft Dynamics CRM]**」ドロップダウンをクリックし、「**[!UICONTROL 設定]**」を選択します。

   ![](assets/image2015-3-19-8-33-29.png)

1. 「**[!UICONTROL 設定]**」で、「**[!UICONTROL ソリューション]**」を選択します。

   ![](assets/image2015-3-19-8-33-3.png)

1. 「**[!UICONTROL インポート]**」をクリックします。

   ![](assets/image2015-3-19-8-34-8.png)

1. 「**[!UICONTROL 参照]**」をクリックし、[ダウンロード](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)したソリューションを選択します。「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/image2015-3-19-9-20-56.png)

1. [!UICONTROL &#x200B; ソリューション情報 &#x200B;] を表示し、「**[!UICONTROL ソリューションパッケージの詳細を表示]**」をクリックします。

   ![](assets/image2015-11-18-11-12-8.png)

1. すべての詳細を確認したら、「**[!UICONTROL 閉じる]**」をクリックします。

   ![](assets/step6.png)

1. [!UICONTROL &#x200B; ソリューション情報 &#x200B;] ページに戻り、「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/image2015-3-19-9-21-50.png)

1. 「SDK」オプションチェックボックスがオンになっていることを確認します。「**[!UICONTROL インポート]**」をクリックします。

   ![](assets/image2015-3-19-9-19-12.png)

1. インポートが完了するまで待ちます。

   >[!TIP]
   >
   >インストールプロセスを完了するには、ブラウザーでポップアップを有効にする必要があります。

   ![](assets/image2015-3-11-11-34-9.png)

1. 必要に応じて、ログファイルをダウンロードし、「**[!UICONTROL 閉じる]**」をクリックします。

   >[!NOTE]
   >
   >「Marketo Lead Management completed with warning」というメッセージが表示される場合があります。これは十分予期されているものです。

   ![](assets/image2015-3-13-9-54-39.png)

1. Marketo リード管理が、**[!UICONTROL すべてのソリューション]**&#x200B;ページに表示されます。

   ![](assets/image2015-3-19-8-40-38.png)

1. Marketo ソリューションを選択し、「**[!UICONTROL すべてのカスタマイズを公開]**」をクリックします。

   ![](assets/image2015-3-19-8-41-21.png)

   お疲れさまでした。インストールが完了しました。

   >[!CAUTION]
   >
   >Marketo SDK メッセージングプロセスを無効にすると、不完全なインストールになります。

   >[!MORELIKETHIS]
   >
   >[Marketo for [!DNL Microsoft Dynamics] 2015 オンプレミスのインストール手順 2/3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-set-up-2015.md)
