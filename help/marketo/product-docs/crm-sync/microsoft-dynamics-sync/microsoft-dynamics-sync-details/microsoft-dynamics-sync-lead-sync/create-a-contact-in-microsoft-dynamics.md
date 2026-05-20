---
unique-page-id: 10095389
description: MarketoからMicrosoft Dynamicsで連絡先を作成する方法を説明します。 トリガーキャンペーンで「人物をMicrosoftに同期」フローアクションを使用すると、リアルタイムの連絡先を作成できます。
title: Microsoft Dynamics での取引先責任者の作成
exl-id: 66cb26c0-f383-4d1e-be22-e7f8c6b266fb
feature: Microsoft Dynamics
TQID: https://experienceleague.adobe.com/5q84B57P88MNhaYHluCKKCYLwOonW2xj7hAUNDOmXl8
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 136
ht-degree: 79%

---

# [!DNL Microsoft Dynamics] での取引先責任者の作成 {#create-a-contact-in-microsoft-dynamics}

1. Dynamics で取引先責任者として作成する Marketo Engage 専用の人物（Microsoft タイプが空）を選択します。

   ![](assets/one.png)

1. **[!UICONTROL 人物アクション]**／**[!DNL Microsoft]** をクリックし、「**[!UICONTROL 人物を Microsoft に同期]**」を選択します。

   ![](assets/two.png)

1. 「**[!UICONTROL 名前を付けて同期]**」をクリックし、「**[!UICONTROL 連絡先]**」を選択します。 「**[!UICONTROL 今すぐ実行]**」をクリックします。

   ![](assets/three.png)

   >[!NOTE]
   >
   >「[!UICONTROL 人物を Microsoft に同期]」フローアクション（トリガーキャンペーン内のみ）を使用すると、Dynamics でリード／取引先責任者がリアルタイムで作成されます。

1. Marketo は、[!DNL Dynamics] のリードレコードを、[!DNL Dynamics] のどのアカウントにも関連付けられていない取引先責任者に限定します。

   ![](assets/image2015-10-23-9-3a43-3a33.png)

1. スマートキャンペーンフィルターで「名前を付けて同期」制約を使用する場合に「**[!UICONTROL 取引先責任者]**」を選択できるようになります。

   ![](assets/five.png)
