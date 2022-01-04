---
description: Microsoft Dynamics 2016/Dynamics 365 オンプレミス 1/3 - Marketoドキュメント — 製品ドキュメント
title: Microsoft Dynamics 2016/Dynamics 365 オンプレミスステップ 1/3 のMarketoのインストール
exl-id: 0a494ae7-87da-4ff9-bb47-990b957533e1
source-git-commit: 3fb93520a653109845c3b40aba20304c6163214f
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 2%

---

# 手順 1/3:Marketo (2016 On-Prem/Dynamics 365 On-Premises) の同期ユーザーを構成する {#step-of-configure-sync-user-for-marketo-on-premises-2016}

Microsoft Dynamics 2016 On-Prem/Dynamics 365 をMarketoと同期する前に、Dynamics にMarketoソリューションをインストールする必要があります。

>[!NOTE]
>
>Marketoを CRM に同期した後は、新しい CRM を既存のMarketoインスタンスに同期できません。

>[!PREREQUISITES]
>
>Microsoft Dynamics オンプレミスを使用している場合は、 [インターネット対応の導入](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD) [Active Directory フェデレーションサービス](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0 以降 (ADFS) が設定されました。 注意：IFD ドキュメントは、リンクをクリックすると自動的にダウンロードされます。
>
>[Marketo Lead Management Solution のダウンロード](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) 始める前に

>[!NOTE]
>
>**Dynamics 管理権限が必要です。**
>
>この同期を実行するには、CRM 管理者権限が必要です。

1. にログインします。 **Dynamics.** 次をクリック： **Microsoft Dynamics CRM** ドロップダウンメニューで「 」を選択します。 **設定**.

   ![](assets/image2015-3-19-8-33-29.png)

1. の下 **設定**&#x200B;を選択します。 **ソリューション**.

   ![](assets/image2015-3-19-8-33-3.png)

1. 「**インポート**」をクリックします。

   ![](assets/image2015-3-19-8-34-8.png)

1. クリック **参照** をクリックし、次の方法を選択します。 [ダウンロード](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). 「**次へ**」をクリックします。

   ![](assets/image2015-3-19-9-20-56.png)

1. ソリューション情報を表示し、 **ソリューションパッケージの詳細を表示**.

   ![](assets/image2015-11-18-11-12-8.png)

1. すべての詳細を確認したら、 **閉じる**.

   ![](assets/step6.png)

1. ソリューション情報ページに戻り、 **次へ**.

   ![](assets/image2015-3-19-9-21-50.png)

1. 「 SDK オプション」チェックボックスがオンになっていることを確認します。 「**インポート**」をクリックします。

   ![](assets/image2015-3-19-9-19-12.png)

1. インポートが完了するまで待ちます。

   >[!TIP]
   >
   >インストールプロセスを完了するには、ブラウザーでポップアップを有効にする必要があります。

   ![](assets/image2015-3-11-11-34-9.png)

1. 必要に応じて、ログファイルをダウンロードし、 **閉じる**.

   >[!NOTE]
   >
   >「Marketo Lead Management completed with warning」というメッセージが表示される場合があります。 これは完全に期待されています。

   ![](assets/image2015-3-13-9-54-39.png)

1. Marketoリード管理が **すべてのソリューション** ページ。

   ![](assets/image2015-3-19-8-40-38.png)

1. Marketoソリューションを選択し、 **すべてのカスタマイズを公開**.

   ![](assets/image2015-3-19-8-41-21.png)

   完成です。インストールが完了しました。

   >[!CAUTION]
   >
   >Marketo SDK メッセージングプロセスを無効にすると、インストールが壊れます。

   >[!MORELIKETHIS]
   >
   >[Dynamics 2015 オンプレミスおよび 2016 365 オンプレミス用Marketoのインストール手順 2 / 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-2-of-3-set-up.md)
