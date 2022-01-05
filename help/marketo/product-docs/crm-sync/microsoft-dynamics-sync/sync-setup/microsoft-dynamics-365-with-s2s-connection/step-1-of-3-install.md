---
description: 手順 1/3 - S2S 接続を使用したMarketoソリューションのインストール — Marketoドキュメント — 製品ドキュメント
title: 手順 1/3 - S2S 接続を使用したMarketoソリューションのインストール
source-git-commit: 9ee27e22fec4e0ab85c193be2ea99d3c8b40568b
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 8%

---

# 手順 1/3:S2S 接続を使用したMarketoソリューションのインストール {#step-1-of-3-install-the-marketo-solution-s2s}

Microsoft Dynamics 365 とMarketoを同期する前に、まず Dynamics にMarketoソリューションをインストールする必要があります。 **Dynamics 管理権限が必要です。**

>[!CAUTION]
>
>* 初期同期が完了する前にカスタムエンティティの同期を有効にしないでください。 初回同期が完了すると、電子メールで通知されます。
>* Dynamics 同期で多要素認証 (MFA) を有効にしている場合、Dynamics がMarketoと正しく同期するには、無効にする必要があります。 詳しくは、 [Marketoサポート](https://nation.marketo.com/t5/Support/ct-p/Support).


>[!NOTE]
>
>Marketoを CRM に同期した後は、インスタンスを置き換えないと、新しい同期を実行できません。

>[!PREREQUISITES]
>
>[Marketo リード管理ソリューションのダウンロード](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)

1. にログインします。 **[Microsoft Office 365](https://login.microsoftonline.com/)**.

   ![](assets/image2015-3-16-15-3a58-3a55.png)

1. クリック ![](assets/image2015-3-16-16-3a1-3a13.png) メニューと選択 **CRM**.

   ![](assets/image2015-3-16-16-3a0-3a10.png)

1. クリック ![](assets/image2015-5-13-10-3a5-3a8.png) メニュー ドロップダウンメニューで、を選択します。 **設定** 次に、 **ソリューション**.

   ![](assets/image2015-5-13-10-3a4-3a1.png)

1. クリック **インポート。**

   ![](assets/image2015-3-19-8-3a34-3a8.png)

1. クリック **「ファイル」を選択します。** お使いのMarketo Lead Management ソリューションを選択してください [ダウンロード](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). 「**次へ**」をクリックします。

   ![](assets/image2015-10-9-14-3a44-3a14.png)

1. ソリューション情報を表示し、 **ソリューションパッケージの詳細を表示**.

   ![](assets/image2015-10-9-15-3a4-3a16.png)

1. すべての詳細を確認したら、 **閉じる**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. 次に、ソリューション情報ページに戻り、 **次へ**.

   ![](assets/image2015-10-9-14-3a59-3a24.png)

1. 「 SDK オプション」チェックボックスがオンになっていることを確認します。 「**インポート**」をクリックします。

   ![](assets/image2015-10-9-15-3a7-3a12.png)

   >[!TIP]
   >
   >インストールプロセスを完了するには、ブラウザーでポップアップを有効にする必要があります。

1. インポートが完了するまで待ちます。起き上がってストレッチを行う。

   ![](assets/image2015-3-11-11-3a34-3a9.png)

1. クリック **閉じます。**

   >[!NOTE]
   >
   >「Marketo Lead Management completed with warning」というメッセージが表示される場合があります。 これは完全に期待されています。

   ![](assets/image2015-3-13-9-3a54-3a39.png)

1. Marketo Lead Management がソリューションのリストに表示されます。

   ![](assets/image2015-3-19-8-3a40-3a38.png)

1. 選択 **Marketoリード管理** をクリックし、 **すべてのカスタマイズを公開します。**

   ![](assets/image2015-3-19-8-3a41-3a21.png)

   完成です。インストールが完了しました。

   >[!MORELIKETHIS]
   >
   >[手順 2 / 3:S2S 接続を使用したMarketoソリューションのセットアップ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up.md)
