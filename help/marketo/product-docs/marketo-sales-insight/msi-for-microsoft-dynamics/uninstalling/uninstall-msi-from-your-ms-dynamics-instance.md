---
unique-page-id: 37355600
description: MS DynamicsインスタンスからMSIをアンインストールします —Marketoドキュメント — 製品ドキュメント
title: MS DynamicsインスタンスからMSIをアンインストールする
exl-id: 86e8dbc9-236f-42ad-96e8-cdb1b4c3bed2
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '156'
ht-degree: 0%

---

# MS Dynamicsインスタンス{#uninstall-msi-from-your-ms-dynamics-instance}からMSIをアンインストールします

MS DynamicsインスタンスからMSIをアンインストールするには、MarketoとMS Dynamicsの両方で手順を実行する必要があります。

>[!PREREQUISITES]
>
>[グローバルMS Dynamics同期を無効にする](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/uninstalling/disable-global-ms-dynamics-sync.md)

1. Marketoで、**管理者**&#x200B;をクリックします。

   ![](assets/one-1.png)

1. 「**Sales Insight**」をクリックします。

   ![](assets/six.png)

1. 「**フィールドの同期を編集**」をクリックします。

   ![](assets/seven.png)

1. 「**同期を無効にする**」チェックボックスを選択し、「**保存**」をクリックします。

   >[!NOTE]
   >
   >フィールドの同期を無効にする前に、グローバルMS Dynamics同期](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/uninstalling/disable-global-ms-dynamics-sync.md)を[無効にしてください。

   ![](assets/eight.png)

## MS Dynamicsインスタンスでは、次の手順が実行されます。{#the-following-steps-take-place-in-your-ms-dynamics-instance}

1. 「**詳細設定**」をクリックします。

1. 「**ソリューション**」をクリックします。

1. 「**Marketo販売インサイト**」を選択し、削除アイコンをクリックします。

1. 「Uninstall Solution」モーダルがポップアップ表示されたら、「**OK**」をクリックします。

   MS Dynamicsソリューションが完全にアンインストールされるまで、通常は約20分かかります。 ただし、大きなMS Dynamicsインスタンスがある場合は、少し時間がかかる場合があります。

   >[!NOTE]
   >
   >MSIをアンインストールした後は、Global MS Dynamicsの同期を必ず有効にしてください。
