---
unique-page-id: 37355600
description: MS Dynamics インスタンスから MSI をアンインストール - Marketo ドキュメント - 製品ドキュメント
title: MS Dynamics インスタンスから MSI をアンインストール
exl-id: 86e8dbc9-236f-42ad-96e8-cdb1b4c3bed2
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '156'
ht-degree: 100%

---

# MS Dynamics インスタンスから MSI をアンインストール {#uninstall-msi-from-your-ms-dynamics-instance}

MS Dynamics インスタンスから MSI をアンインストールするには、Marketo と MS Dynamics の両方で手順を実行する必要があります。

>[!PREREQUISITES]
>
>[グローバル MS Dynamics 同期の無効化](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/uninstalling/disable-global-ms-dynamics-sync.md)

1. Marketo で、「**管理者**」をクリックします。

   ![](assets/one-1.png)

1. 「**Sales Insight**」をクリックします。

   ![](assets/six.png)

1. 「**フィールド同期を編集**」をクリックします。

   ![](assets/seven.png)

1. 「**同期を無効にする**」チェックボックスを選択して、「**保存**」をクリックします。

   >[!NOTE]
   >
   >フィールドの同期を無効にする前に、必ず[グローバル MS Dynamics 同期](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/uninstalling/disable-global-ms-dynamics-sync.md)を無効にしてください。

   ![](assets/eight.png)

## 次の手順は、MS Dynamics インスタンスで実行します。 {#the-following-steps-take-place-in-your-ms-dynamics-instance}

1. 「**詳細設定**」をクリックします。

1. 「**ソリューション**」をクリックします。

1. **Marketo Sales Insight** を選択し、削除アイコンをクリックします。

1. ソリューションをアンインストールモーダルが表示されたら、「**OK**」をクリックします。

   MS Dynamics ソリューションが完全にアンインストールされるまで、通常 20 分ほどかかります。ただし、大きな MS Dynamics インスタンスがある場合は、もう少し時間がかかる場合があります。

   >[!NOTE]
   >
   >MSI をアンインストールしたら、必ずグローバル MS Dynamics 同期をオンにしてください。
