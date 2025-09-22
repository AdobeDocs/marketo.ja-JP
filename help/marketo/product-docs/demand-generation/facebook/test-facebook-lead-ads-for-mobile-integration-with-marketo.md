---
unique-page-id: 10098759
description: Marketo とのモバイル統合に向けた Facebook リード広告のテスト - Marketo ドキュメント - 製品ドキュメント
title: Marketo とのモバイル統合に向けた Facebook リード広告のテスト
exl-id: 0c381c53-f97a-4e1d-b44d-5ee6521ac990
feature: Integrations
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 100%

---

# Marketo とのモバイル統合に向けた [!DNL Facebook] リード広告のテスト {#test-facebook-lead-ads-for-mobile-integration-with-marketo}

リード広告を作成した後、テストする必要があります。

>[!PREREQUISITES]
>
>[[!UICONTROL Facebook リード広告]の統合を設定](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)する必要があります。

1. [!UICONTROL Facebook Power Editor] で、キャンペーンと広告を選択し、「**[!UICONTROL 編集]**」をクリックします。

1. 「**[!UICONTROL リンク]**」で、「**[!UICONTROL モバイルアプリで表示]**」リンクをクリックします。

   ![](assets/image2016-5-13-15-3a2-3a38.png)

1. 新しい通知が [!DNL Facebook] アカウントに送信され、認証済みアカウントでモバイルデバイスからアクセスできるようになります。「**[!UICONTROL OK]**」をクリックします。

   ![](assets/image2016-3-11-8-3a35-3a7.png)

1. モバイルデバイスで、[!DNL Facebook] モバイルアプリの「**[!UICONTROL 通知]**」をタップします。

   ![](assets/image2016-3-11-8-3a38-3a35.png)

1. 「通知」で、「**[!UICONTROL 広告をプレビューする準備が整いました]**」をタップします。

   ![](assets/image2016-3-11-8-3a41-3a59.png)

1. コールトゥアクションをタップし、作成したフォームに入力して、テスト用リード広告ユニットを送信します。

   ![](assets/image2016-3-11-8-3a52-3a20.png)

   >[!NOTE]
   >
   >これは、「詳細コールトゥアクション」を使用する一例です。リード広告ユニットのコールトゥアクションは異なる可能性があります。

1. 魔法が起こるのはここです。フォームを送信したら、「**[!UICONTROL Facebook リード広告フォームに入力済み]**」フィルターを使用するプログラムの一部またはデータベース内で [Marketo のスマートリストを作成](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)します。先ほど送信したフォームのリード広告フォーム名を挿入します。

   ![](assets/image2016-3-11-8-3a59-3a34.png)

1. 次に、「リード」タブをクリックして、同期が正しく機能していることを検証します。

   ![](assets/image2016-3-11-15-3a27-3a54.png)

凄いでしょう。

>[!NOTE]
>
>[[!UICONTROL Facebook リード広告の有効化／無効化]](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)
