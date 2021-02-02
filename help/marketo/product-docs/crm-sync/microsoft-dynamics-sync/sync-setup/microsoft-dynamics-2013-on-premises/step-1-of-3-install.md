---
unique-page-id: 3571813
description: 手順1/3 - Dynamics (2013 On-Premises)でのMarketo Solutionのインストール — Marketto Docs — 製品ドキュメント
title: 手順1/3 - DynamicsでのMarketo Solutionのインストール(2013 On-Premises)
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---


# 手順1/3:Dynamics (2013 On-Premises)にMarketo Solutionをインストールする{#step-of-install-the-marketo-solution-in-dynamics-on-premises}

Microsoft Dynamics On-PremisesとMarketoを同期する前に、DynamicsにMarketo Solutionをインストールする必要があります。

>[!NOTE]
>
>マーケティングをCRMに同期した後は、インスタンスを置き換えないと、新しい同期を実行できません。

>[!PREREQUISITES]
>
>[Active Directoryフェデレーションサービス](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0、2.1、または3.0 (ADFS)が構成された[インターネット対応の展開](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD)が必要です。 注意：IFDドキュメントは、リンクをクリックすると自動的にダウンロードします。
>
>[開始する前に、Marketing ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) Solutionをダウンロードしてください。

>[!NOTE]
>
>**Dynamics管理権限が必要です。**
>
>この同期を実行するには、CRMの管理者権限が必要です。

1. **Dynamics**&#x200B;にログインします。 **Microsoft Dynamics CRM**&#x200B;ドロップダウンメニューをクリックし、**設定**&#x200B;を選択します。

   ![](assets/image2014-12-11-10-3a39-3a41.png)

1. 「**設定**」で、「**ソリューション**」を選択します。

   ![](assets/image2014-12-11-10-3a39-3a51.png)

1. 「**インポート**」をクリックします。

   ![](assets/image2015-3-26-9-3a52-3a10.png)

1. 「**参照**」をクリックし、[ダウンロードしたソリューション](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)を選択します。 「**次へ**」をクリックします。

   ![](assets/image2015-3-26-9-3a54-3a1.png)

1. ソリューション情報を表示し、**表示ソリューションパッケージの詳細**&#x200B;をクリックします。

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. すべての詳細の確認が完了したら、[**閉じる**]をクリックします。

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. ソリューション情報ページに戻り、「**次へ**」をクリックします。

   ![](assets/image2015-3-26-9-3a55-3a17.png)

1. 「SDK」オプションがオンになっていることを確認します。 「**インポート**」をクリックします。

   ![](assets/image2015-3-26-10-3a3-3a11.png)

1. インポートが完了するまで待ちます。

   >[!TIP]
   >
   >インストールプロセスを完了するには、ブラウザーでポップアップを有効にする必要があります。

   ![](assets/image2014-12-11-10-3a41-3a5.png)

1. ログファイルをダウンロードし（必要に応じて）、**閉じる**&#x200B;をクリックします。

   >[!NOTE]
   >
   >「Marketto Lead Management completed with warning」というメッセージが表示される場合があります。 これは完全に期待されています。

   ![](assets/image2014-12-11-10-3a41-3a14.png)

1. Marketto Lead Managementが&#x200B;**すべてのソリューション**&#x200B;ページに表示されます。

   ![](assets/image2015-3-26-10-3a1-3a21.png)

1. Marketoソリューションを選択し、「**すべてのカスタマイズを発行**」をクリックします。

   ![](assets/image2014-12-11-10-3a41-3a32.png)

悪くなかった？ さあ、残りの部分を歩き続ける。

>[!CAUTION]
>
>Marketto SDKのメッセージングプロセスを無効にすると、インストールが中断されます。

>[!MORELIKETHIS]
>
>[手順2/3:Marketor用の同期ユーザーの設定(2013 On-Premises)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-2-of-3-configure.md)
