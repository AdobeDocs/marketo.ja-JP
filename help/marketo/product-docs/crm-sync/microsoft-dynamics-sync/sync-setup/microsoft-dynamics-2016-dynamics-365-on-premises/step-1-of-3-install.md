---
description: Microsoft Dynamics 2016／Dynamics 365 オンプレミス向け Marketo インストール手順 1 / 3 - Marketo ドキュメント - 製品ドキュメント
title: Microsoft Dynamics 2016／Dynamics 365 オンプレミス向け Marketo インストール手順 1 / 3
exl-id: 0a494ae7-87da-4ff9-bb47-990b957533e1
source-git-commit: 3fb93520a653109845c3b40aba20304c6163214f
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 100%

---

# 手順 1 / 3：Marketo（2016 オンプレミス／Dynamics 365 オンプレミス）の同期ユーザーの設定 {#step-of-configure-sync-user-for-marketo-on-premises-2016}

Microsoft Dynamics 2016 オンプレミス／Dynamics 365 と Marketo を同期する前に、Dynamics に Marketo ソリューションをインストールする必要があります。

>[!NOTE]
>
>Marketo を CRM に同期した後は、新しい CRM を既存の Marketo インスタンスに同期できません。

>[!PREREQUISITES]
>
>Microsoft Dynamics オンプレミスを使用している場合は、[Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0 以降（ADFS）が設定された、[インターネットに接続する展開](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701)（IFD）が構成されている必要があります。注意：IFD ドキュメントは、リンクをクリックすると自動的にダウンロードされます。
>
>始める前に、[Marketo リード管理ソリューションをダウンロード](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)します。

>[!NOTE]
>
>**Dynamics 管理権限が必要。**
>
>この同期を実行するには、CRM 管理者権限が必要です。

1. **Dynamics にログインします。**「**Microsoft Dynamics CRM**」ドロップダウンをクリックし、「**設定**」を選択します。

   ![](assets/image2015-3-19-8-33-29.png)

1. 「**設定**」で、「**ソリューション**」を選択します。

   ![](assets/image2015-3-19-8-33-3.png)

1. 「**インポート**」をクリックします。

   ![](assets/image2015-3-19-8-34-8.png)

1. 「**参照**」をクリックし、[ダウンロード](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)したソリューションを選択します。「**次へ**」をクリックします。

   ![](assets/image2015-3-19-9-20-56.png)

1. ソリューション情報を表示し、「**ソリューションパッケージ詳細を表示**」をクリックします。

   ![](assets/image2015-11-18-11-12-8.png)

1. すべての詳細を確認したら、「**閉じる**」をクリックします。

   ![](assets/step6.png)

1. ソリューション情報ページに戻り、「**次へ**」をクリックします。

   ![](assets/image2015-3-19-9-21-50.png)

1. 「SDK」オプションチェックボックスがオンになっていることを確認します。「**インポート**」をクリックします。

   ![](assets/image2015-3-19-9-19-12.png)

1. インポートが完了するまで待ちます。

   >[!TIP]
   >
   >インストールプロセスを完了するには、ブラウザーでポップアップを有効にする必要があります。

   ![](assets/image2015-3-11-11-34-9.png)

1. 必要に応じて、ログファイルをダウンロードし、「**閉じる**」をクリックします。

   >[!NOTE]
   >
   >「Marketo Lead Management completed with warning」というメッセージが表示される場合があります。これは十分予期されているものです。

   ![](assets/image2015-3-13-9-54-39.png)

1. Marketo リード管理が、**すべてのソリューション**&#x200B;ページに表示されます。

   ![](assets/image2015-3-19-8-40-38.png)

1. Marketo ソリューションを選択し、「**すべてのカスタマイズを公開**」をクリックします。

   ![](assets/image2015-3-19-8-41-21.png)

   完成です。インストールが完了しました。

   >[!CAUTION]
   >
   >Marketo SDK メッセージングプロセスを無効にすると、不完全なインストールになります。

   >[!MORELIKETHIS]
   >
   >[Dynamics 2015 オンプレミスおよび 2016 365 オンプレミス向け Marketo インストール手順 2 / 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-2-of-3-set-up.md)
