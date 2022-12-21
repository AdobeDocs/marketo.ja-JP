---
unique-page-id: 3571813
description: 手順 1 / 3 - Dynamics（2013 オンプレミス）での Marketo ソリューションのインストール - Marketo ドキュメント - 製品ドキュメント
title: 手順 1 / 3 - Dynamics（2013 オンプレミス）での Marketo ソリューションのインストール
exl-id: 89f90bca-b459-447f-bbdd-363f232a1059
source-git-commit: 64c5f03bd2320bfbffd257684d1482e995def83a
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 100%

---

# 手順 1 / 3：Dynamics（2013 オンプレミス）での Marketo ソリューションのインストール {#step-of-install-the-marketo-solution-in-dynamics-on-premises}

Microsoft Dynamics オンプレミスと Marketo を同期する前に、Dynamics に Marketo ソリューションをインストールする必要があります。

>[!NOTE]
>
>Marketo を CRM に同期した後は、インスタンスを置き換えないと、新しい同期を実行できません。

>[!PREREQUISITES]
>
>[Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0、2.1、または 3.0（ADFS）が設定された、[インターネットに接続する展開](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701)（IFD）が構成されている必要があります。注意：IFD ドキュメントは、リンクをクリックすると自動的にダウンロードされます。
>
>始める前に、[Marketo ソリューションをダウンロード](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)します。

>[!NOTE]
>
>**Dynamics 管理権限が必要。**
>
>この同期を実行するには、CRM 管理者権限が必要です。

1. **Dynamics** にログインします。「**Microsoft Dynamics CRM**」ドロップダウンをクリックし、「**設定**」を選択します。

   ![](assets/image2014-12-11-10-3a39-3a41.png)

1. 「**設定**」で、「**ソリューション**」を選択します。

   ![](assets/image2014-12-11-10-3a39-3a51.png)

1. 「**インポート**」をクリックします。

   ![](assets/image2015-3-26-9-3a52-3a10.png)

1. 「**参照**」をクリックし、「[ダウンロードされたソリューション](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)」を選択します。「**次へ**」をクリックします。

   ![](assets/image2015-3-26-9-3a54-3a1.png)

1. ソリューション情報を表示し、「**ソリューションパッケージ詳細を表示**」をクリックします。

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. すべての詳細を確認したら、「**閉じる**」をクリックします。

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. ソリューション情報ページに戻り、「**次へ**」をクリックします。

   ![](assets/image2015-3-26-9-3a55-3a17.png)

1. 「SDK」オプションがオンになっていることを確認します。「**インポート**」をクリックします。

   ![](assets/image2015-3-26-10-3a3-3a11.png)

1. インポートが完了するまで待ちます。

   >[!TIP]
   >
   >インストールプロセスを完了するには、ブラウザーでポップアップを有効にする必要があります。

   ![](assets/image2014-12-11-10-3a41-3a5.png)

1. 必要に応じて、ログファイルをダウンロードし、「**閉じる**」をクリックします。

   >[!NOTE]
   >
   >「Marketo Lead Management completed with warning」というメッセージが表示される場合があります。これは十分予期されているものです。

   ![](assets/image2014-12-11-10-3a41-3a14.png)

1. Marketo リード管理が、**すべてのソリューション**&#x200B;ページに表示されます。

   ![](assets/image2015-3-26-10-3a1-3a21.png)

1. Marketo ソリューションを選択し、「**すべてのカスタマイズを公開**」をクリックします。

   ![](assets/image2014-12-11-10-3a41-3a32.png)

これで完了です。それでは、先へ進みましょう。

>[!CAUTION]
>
>Marketo SDK メッセージングプロセスを無効にすると、不完全なインストールになります。

>[!MORELIKETHIS]
>
>[手順 2 / 3：Marketo（2013 オンプレミス）の同期ユーザーの設定](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-configure-2013.md)
