---
unique-page-id: 30081815
description: Adobe Experience Manager統合の設定 — Marketoドキュメント — 製品ドキュメント
title: Adobe Experience Manager 統合の設定
exl-id: 06b2c214-1afb-443f-ae01-0c00fed77dce
source-git-commit: 47b0f31b410f0bf4b41740aa6440c2a0484ab835
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 11%

---

# Adobe Experience Manager 統合の設定 {#configuring-adobe-experience-manager-integration}

AEMアセットにアクセスし、選択し、Marketo Design Studio に読み込めるようにAEMを設定します。

>[!NOTE]
>
>**管理者権限が必要**

>[!CAUTION]
>
>現在、この機能は Firefox でのみ完全にサポートされています。Safari ではサポートされていないので、SameSite cookie の設定によっては、最新バージョンの Chrome では動作しない可能性があります。

1. Adobe Experience Managerに移動します（この URL は会社に固有のものです）。

   ![](assets/one.png)

1. ユーザーは、Adobeでログインするか、ローカルでログインすることができます。 この例では、ローカルでサインインします。

   ![](assets/two.png)

1. In **ツール**&#x200B;をクリックし、 **運用** を選択し、 **Web コンソール**.

   ![](assets/2a.png)

1. ブラウザーで、「AdobeGranite クロスオリジンリソース共有ポリシー」を検索 (Windows では ctrl+f、Macでは cmd+f) します。

   ![](assets/three.png)

1. 次をクリック： **+** 右側にサインします。

   ![](assets/four.png)

1. 内 **許可された起源（正規表現）** テキストボックス、入力 `https://.*\.marketo\.com` をクリックし、 **保存**.

   ![](assets/five-psd.png)

1. ページ上部のヘッダーで、 **Web コンソール** を選択し、 **システム情報**.

   ![](assets/six.png)

1. [ サーバ情報 ] で、 **再起動** 」ボタンをクリックします。

   ![](assets/seven.png)

1. クリック **OK** をクリックして確定します。

   ![](assets/eight.png)

1. Marketo Classicで、 **管理者**.

   ![](assets/nine.png)

1. 「統合」で、「 **Adobe Experience Manager**.

   ![](assets/ten.png)

1. 「**編集**」をクリックします。

   ![](assets/eleven.png)

1. AEM URL を入力し、 **OK**.

   ![](assets/twelve.png)

   準備は整った！ 次の操作を実行できます。 [AEMアセットを Design Studio のMarketo Skyに読み込む](https://experienceleague.adobe.com/docs/marketo/sky/design-studio/importing-assets-with-adobe-experience-manager.html?lang=en#design-studio).
