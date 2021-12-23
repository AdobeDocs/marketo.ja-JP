---
unique-page-id: 3571813
description: 手順 1/3 - Dynamics（2013 オンプレミス）にMarketoソリューションをインストールする — Marketoドキュメント — 製品ドキュメント
title: 手順 1/3 - Dynamics （2013 オンプレミス）にMarketoソリューションをインストールする
exl-id: 89f90bca-b459-447f-bbdd-363f232a1059
source-git-commit: 64c5f03bd2320bfbffd257684d1482e995def83a
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 7%

---

# 手順 1 / 3：Dynamics（2013 オンプレミス）での Marketo ソリューションのインストール {#step-of-install-the-marketo-solution-in-dynamics-on-premises}

Microsoft Dynamics On-Premises とMarketoを同期する前に、Dynamics にMarketoソリューションをインストールする必要があります。

>[!NOTE]
>
>Marketoを CRM に同期した後は、インスタンスを置き換えないと、新しい同期を実行できません。

>[!PREREQUISITES]
>
>必ず [インターネット対応の導入](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD) [Active Directory フェデレーションサービス](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0、2.1、または 3.0(ADFS) が設定されました。 注意：IFD ドキュメントは、リンクをクリックすると自動的にダウンロードされます。
>
>[Marketo Solution のダウンロード](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) 始める前に

>[!NOTE]
>
>**Dynamics 管理権限が必要です。**
>
>この同期を実行するには、CRM 管理者権限が必要です。

1. ログイン **Dynamics**. 次をクリック： **Microsoft Dynamics CRM** ドロップダウンメニューで「 」を選択します。 **設定**.

   ![](assets/image2014-12-11-10-3a39-3a41.png)

1. の下 **設定**&#x200B;を選択します。 **ソリューション**.

   ![](assets/image2014-12-11-10-3a39-3a51.png)

1. 「**インポート**」をクリックします。

   ![](assets/image2015-3-26-9-3a52-3a10.png)

1. クリック **参照** をクリックし、 [ダウンロードされたソリューション](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). 「**次へ**」をクリックします。

   ![](assets/image2015-3-26-9-3a54-3a1.png)

1. ソリューション情報を表示し、 **ソリューションパッケージの詳細を表示**.

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. すべての詳細を確認したら、 **閉じる**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. ソリューション情報ページに戻り、 **次へ**.

   ![](assets/image2015-3-26-9-3a55-3a17.png)

1. 「 SDK 」オプションがオンになっていることを確認します。 「**インポート**」をクリックします。

   ![](assets/image2015-3-26-10-3a3-3a11.png)

1. インポートが完了するまで待ちます。

   >[!TIP]
   >
   >インストールプロセスを完了するには、ブラウザーでポップアップを有効にする必要があります。

   ![](assets/image2014-12-11-10-3a41-3a5.png)

1. 必要に応じて、ログファイルをダウンロードし、 **閉じる**.

   >[!NOTE]
   >
   >「Marketo Lead Management completed with warning」というメッセージが表示される場合があります。 これは完全に期待されています。

   ![](assets/image2014-12-11-10-3a41-3a14.png)

1. Marketoリード管理が **すべてのソリューション** ページ。

   ![](assets/image2015-3-26-10-3a1-3a21.png)

1. Marketoソリューションを選択し、 **すべてのカスタマイズを公開**.

   ![](assets/image2014-12-11-10-3a41-3a32.png)

悪くなかったでしょ？ さあ、あとは歩き続ける。

>[!CAUTION]
>
>Marketo SDK メッセージングプロセスを無効にすると、インストールが壊れます。

>[!MORELIKETHIS]
>
>[手順 2 / 3：Marketo（2013 オンプレミス）の同期ユーザーの設定](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-configure-2013.md)
