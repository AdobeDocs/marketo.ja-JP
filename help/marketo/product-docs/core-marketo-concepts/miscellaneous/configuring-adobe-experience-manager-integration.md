---
unique-page-id: 30081815
description: Adobe Experience Manager統合の設定 — Marketto Docs — 製品ドキュメント
title: Adobe Experience Manager統合の設定
translation-type: tm+mt
source-git-commit: e5050328cbddaf072dd60ddd8d7363a704e720b5
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---


# Adobe Experience Manager統合の設定{#configuring-adobe-experience-manager-integration}

AEMアセットにアクセス、選択およびMarketorのDesign Studioへの読み込みができるようにAEMを設定します。

>[!NOTE]
>
>**必要な管理者権限**

>[!CAUTION]
>
>現在、この機能はFirefoxでのみ完全にサポートされています。 Safariではサポートされていないため、SameSite Cookieの設定によっては、最新バージョンのChrome(v. 80)では動作しない場合があります。

1. Adobe Experience Managerに移動します(URLは会社に固有です)。

   ![](assets/one.png)

1. Adobeを使用してサインインするか、ローカルでサインインすることができます。 この例では、ローカルにサインインします。

   ![](assets/two.png)

1. **ツール**&#x200B;で、**操作**&#x200B;をクリックし、**Webコンソール**&#x200B;を選択します。

   ![](assets/2a.png)

1. ブラウザーで、（Windowsではctrl + fキー、Macではcmd + fキー）に対して「AdobeGranite Cross-接触チャネルリソース共有ポリシー」を検索します。

   ![](assets/three.png)

1. 右側の&#x200B;**+**&#x200B;記号をクリックします。

   ![](assets/four.png)

1. 「**許可されている接触チャネル(Regexp)**」テキストボックスに、`https://.*\.marketo\.com`に入力し、「**保存**」をクリックします。

   ![](assets/five-psd.png)

1. ページ上部のヘッダーで、「**Webコンソール**」をクリックし、「**システム情報**」を選択します。

   ![](assets/six.png)

1. 「Server Information」で、「**Restart**」ボタンをクリックします。

   ![](assets/seven.png)

1. 「**OK**」をクリックして確認します。

   ![](assets/eight.png)

1. Marketo Classicで、「**管理者**」をクリックします。

   ![](assets/nine.png)

1. 「統合」で、**Adobe Experience Manager**&#x200B;を選択します。

   ![](assets/ten.png)

1. 「**編集**」をクリックします。

   ![](assets/eleven.png)

1. AEM URLを入力し、「**OK**」をクリックします。

   ![](assets/twelve.png)

   準備万端！ これで、Marketo Sky](https://help.marketo.com/hc/en-us/articles/360036765993)のDesign StudioにAEMアセットを[読み込むことができるようになりました。
