---
unique-page-id: 30081815
description: Adobe Experience Manager 統合の設定 - Marketo ドキュメント - 製品ドキュメント
title: Adobe Experience Manager 統合の設定
exl-id: 06b2c214-1afb-443f-ae01-0c00fed77dce
source-git-commit: 47b0f31b410f0bf4b41740aa6440c2a0484ab835
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 89%

---

# Adobe Experience Manager 統合の設定 {#configuring-adobe-experience-manager-integration}

AEM のアセットにアクセス、選択し、Marketo Design Studio に読み込めるように AEM を設定します。

>[!NOTE]
>
>**管理者権限が必要**

>[!CAUTION]
>
>現在、この機能は Firefox でのみ完全にサポートされています。Safari ではサポートされていないので、SameSite cookie の設定によっては、最新バージョンの Chrome では動作しない可能性があります。

1. Adobe Experience Manager に移動します（URL は会社に固有のものです）。

   ![](assets/one.png)

1. ユーザーは、アドビでログインするか、ローカルでログインできます。この例では、ローカルでログインします。

   ![](assets/two.png)

1. **ツール**&#x200B;で「**運用**」を選択し、「**Web コンソール**」を選択します。

   ![](assets/2a.png)

1. ブラウザーで、「Adobe Granite Cross-Origin Resource Sharing Policy」を検索します（Windows では Ctrl + F キー、Mac では Cmd + F キー）。

   ![](assets/three.png)

1. 右側の「**+**」記号をクリックします。

   ![](assets/four.png)

1. 「**許可済み接触チャネル（正規表現）**」テキストボックスに、`https://.*\.marketo\.com` と入力し、「**保存**」をクリックします。

   ![](assets/five-psd.png)

1. ページ上部のヘッダーで、「**Web コンソール**」を選択し、「**システム情報**」を選択します。

   ![](assets/six.png)

1. 「サーバー情報」で、「**再起動**」ボタンをクリックします。

   ![](assets/seven.png)

1. 「**OK**」をクリックして続行します。

   ![](assets/eight.png)

1. Marketo Classic で、「**管理者**」をクリックします。

   ![](assets/nine.png)

1. 「統合」で、「**Adobe Experience Manager**」を選択します。

   ![](assets/ten.png)

1. 「**編集**」をクリックします。

   ![](assets/eleven.png)

1. AEM の URL を入力し、「**OK**」をクリックします。

   ![](assets/twelve.png)

   準備完了です。これで、[AEM のアセットを Marketo Sky の Design Studio にインポート](https://experienceleague.adobe.com/docs/marketo/sky/design-studio/importing-assets-with-adobe-experience-manager.html?lang=jp#design-studio)できます。
