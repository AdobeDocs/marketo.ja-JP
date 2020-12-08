---
unique-page-id: 37355600
description: MS Dynamicsインスタンス — Marketto Docs — 製品ドキュメントからMSIをアンインストールします
title: MS DynamicsインスタンスからMSIをアンインストールする
translation-type: tm+mt
source-git-commit: 23428a6e0ba9b2108a8f2f7dd6a69929dd069834
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 0%

---


# MS DynamicsインスタンスからMSIをアンインストールする {#uninstall-msi-from-your-ms-dynamics-instance}

MS DynamicsインスタンスからMSIをアンインストールするには、MarketorとMS Dynamicsの両方で手順を実行する必要があります。

>[!NOTE]
>
>**前提条件**
>
>[グローバルMS Dynamics同期を無効にする](http://docs.marketo.com/x/TAA6Ag)

1. Marketorで、「 **管理者**」をクリックします。

   ![](assets/one-1.png)

1. [ **販売インサイト**]をクリックします。

   ![](assets/six.png)

1. [フィールドの同期 **の編集**]をクリックします。

   ![](assets/seven.png)

1. 「同期を **無効にする** 」チェックボックスを選択し、「 **保存**」をクリックします。

   >[!NOTE]
   >
   >**Reminder**
   >
   >
   >フィールドの同期を無効にする前に、Global MS Dynamics Sync [を](http://docs.marketo.com/x/TAA6Ag) 無効にしてください。

   ![](assets/eight.png)

## MS Dynamicsインスタンスでは、次の手順が実行されます。 {#the-following-steps-take-place-in-your-ms-dynamics-instance}

1. 「 **詳細設定**」をクリックします。
1. 「 **ソリューション**」をクリックします。
1. 「 **Marketor Sales Insight** 」を選択し、削除アイコンをクリックします。
1. 「アンインストールソリューション」モーダルがポップアップ表示されたら、「 **OK**」をクリックします。

   MS Dynamicsソリューションが完全にアンインストールされるまで、通常は約20分かかります。 ただし、大きなMS Dynamicsインスタンスがある場合は、少し時間がかかる場合があります。

   >[!NOTE]
   >
   >**Reminder**
   >
   >
   >MSIをアンインストールした後は、Global MS Dynamicsの同期を必ず有効にしてください。

