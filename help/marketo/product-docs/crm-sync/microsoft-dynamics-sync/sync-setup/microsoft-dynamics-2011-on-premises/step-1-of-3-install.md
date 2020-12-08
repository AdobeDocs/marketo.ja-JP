---
unique-page-id: 3571805
description: 手順1/3 - Marketto Solution(2011 On-Premises)のインストール — Marketto Docs — 製品ドキュメント
title: 手順1/3 - Marketto Solution(2011 On-Premises)のインストール
translation-type: tm+mt
source-git-commit: dc20aede0894a09e6c0bcd3d1580859b5fecb5f1
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---


# 手順1/3:Marketo Solution(2011 On-Premises)のインストール {#step-of-install-the-marketo-solution-on-premises}

Microsoft Dynamics On-PremisesとMarketoを同期する前に、DynamicsにMarketo Solutionをインストールする必要があります。

>[!NOTE]
>
>マーケティングをCRMに同期した後は、インスタンスを置き換えないと、新しい同期を実行できません。

>[!NOTE]
>
>**前提条件**
>
>Active Directoryフェデレーションサービス [2.0、2.1、または3.0 (ADFS)が構成されている](http://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) Internet Facing Deployment [](https://msdn.microsoft.com/en-us/library/bb897402.aspx) (IFD)が必要です。 **注意**:IFDドキュメントは、リンクをクリックすると自動的にダウンロードします。
>
>[開始する前に、Marketto Lead Management Solution](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) をダウンロードします。

>[!NOTE]
>
>**Dynamics管理権限が必要です。**
>
>この同期を実行するには、CRMの管理者権限が必要です。

1. **Dynamics**&#x200B;にログインし、左下のメニューで **設定** (Settings)を選択します。

   ![](assets/image2015-4-2-11-3a32-3a53.png)

1. ツリーで **「Solutions** 」を選択します。

   ![](assets/image2015-4-2-11-3a35-3a28.png)

1. 「 **読み込み**」をクリックします。

   ![](assets/image2015-4-2-11-3a37-3a33.png)

1. 「 **参照**」をクリックします。 ダウンロードしたマーケティング担当者管理ソリューション [を選択します](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)。 「 **次へ**」をクリックします。

   ![](assets/image2015-4-2-11-3a40-3a33.png)

1. 「ソリューション情報」を表示し、「 **表示ソリューションパッケージの詳細**」をクリックします。

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. すべての詳細の確認が完了したら、「 **閉じる**」をクリックします。

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. ソリューション情報ページに戻り、「 **次へ**」をクリックします。

   ![](assets/image2015-4-2-11-3a41-3a48.png)

1. 「SDKメッセージオプション」チェックボックスがオンになっていることを確認します。 「 **次へ**」をクリックします。

   ![](assets/image2015-4-2-11-3a42-3a37.png)

   >[!TIP]
   >
   >インストールプロセスを完了するには、ブラウザーでポップアップを有効にする必要があります。

1. 次に、インポートが終了するのを待ちます。 起き上がって、何か手を伸ばして。

   ![](assets/image2015-4-2-11-3a43-3a51.png)

1. 「 **閉じる**」をクリックします。

   >[!NOTE]
   >
   >「Marketto Lead Management completed with warning」というメッセージが表示される場合があります。 これは完全に期待されています。

   ![](assets/image2015-4-2-11-3a44-3a44.png)

1. マーケティング担当者のリード管理が **すべてのソリューション** ページに表示されます。

   ![](assets/image2015-4-2-11-3a46-3a55.png)

1. 「マーケティング」「リード管理」を選択し、「すべてのカスタマイズを **発行」をクリックします。**

   ![](assets/image2015-4-2-11-3a48-3a21.png)

悪くなかった？ さあ、残りの部分を歩き続ける。

>[!CAUTION]
>
>Marketto SDKのメッセージングプロセスを無効にすると、インストールが中断されます。

>[!NOTE]
>
>**関連記事**
>
>[手順2/3:Dynamics (2011 On-Premises)でMarketo Syncユーザーを設定](step-2-of-3-set-up.md)
