---
unique-page-id: 10098759
description: MarketoでFacebook リード広告モバイル統合をテストする方法について説明します。 モバイルから送信されたリードと送信を正しく同期します。
title: Marketo とのモバイル統合に向けた Facebook リード広告のテスト
exl-id: 0c381c53-f97a-4e1d-b44d-5ee6521ac990
feature: Integrations
TQID: https://experienceleague.adobe.com/VrGVY61VlAmqLgSm6r2lCFHed5Cqn88mojgKZpP9-Lg
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 221
ht-degree: 61%

---

# Marketo とのモバイル統合に向けた [!DNL Facebook] リード広告のテスト {#test-facebook-lead-ads-for-mobile-integration-with-marketo}

リード広告を作成したら、テストする必要があります。

>[!PREREQUISITES]
>
>[[!UICONTROL Facebook リード広告]の統合を設定](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)する必要があります。

1. [!UICONTROL Facebook Power Editor] で、キャンペーンと広告を選択し、「**[!UICONTROL 編集]**」をクリックします。

1. 「**[!UICONTROL リンク]**」で、「**[!UICONTROL モバイルアプリで表示]**」リンクをクリックします。

   ![](assets/image2016-5-13-15-3a2-3a38.png)

1. 新しい通知が [!DNL Facebook] アカウントに送信され、認証済みアカウントでモバイルデバイスからアクセスできるようになります。 「**[!UICONTROL OK]**」をクリックします。

   ![](assets/image2016-3-11-8-3a35-3a7.png)

1. モバイルデバイスで、[!DNL Facebook] モバイルアプリの「**[!UICONTROL 通知]**」をタップします。

   ![](assets/image2016-3-11-8-3a38-3a35.png)

1. 「通知」で、「**[!UICONTROL 広告をプレビューする準備が整いました]**」をタップします。

   ![](assets/image2016-3-11-8-3a41-3a59.png)

1. コールトゥアクションをタップし、作成したフォームに入力して、テスト用リード広告ユニットを送信します。

   ![](assets/image2016-3-11-8-3a52-3a20.png)

   >[!NOTE]
   >
   >この例では、Call to actionの詳細を使用します。 リード広告ユニットのコールトゥアクションは異なる可能性があります。

1. フォームを送信した後、プログラムの一部として、または&#x200B;**[!UICONTROL Filled Out Facebook Lead Ads Form]** フィルターを使用するリードデータベースの一部として、[Marketo](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)でスマートリストを作成します。 送信したフォームのリードとフォーム名を挿入します。

   ![](assets/image2016-3-11-8-3a59-3a34.png)

1. 次に、「リード」タブをクリックして、同期が正しく機能していることを検証します。

   ![](assets/image2016-3-11-15-3a27-3a54.png)

>[!NOTE]
>
>[[!UICONTROL Facebook リード広告]](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)の設定
