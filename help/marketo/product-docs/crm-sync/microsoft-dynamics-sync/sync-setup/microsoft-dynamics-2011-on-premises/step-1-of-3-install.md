---
unique-page-id: 3571805
description: 手順1/3 -Marketoソリューション（2011オンプレミス）のインストール —Marketoドキュメント — 製品ドキュメント
title: 手順1/3 -Marketoソリューションのインストール（2011オンプレミス）
exl-id: 6e559b10-5273-4dc2-b98d-49c509cbeff7
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---

# 手順1/3:Marketoソリューション(2011 On-Premises)のインストール{#step-of-install-the-marketo-solution-on-premises}

Microsoft Dynamics On-PremisesとMarketoを同期する前に、DynamicsにMarketoソリューションをインストールする必要があります。

>[!NOTE]
>
>MarketoをCRMに同期した後は、インスタンスを置き換えないと、新しい同期を実行できません。

>[!PREREQUISITES]
>
>[Active Directoryフェデレーションサービス](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0、2.1、または3.0 (ADFS)が構成された[インターネット対応の展開](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD)が必要です。 **注意**:IFDドキュメントは、リンクをクリックすると自動的にダウンロードします。
>
>[開始の前に、Marketoリード管理](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) ソリューションをダウンロードしてください。

>[!NOTE]
>
>**Dynamics管理権限が必要です。**
>
>この同期を実行するには、CRMの管理者権限が必要です。

1. **Dynamics**&#x200B;にログインし、左下のメニューで&#x200B;**設定**&#x200B;を選択します。

   ![](assets/image2015-4-2-11-3a32-3a53.png)

1. ツリーで&#x200B;**ソリューション**&#x200B;を選択します。

   ![](assets/image2015-4-2-11-3a35-3a28.png)

1. 「**インポート**」をクリックします。

   ![](assets/image2015-4-2-11-3a37-3a33.png)

1. 「**参照**」をクリックします。 [ダウンロードした](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)Marketoリード管理ソリューションを選択します。 「**次へ**」をクリックします。

   ![](assets/image2015-4-2-11-3a40-3a33.png)

1. ソリューション情報を表示し、**表示ソリューションパッケージの詳細**&#x200B;をクリックします。

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. すべての詳細の確認が完了したら、[**閉じる**]をクリックします。

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. ソリューション情報ページに戻り、「**次へ**」をクリックします。

   ![](assets/image2015-4-2-11-3a41-3a48.png)

1. 「SDKメッセージオプション」チェックボックスがオンになっていることを確認します。 「**次へ**」をクリックします。

   ![](assets/image2015-4-2-11-3a42-3a37.png)

   >[!TIP]
   >
   >インストールプロセスを完了するには、ブラウザーでポップアップを有効にする必要があります。

1. 次に、インポートが終了するのを待ちます。 起き上がって、何か手を伸ばして。

   ![](assets/image2015-4-2-11-3a43-3a51.png)

1. 「**閉じる**」をクリックします。

   >[!NOTE]
   >
   >「Marketoリード管理は警告付きで完了しました」というメッセージが表示される場合があります。 これは完全に期待されています。

   ![](assets/image2015-4-2-11-3a44-3a44.png)

1. Marketoリードの管理が&#x200B;**すべてのソリューション**&#x200B;ページに表示されます。

   ![](assets/image2015-4-2-11-3a46-3a55.png)

1. 「Marketoリード管理」を選択し、「**すべてのカスタマイズを発行」をクリックします。**

   ![](assets/image2015-4-2-11-3a48-3a21.png)

悪くなかった？ さあ、残りの部分を歩き続ける。

>[!CAUTION]
>
>MarketoSDKメッセージングプロセスを無効にすると、インストールが中断されます。

>[!MORELIKETHIS]
>
>[手順2/3:DynamicsでのMarketo同期ユーザーのセットアップ（2011オンプレミス）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-2-of-3-set-up.md)
