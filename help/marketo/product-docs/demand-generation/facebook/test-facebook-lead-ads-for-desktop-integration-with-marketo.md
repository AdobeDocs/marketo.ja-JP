---
unique-page-id: 11370892
description: Marketoと Facebook リード広告のデスクトップ統合をテストする方法について説明します。 デスクトップからのリード広告の送信内容が正しく同期されていることを確認します。
title: Marketo とのデスクトップ統合に向けた Facebook リード広告のテスト
exl-id: 2025b6e9-ecd7-4677-9f76-bc7813884e93
feature: Integrations
source-git-commit: 031eb5f3ff8aac185ce496664f984a4c745c6e44
workflow-type: tm+mt
source-wordcount: '224'
ht-degree: 91%

---

# Marketo とのデスクトップ統合に向けた [!DNL Facebook] リード広告のテスト {#test-facebook-lead-ads-for-desktop-integration-with-marketo}

リード広告を作成した後、テストする必要があります。デスクトップでの実行方法を次に示します。

>[!PREREQUISITES]
>
>[[!UICONTROL Facebook リード広告]の統合を設定](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)する必要があります。

1. Facebook Power Editor で、キャンペーンと広告を選択し、「**[!UICONTROL 編集]**」をクリックします。

1. **[!UICONTROL リンク]**&#x200B;の下で、「**[!UICONTROL ニュースフィードで表示]**」リンクをクリックします。

   ![](assets/image2016-5-13-14-3a35-3a36.png)

1. ブラウザーの新しいタブで [!DNL Facebook] に移動します。[!DNL Facebook] リード広告ユニットの「[!UICONTROL コールトゥアクション]」をクリックします。

   ![](assets/image2016-5-13-14-3a42-3a45.png)

   >[!NOTE]
   >
   >これは、「詳細コールトゥアクション」を使用する一例です。リード広告ユニットのコールトゥアクションは異なる可能性があります。

1. デスクトップのフォームに入力して、テスト用リード広告ユニットを送信します。「**[!UICONTROL 送信]**」をクリックします。

   ![](assets/image2016-5-13-14-3a47-3a43.png)

1. おめでとうございます。リード広告フォームの送信が完了しました。

   ![](assets/image2016-5-13-14-3a52-3a57.png)

1. 魔法が起こるのはここです。フォームを送信したら、「[!DNL Facebook] リード広告フォームに入力済み」フィルターを使用するプログラムの一部またはデータベース内で [Marketo のスマートリストを作成](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)します。先ほど送信したフォームのリード広告フォーム名を挿入します。

   ![](assets/image2016-3-11-8-3a59-3a34-1.png)

1. 次に、「**[!UICONTROL ユーザー]**」タブをクリックして、同期が正しく動作していることを確認します。

   ![](assets/people.png)

   凄いでしょう。

>[!MORELIKETHIS]
>
>[[!UICONTROL Facebook リード広告]](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)の設定
