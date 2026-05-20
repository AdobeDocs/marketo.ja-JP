---
unique-page-id: 30081815
description: Adobe Experience ManagerとMarketoの連携を設定する方法について説明します。 AEMを設定し、アセットにアクセスしてDesign Studioに読み込めるようにします。
title: Adobe Experience Manager 統合の設定
hide: true
exl-id: 06b2c214-1afb-443f-ae01-0c00fed77dce
feature: Integrations
TQID: https://experienceleague.adobe.com/nJBydVi8mRwVf1vAIFuI1S3nEuX0FGiztp8fhRHq6RM
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: d65b4a73-87a3-4d56-b638-74e74d9939ce
  - id: e2290edd-b061-4880-9d79-dee306cf5aa9
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 229
ht-degree: 87%

---

# Adobe Experience Manager 統合の設定 {#configuring-adobe-experience-manager-integration}

Adobe Experience Manager（AEM）を設定し、AEM のアセットにアクセスして選択し、Marketo Engage デザインスタジオに読み込めるようにします。

>[!NOTE]
>
>**管理者権限が必要**

>[!IMPORTANT]
>
>* この統合は、AEM のオンプレミス実装でのみ機能し、AEM Cloud Service 実装ではサポートされません。
>
>* 現在、この機能は Firefox でのみ完全にサポートされています。 Safari ではサポートされていません。また、SameSite の Cookie 設定によっては、最新バージョンの Chrome では動作しない可能性があります。

1. Adobe Experience Manager に移動します（URL は会社に固有のものです）。

   ![](assets/one.png)

1. ユーザは、アドビでログインするか、ローカルでログインできます。 この例では、ローカルログインを使用します。

   ![](assets/two.png)

1. 「**[!UICONTROL ツール]**」で、「**[!UICONTROL 運用]**」をクリックし、「**[!UICONTROL web コンソール]**」を選択します。

   ![](assets/2a.png)

1. ブラウザーで、「[!UICONTROL Adobe Granite クロスオリジンリソース共有ポリシー]」を検索します（Windows では Ctrl + F キー、Mac では Cmd + F キー）。

   ![](assets/three.png)

1. 右側の「**+**」記号をクリックします。

   ![](assets/four.png)

1. 「**[!UICONTROL 許可済み接触チャネル（正規表現）]**」テキストボックスに、`https://.*\.marketo\.com` と入力し、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/five-psd.png)

1. ページ上部のヘッダーで、「**[!UICONTROL Web コンソール]**」を選択し、「**[!UICONTROL システム情報]**」を選択します。

   ![](assets/six.png)

1. 「サーバー情報」で、「**[!UICONTROL 再起動]**」ボタンをクリックします。

   ![](assets/seven.png)

1. 「**[!UICONTROL OK]**」をクリックして続行します。

   ![](assets/eight.png)

1. Marketo Engage で、「**[!UICONTROL 管理者]**」をクリックします。

   ![](assets/nine.png)

1. 「統合」で、「**[!UICONTROL Adobe Experience Manager]**」を選択します。

   ![](assets/ten.png)

1. 「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/eleven.png)

1. AEM の URL を入力し、「**[!UICONTROL OK]**」をクリックします。

   ![](assets/twelve.png)
