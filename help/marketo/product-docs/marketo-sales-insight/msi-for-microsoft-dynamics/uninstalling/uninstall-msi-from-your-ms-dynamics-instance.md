---
unique-page-id: 37355600
description: MS Dynamicsインスタンス — Marketto Docs — 製品ドキュメントからMSIをアンインストールします
title: MS DynamicsインスタンスからMSIをアンインストールする
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 0%

---


# MS Dynamicsインスタンス{#uninstall-msi-from-your-ms-dynamics-instance}からMSIをアンインストールします

MS DynamicsインスタンスからMSIをアンインストールするには、MarketorとMS Dynamicsの両方で手順を実行する必要があります。

>[!PREREQUISITES]
>
>[グローバルMS Dynamics同期を無効にする](http://docs.marketo.com/x/TAA6Ag)

1. Marketoで、「**管理者**」をクリックします。

   ![](assets/one-1.png)

1. 「**Sales Insight**」をクリックします。

   ![](assets/six.png)

1. 「**フィールドの同期を編集**」をクリックします。

   ![](assets/seven.png)

1. 「**同期を無効にする**」チェックボックスを選択し、「**保存**」をクリックします。

   >[!NOTE]
   >
   >**Reminder**
   >
   >
   >フィールドの同期を無効にする前に、グローバルMS Dynamics同期](http://docs.marketo.com/x/TAA6Ag)を[無効にしてください。

   ![](assets/eight.png)

## MS Dynamicsインスタンスでは、次の手順が実行されます。{#the-following-steps-take-place-in-your-ms-dynamics-instance}

1. 「**詳細設定**」をクリックします。
1. 「**ソリューション**」をクリックします。
1. **Marketto Sales Insight**&#x200B;を選択し、削除アイコンをクリックします。
1. 「Uninstall Solution」モーダルがポップアップ表示されたら、「**OK**」をクリックします。

   MS Dynamicsソリューションが完全にアンインストールされるまで、通常は約20分かかります。 ただし、大きなMS Dynamicsインスタンスがある場合は、少し時間がかかる場合があります。

   >[!NOTE]
   >
   >**Reminder**
   >
   >
   >MSIをアンインストールした後は、Global MS Dynamicsの同期を必ず有効にしてください。

