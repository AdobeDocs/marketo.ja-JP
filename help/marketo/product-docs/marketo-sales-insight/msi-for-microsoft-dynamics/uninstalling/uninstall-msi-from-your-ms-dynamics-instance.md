---
unique-page-id: 37355600
description: MS Dynamics インスタンスからMarketo Sales Insightをアンインストールする方法について説明します。 解決策を削除し、必要に応じてクリーンアップします。
title: MS  [!DNL Dynamics]  インスタンスから MSI をアンインストール
exl-id: 86e8dbc9-236f-42ad-96e8-cdb1b4c3bed2
feature: Marketo Sales Insights
TQID: https://experienceleague.adobe.com/tv5uoDyp6czOdjx3D1RDZUtoDTaaZniVF5fZDWnxPPk
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
topic_v2: id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 156
ht-degree: 87%

---

# MS [!DNL Dynamics] インスタンスから MSI をアンインストール {#uninstall-msi-from-your-ms-dynamics-instance}

MS [!DNL Dynamics] インスタンスから MSI をアンインストールするには、Marketo と MS [!DNL Dynamics] の両方で手順を実行する必要があります。

>[!PREREQUISITES]
>
>[グローバル MS  [!DNL Dynamics]  同期の無効化](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/uninstalling/disable-global-ms-dynamics-sync.md)

1. Marketo で、「**[!UICONTROL 管理者]**」をクリックします。

   ![](assets/one-1.png)

1. 「**[!UICONTROL セールスインサイト]**」をクリックします。

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

1. **[!UICONTROL Marketo セールスインサイト]**&#x200B;を選択し、削除アイコンをクリックします。

1. ソリューションをアンインストールモーダルが表示されたら、「**[!UICONTROL OK]**」をクリックします。

   MS [!DNL Dynamics] ソリューションが完全にアンインストールされるまで、通常 20 分ほどかかります。 ただし、大きな MS [!DNL Dynamics] インスタンスがある場合は、もう少し時間がかかる場合があります。

   >[!NOTE]
   >
   >MSI をアンインストールしたら、必ずグローバル MS [!DNL Dynamics] 同期をオンにしてください。
