---
unique-page-id: 3571805
description: 手順 1 / 3 - Marketo ソリューション（2011 オンプレミス版）のインストール - Marketo ドキュメント - 製品ドキュメント
title: 手順 1 / 3 - Marketo ソリューション（2011 オンプレミス版）のインストール
exl-id: 6e559b10-5273-4dc2-b98d-49c509cbeff7
source-git-commit: eac7e219f1babc22dce30717fea4cecb93e1cce7
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 100%

---

# 手順 1 / 3：Marketo ソリューション（2011 オンプレミス版）のインストール {#step-of-install-the-marketo-solution-on-premises}

Microsoft Dynamics オンプレミスと Marketo を同期する前に、Dynamics に Marketo ソリューションをインストールする必要があります。

>[!NOTE]
>
>Marketo を CRM に同期した後は、インスタンスを置き換えないと、新しい同期を実行できません。

>[!PREREQUISITES]
>
>[Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0、2.1、または 3.0（ADFS）が設定された、[インターネットに接続する展開](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701)（IFD）が構成されている必要があります。**注意**：IFD ドキュメントは、リンクをクリックすると自動的にダウンロードされます。
>
>始める前に、[Marketo リード管理ソリューションをダウンロード](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)します。

>[!NOTE]
>
>**Dynamics 管理権限が必要。**
>
>この同期を実行するには、CRM 管理者権限が必要です。

1. **Dynamics** にログインして、左下のメニューで「**設定**」を選択します。

   ![](assets/image2015-4-2-11-3a32-3a53.png)

1. ツリーで「**ソリューション**」を選択します。

   ![](assets/image2015-4-2-11-3a35-3a28.png)

1. 「**インポート**」をクリックします。

   ![](assets/image2015-4-2-11-3a37-3a33.png)

1. 「**参照**」をクリックします。[ダウンロードした](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) Marketo リード管理ソリューションを選択します。「**次へ**」をクリックします。

   ![](assets/image2015-4-2-11-3a40-3a33.png)

1. ソリューション情報を表示し、「**ソリューションパッケージ詳細を表示**」をクリックします。

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. すべての詳細を確認したら、「**閉じる**」をクリックします。

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. ソリューション情報ページに戻り、「**次へ**」をクリックします。

   ![](assets/image2015-4-2-11-3a41-3a48.png)

1. 「SDK メッセージ」オプションチェックボックスがオンになっていることを確認します。「**次へ**」をクリックします。

   ![](assets/image2015-4-2-11-3a42-3a37.png)

   >[!TIP]
   >
   >インストールプロセスを完了するには、ブラウザーでポップアップを有効にする必要があります。

1. インポートが完了するまで待ちます。ストレッチでもしながらお待ちください。

   ![](assets/image2015-4-2-11-3a43-3a51.png)

1. 「**閉じる**」をクリックします。

   >[!NOTE]
   >
   >「Marketo Lead Management completed with warning」というメッセージが表示される場合があります。これは十分予期されているものです。

   ![](assets/image2015-4-2-11-3a44-3a44.png)

1. Marketo リード管理が、**すべてのソリューション**&#x200B;ページに表示されます。

   ![](assets/image2015-4-2-11-3a46-3a55.png)

1. 「Marketo リード管理」を選択し、「**すべてのカスタマイズを公開**」をクリックします。

   ![](assets/image2015-4-2-11-3a48-3a21.png)

これで完了です。それでは、先へ進みましょう。

>[!CAUTION]
>
>Marketo SDK メッセージングプロセスを無効にすると、不完全なインストールになります。

>[!MORELIKETHIS]
>
>[手順 2 / 3：Dynamics（2011 オンプレミス）での Marketo 同期ユーザーのセットアップ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-set-up-2011.md)
