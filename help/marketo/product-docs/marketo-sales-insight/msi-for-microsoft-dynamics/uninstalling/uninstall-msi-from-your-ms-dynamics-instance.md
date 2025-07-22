---
unique-page-id: 37355600
description: MS [!DNL Dynamics] Instance から MSI をアンインストールする – Marketo ドキュメント – 製品情報
title: MS [!DNL Dynamics] Instance から MSI をアンインストールする
exl-id: 86e8dbc9-236f-42ad-96e8-cdb1b4c3bed2
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 38%

---

# MS [!DNL Dynamics] インスタンスから MSI をアンインストールする {#uninstall-msi-from-your-ms-dynamics-instance}

MS [!DNL Dynamics] インスタンスから MSI をアンインストールするには、Marketoと MS [!DNL Dynamics] の両方で手順を実行する必要があります。

>[!PREREQUISITES]
>
>[ グローバル MS [!DNL Dynamics] Sync の無効化 ](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/uninstalling/disable-global-ms-dynamics-sync.md)

1. Marketo で、「**[!UICONTROL 管理者]**」をクリックします。

   ![](assets/one-1.png)

1. 「**[!UICONTROL Sales Insight]**」をクリックします。

   ![](assets/six.png)

1. 「**[!UICONTROL フィールド同期を編集]**」をクリックします。

   ![](assets/seven.png)

1. 「**[!UICONTROL 同期を無効にする]**」チェックボックスを選択して、「**[!UICONTROL 保存]**」をクリックします。

   >[!NOTE]
   >
   >フィールドの同期を無効にする前に、必ず[グローバル MS Dynamics 同期](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/uninstalling/disable-global-ms-dynamics-sync.md)を無効にしてください。

   ![](assets/eight.png)

## 次の手順は、MS [!DNL Dynamics] インスタンスで実行します。 {#the-following-steps-take-place-in-your-ms-dynamics-instance}

1. 「**[!UICONTROL 詳細設定]**」をクリックします。

1. 「**[!UICONTROL ソリューション]**」をクリックします。

1. **[!UICONTROL Marketo Sales Insight]** を選択し、削除アイコンをクリックします。

1. ソリューションをアンインストールモーダルが表示されたら、「**[!UICONTROL OK]**」をクリックします。

   MS [!DNL Dynamics] ソリューションが完全にアンインストールされるまで、通常は約 20 分かかります。 ただし、MS [!DNL Dynamics] インスタンスが大きい場合は、少し時間がかかる場合があります。

   >[!NOTE]
   >
   >MSI をアンインストールしたら、必ずグローバル MS [!DNL Dynamics] 同期を有効にしてください。
