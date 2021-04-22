---
unique-page-id: 3571822
description: 手順1/3 -Marketoソリューションのインストール（オンライン） -Marketoドキュメント — 製品ドキュメント
title: 手順1/3 -Marketoソリューションのインストール（オンライン）
exl-id: 593fc014-db38-42cc-8f9f-0dd8307751e8
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 0%

---

# 手順1/3:Marketoソリューションのインストール（オンライン） {#step-of-install-the-marketo-solution-online}

Microsoft Dynamics 365とMarketoを同期する前に、DynamicsにMarketoソリューションをインストールする必要があります。 **Dynamics管理権限が必要です。**

>[!CAUTION]
>
>* 初期同期が完了する前に、カスタムエンティティの同期を有効にしないでください。 初回同期が完了すると、電子メールで通知されます。
>* Dynamics SyncでMulti-Factor Authentication (MFA)が有効になっている場合、DynamicsがMarketoと正しく同期するには、これを無効にする必要があります。 詳しくは、[Marketoサポート](https://nation.marketo.com/t5/Support/ct-p/Support)にお問い合わせください。


>[!NOTE]
>
>MarketoをCRMに同期した後は、インスタンスを置き換えないと、新しい同期を実行できません。

>[!PREREQUISITES]
>
>[Marketoリード管理ソリューションのダウンロード](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)

1. **[Microsoft Office 365](https://login.microsoftonline.com/)**&#x200B;にログインします。

   ![](assets/image2015-3-16-15-3a58-3a55.png)

1. ![](assets/image2015-3-16-16-3a1-3a13.png)メニューをクリックし、**CRM**&#x200B;を選択します。

   ![](assets/image2015-3-16-16-3a0-3a10.png)

1. ![](assets/image2015-5-13-10-3a5-3a8.png)メニューをクリックします。 ドロップダウンメニューで[**設定**]を選択し、[**ソリューション**]を選択します。

   ![](assets/image2015-5-13-10-3a4-3a1.png)

1. 「**読み込み」をクリックします。**

   ![](assets/image2015-3-19-8-3a34-3a8.png)

1. 「**ファイルを選択」をクリックします。** ダウンロードしたMarketoリード管理ソリューションを選択 [します](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)。「**次へ**」をクリックします。

   ![](assets/image2015-10-9-14-3a44-3a14.png)

1. ソリューション情報を表示し、**表示ソリューションパッケージの詳細**&#x200B;をクリックします。

   ![](assets/image2015-10-9-15-3a4-3a16.png)

1. すべての詳細の確認が完了したら、[**閉じる**]をクリックします。

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. 次に、ソリューション情報ページに戻り、**次へ**&#x200B;をクリックします。

   ![](assets/image2015-10-9-14-3a59-3a24.png)

1. 「SDKオプション」チェックボックスが選択されていることを確認します。 「**インポート**」をクリックします。

   ![](assets/image2015-10-9-15-3a7-3a12.png)

   >[!TIP]
   >
   >インストールプロセスを完了するには、ブラウザーでポップアップを有効にする必要があります。

1. 次に、インポートが終了するのを待ちます。 起き上がって、何か手を伸ばして。

   ![](assets/image2015-3-11-11-3a34-3a9.png)

1. 「**閉じる」をクリックします。**

   >[!NOTE]
   >
   >「Marketoリード管理は警告付きで完了しました」というメッセージが表示される場合があります。 これは完全に期待されています。

   ![](assets/image2015-3-13-9-3a54-3a39.png)

1. Marketoリードマネジメントは、ソリューションのリストに表示されます。

   ![](assets/image2015-3-19-8-3a40-3a38.png)

1. **Marketoリード管理**&#x200B;を選択し、**「すべてのカスタマイズを発行」をクリックします。**

   ![](assets/image2015-3-19-8-3a41-3a21.png)

   ハイフィーブ！ インストールが完了しました。

   >[!MORELIKETHIS]
   >
   >[手順2/3:DynamicsでのMarketo同期ユーザーの設定](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-2-of-3-set-up.md)
