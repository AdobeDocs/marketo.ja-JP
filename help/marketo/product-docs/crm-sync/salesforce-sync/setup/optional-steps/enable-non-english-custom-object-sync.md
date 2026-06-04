---
unique-page-id: 4719302
description: Marketo sync ユーザーが英語以外の言語を使用している場合にカスタムオブジェクトの同期を有効にする方法について説明します。 Salesforceでsync user languageをEnglishに設定し、スキーマを更新します。
title: 英語以外のカスタムオブジェクト同期の有効化
exl-id: 5d1c5b52-5323-4f68-847b-7d24e6acd6c4
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/kPzDEdjDnDAvuJmCtPj0I2Lfl63Lset00t-LwB8DDhI
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: 67c57a9162946c4b9c424ab3fd445b70e90b530a
workflow-type: tm+mt
source-wordcount: 195
ht-degree: 35%

---

# 英語以外のカスタムオブジェクト同期の有効化 {#enable-non-english-custom-object-sync}

Marketo 同期ユーザーが英語以外の言語に設定されている場合、カスタムオブジェクト同期を有効にしようとするとエラーが発生することがあります。

![](assets/image2014-12-10-13-3a17-3a51.png)

## 解決方法 {#how-to-fix}

1. Marketo 同期ユーザを使用して [!DNL Salesforce] にログインします。

   ![](assets/image2014-12-10-13-3a18-3a1.png)

1. ユーザー名ドロップダウンをクリックし、**[!UICONTROL 設定]**&#x200B;を選択します。

   ![](assets/image2014-12-10-13-3a18-3a11.png)

1. 「**[!UICONTROL 個人情報]**」で、「**[!UICONTROL 個人情報]**」をクリックします。

   ![](assets/image2014-12-10-13-3a18-3a22.png)

1. 「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/image2014-12-10-13-3a18-3a32.png)

1. 「**[!UICONTROL 言語]**」を&#x200B;**[!UICONTROL 英語]**&#x200B;に変更します。

   ![](assets/image2014-12-10-13-3a18-3a45.png)

1. 「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2014-12-10-13-3a18-3a55.png)

1. [Adobe Account Profile](https://account.adobe.com/profile){target="_blank"}で、**[!UICONTROL Preferred languages]**&#x200B;までスクロールして、最初の言語が英語に設定されていることを確認します。

   ![](assets/enable-non-english-custom-object-sync-step-6.5.png)

1. Marketo Engageで、**[!UICONTROL 管理者]** > **[!UICONTROL Salesforce]** > **[!UICONTROL オブジェクト]**&#x200B;に移動します。 「**[!UICONTROL スキーマを更新]**」をクリックします。

   ![](assets/image2014-12-10-13-3a19-3a6.png)

1. これは英語でオブジェクトリストを引き出します。 目的のオブジェクトを選択し、**[!UICONTROL 同期を有効にする]**&#x200B;をクリックします。

   ![](assets/image2014-12-10-13-3a19-3a16.png)

1. カスタムオブジェクトが有効になり、同期されます。

   ![](assets/image2014-12-10-13-3a19-3a26.png)

1. [!DNL Salesforce]に戻り、上記の手順を使用して、同期ユーザーを目的の言語に戻します。

>[!NOTE]
>
>オブジェクトを言語に戻すために、スキーマを最後に1回更新します。
