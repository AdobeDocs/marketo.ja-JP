---
unique-page-id: 3571805
description: 手順 1/3 - Marketoソリューション（2011 オンプレミス）のインストール — Marketoドキュメント — 製品ドキュメント
title: 手順 1/3 - Marketoソリューション（2011 オンプレミス）のインストール
exl-id: 6e559b10-5273-4dc2-b98d-49c509cbeff7
source-git-commit: 2568d3414c8aaec882b79442f6312bae3b9514ab
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 13%

---

# 手順 1 / 3：Marketo ソリューション（2011 オンプレミス版）のインストール {#step-of-install-the-marketo-solution-on-premises}

Microsoft Dynamics On-Premises とMarketoを同期する前に、Dynamics にMarketoソリューションをインストールする必要があります。

>[!NOTE]
>
>Marketoを CRM に同期した後は、インスタンスを置き換えないと、新しい同期を実行できません。

>[!PREREQUISITES]
>
>必ず [インターネット対応の導入](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD) [Active Directory フェデレーションサービス](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0、2.1、または 3.0(ADFS) が設定されました。 **注意**:IFD ドキュメントは、リンクをクリックすると自動的にダウンロードされます。
>
>[Marketo Lead Management Solution のダウンロード](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) 始める前に

>[!NOTE]
>
>**Dynamics 管理権限が必要です。**
>
>この同期を実行するには、CRM 管理者権限が必要です。

1. にログインします。 **Dynamics**&#x200B;を選択します。 **設定** をクリックします。

   ![](assets/image2015-4-2-11-3a32-3a53.png)

1. ツリーで「**ソリューション**」を選択します。

   ![](assets/image2015-4-2-11-3a35-3a28.png)

1. 「**インポート**」をクリックします。

   ![](assets/image2015-4-2-11-3a37-3a33.png)

1. 「**参照**」をクリックします。お使いのMarketo Lead Management ソリューションを選択してください [ダウンロード](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). 「**次へ**」をクリックします。

   ![](assets/image2015-4-2-11-3a40-3a33.png)

1. ソリューション情報を表示し、 **ソリューションパッケージの詳細を表示**.

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. すべての詳細を確認したら、 **閉じる**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. ソリューション情報ページに戻り、 **次へ**.

   ![](assets/image2015-4-2-11-3a41-3a48.png)

1. 「 SDK メッセージオプション」チェックボックスがオンになっていることを確認します。 「**次へ**」をクリックします。

   ![](assets/image2015-4-2-11-3a42-3a37.png)

   >[!TIP]
   >
   >インストールプロセスを完了するには、ブラウザーでポップアップを有効にする必要があります。

1. インポートが完了するまで待ちます。起き上がってストレッチを行う。

   ![](assets/image2015-4-2-11-3a43-3a51.png)

1. 「**閉じる**」をクリックします。

   >[!NOTE]
   >
   >「Marketo Lead Management completed with warning」というメッセージが表示される場合があります。 これは完全に期待されています。

   ![](assets/image2015-4-2-11-3a44-3a44.png)

1. Marketoリード管理が **すべてのソリューション** ページ。

   ![](assets/image2015-4-2-11-3a46-3a55.png)

1. 「 Marketo Lead Management 」を選択し、「 **すべてのカスタマイズを公開します。**

   ![](assets/image2015-4-2-11-3a48-3a21.png)

悪くなかったでしょ？ さあ、あとは歩き続ける。

>[!CAUTION]
>
>Marketo SDK メッセージングプロセスを無効にすると、インストールが壊れます。

>[!MORELIKETHIS]
>
>[手順 2 / 3：Dynamics（2011 オンプレミス）での Marketo 同期ユーザーのセットアップ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-2-of-3-set-up.md)
