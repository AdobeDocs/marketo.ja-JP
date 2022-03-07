---
description: 手順 1／4 - リソース所有者のパスワード制御接続を使用した Marketo ソリューションのインストール - Marketo ドキュメント - 製品ドキュメント
title: 手順 1／4 - リソース所有者のパスワード制御接続を使用した Marketo ソリューションのインストール
exl-id: aab3bbb8-4e52-4c40-94d1-631af1d63f9f
source-git-commit: 7e6fab646ec03394cb406fc41442d585c162bb25
workflow-type: ht
source-wordcount: '308'
ht-degree: 100%

---

# 手順 1／4：リソース所有者のパスワード制御接続を使用した Marketo ソリューションのインストール {#step-1-of-4-install-the-marketo-solution-ropc}

Microsoft Dynamics 365 と Marketo を同期する前に、まず Dynamics に Marketo ソリューションをインストールする必要があります。**管理者権限が必要**。

>[!CAUTION]
>
>* 初期同期が完了する前にカスタムエンティティの同期を有効にしないでください。初回同期が完了すると、電子メールで通知されます。
>* Dynamics Sync で多要素認証（MFA）を有効にしている場合、Dynamics が Marketo と正しく同期するには、無効にする必要があります。詳しくは、[Marketo サポート](https://nation.marketo.com/t5/Support/ct-p/Support)にお問い合わせください。


>[!NOTE]
>
>Marketo を CRM に同期した後は、インスタンスを置き換えないと、新しい同期を実行できません。

>[!PREREQUISITES]
>
>[Marketo リード管理ソリューションのダウンロード](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)

1. **[Microsoft Office 365](https://login.microsoftonline.com/)**.にログインします。

   ![](assets/image2015-3-16-15-3a58-3a55.png)

1. ![](assets/image2015-3-16-16-3a1-3a13.png) メニューをクリックして、「**CRM**」を選択します。

   ![](assets/image2015-3-16-16-3a0-3a10.png)

1. ![](assets/image2015-5-13-10-3a5-3a8.png) メニューをクリックします。ドロップダウンメニューで、**設定**／**ソリューション**&#x200B;を選択します。

   ![](assets/image2015-5-13-10-3a4-3a1.png)

1. 「**インポート**」をクリックします。

   ![](assets/image2015-3-19-8-3a34-3a8.png)

1. 「**ファイルを選択**」をクリックします。[ダウンロードした](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) Marketo Lead Management ソリューションを選択します。「**次へ**」をクリックします。

   ![](assets/image2015-10-9-14-3a44-3a14.png)

1. ソリューション情報を表示し、「**ソリューションパッケージの詳細を表示**」をクリックします。

   ![](assets/image2015-10-9-15-3a4-3a16.png)

1. すべての詳細を確認したら、「**閉じる**」をクリックします。

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. 次に、ソリューション情報ページに戻り、「**次へ**」をクリックします。

   ![](assets/image2015-10-9-14-3a59-3a24.png)

1. 「SDK オプション」チェックボックスがオンになっていることを確認します。「**インポート**」をクリックします。

   ![](assets/image2015-10-9-15-3a7-3a12.png)

   >[!TIP]
   >
   >インストールプロセスを完了するには、ブラウザーでポップアップを有効にする必要があります。

1. インポートが完了するまで待ちます。休憩してください。

   ![](assets/image2015-3-11-11-3a34-3a9.png)

1. 「**閉じる**」をクリックします。

   >[!NOTE]
   >
   >「Marketo Lead Management completed with warning」というメッセージが表示される場合があります。これは完全に期待通りです。

   ![](assets/image2015-3-13-9-3a54-3a39.png)

1. Marketo Lead Management がソリューションのリストに表示されます。

   ![](assets/image2015-3-19-8-3a40-3a38.png)

1. 「**Marketo Lead Management**」を選択し、「**すべてのカスタマイズを公開**」をクリックします。

   ![](assets/image2015-3-19-8-3a41-3a21.png)

   完成です。インストールが完了しました。

   >[!MORELIKETHIS]
   >
   >[手順 2／4：リソース所有者のパスワード制御接続を使用した Marketo ソリューションの設定](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md)
