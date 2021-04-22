---
unique-page-id: 7504736
description: Dynamics 2015オンプレム版Marketoと2016 365オンプレム版の3 -Marketoドキュメント — 製品ドキュメントのインストール手順1
title: Dynamics 2015オンプレム版Marketoと2016 365オンプレム版の3ステップ1のインストール
exl-id: c9b6d365-15c1-4eff-938c-8433b1fe7f24
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---

# 手順1/3:Marketoの同期ユーザーの設定（2015オンプレムおよび2016 365オンプレム） {#step-of-configure-sync-user-for-marketo-on-premises-and-365}

Microsoft Dynamics 2015オンプレミスまたは2016 (Dynamics 365)をMarketoと同期する前に、DynamicsでMarketoソリューションをインストールする必要があります。

>[!NOTE]
>
>MarketoをCRMに同期した後は、新しいCRMを既存のMarketoのインスタンスと同期できません。

>[!PREREQUISITES]
>
>Microsoft Dynamics On-Premiseを使用する場合は、[Active Directoryフェデレーションサービス](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0+ (ADFS)が構成された[インターネット対応展開](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD)が必要です。 注意：IFDドキュメントは、リンクをクリックすると自動的にダウンロードします。
>
>[開始の前に、Marketoリード管理](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) ソリューションをダウンロードしてください。

>[!NOTE]
>
>**Dynamics管理権限が必要です。**
>
>この同期を実行するには、CRMの管理者権限が必要です。

1. **Dynamicsにログインします。** 「 **Microsoft Dynamics** CRM」ドロップダウンメニューをクリックし、「 **設定**」を選択します。

   ![](assets/image2015-3-19-8-33-29.png)

1. 「**設定**」で、「**ソリューション**」を選択します。

   ![](assets/image2015-3-19-8-33-3.png)

1. 「**インポート**」をクリックします。

   ![](assets/image2015-3-19-8-34-8.png)

1. 「**参照**」をクリックし、[ダウンロードした](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)ソリューションを選択します。 「**次へ**」をクリックします。

   ![](assets/image2015-3-19-9-20-56.png)

1. ソリューション情報を表示し、**表示ソリューションパッケージの詳細**&#x200B;をクリックします。

   ![](assets/image2015-11-18-11-12-8.png)

1. すべての詳細の確認が完了したら、[**閉じる**]をクリックします。

   ![](assets/step6.png)

1. ソリューション情報ページに戻り、「**次へ**」をクリックします。

   ![](assets/image2015-3-19-9-21-50.png)

1. 「SDKオプション」チェックボックスが選択されていることを確認します。 「**インポート**」をクリックします。

   ![](assets/image2015-3-19-9-19-12.png)

1. インポートが完了するまで待ちます。

   >[!TIP]
   >
   >インストールプロセスを完了するには、ブラウザーでポップアップを有効にする必要があります。

   ![](assets/image2015-3-11-11-34-9.png)

1. ログファイルをダウンロードし（必要に応じて）、**閉じる**&#x200B;をクリックします。

   >[!NOTE]
   >
   >「Marketoリード管理は警告付きで完了しました」というメッセージが表示される場合があります。 これは完全に期待されています。

   ![](assets/image2015-3-13-9-54-39.png)

1. Marketoリードの管理が&#x200B;**すべてのソリューション**&#x200B;ページに表示されます。

   ![](assets/image2015-3-19-8-40-38.png)

1. Marketoソリューションを選択し、「**すべてのカスタマイズを発行**」をクリックします。

   ![](assets/image2015-3-19-8-41-21.png)

   ハイフィーブ！ インストールが完了しました。

   >[!CAUTION]
   >
   >MarketoSDKメッセージングプロセスを無効にすると、インストールが中断されます。

   >[!MORELIKETHIS]
   >
   >[Dynamics 2015 On-Premおよび2016 365 On-Prem Step 2 of 3のDynamics 2015 On-Premのインストール](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-2-of-3-set-up.md)
