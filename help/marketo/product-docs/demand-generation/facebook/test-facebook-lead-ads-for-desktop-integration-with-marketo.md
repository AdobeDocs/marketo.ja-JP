---
unique-page-id: 11370892
description: MarketoでFacebook リード広告のデスクトップ統合をテストする方法について説明します。 デスクトップから送信されたリードと送信が正しく同期されていることを確認します。
title: Marketo とのデスクトップ統合に向けた Facebook リード広告のテスト
exl-id: 2025b6e9-ecd7-4677-9f76-bc7813884e93
feature: Integrations
source-git-commit: d20c398cd1f5ed2646f56995c35a57630c3f2e95
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 47%

---

# Marketo とのデスクトップ統合に向けた [!DNL Facebook] リード広告のテスト {#test-facebook-lead-ads-for-desktop-integration-with-marketo}

リード広告を作成したら、テストする必要があります。 次の手順に従って、デスクトップで行います。

>[!PREREQUISITES]
>
>[[!UICONTROL Facebook リード広告]の統合を設定](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)する必要があります。

1. Facebook Power Editor で、キャンペーンと広告を選択し、「**[!UICONTROL 編集]**」をクリックします。

1. **[!UICONTROL リンク]**&#x200B;の下で、「**[!UICONTROL ニュースフィードで表示]**」リンクをクリックします。

   ![](assets/image2016-5-13-14-3a35-3a36.png)

1. ブラウザーの新しいタブで[!DNL Facebook]へ移動します。 [!DNL Facebook] リード広告ユニットの「[!UICONTROL コールトゥアクション]」をクリックします。

   ![](assets/image2016-5-13-14-3a42-3a45.png)

   >[!NOTE]
   >
   >この例では、Call to actionの詳細を使用します。 リード広告ユニットのコールトゥアクションは異なる可能性があります。

1. デスクトップのフォームに入力して、テスト用リード広告ユニットを送信します。 「**[!UICONTROL 送信]**」をクリックします。

   ![](assets/image2016-5-13-14-3a47-3a43.png)

1. リード広告フォームの送信が完了しました。

   ![](assets/image2016-5-13-14-3a52-3a57.png)

1. フォームを送信した後、プログラムの一部として、または塗りつぶされた[!DNL Facebook] リード広告フォーム フィルターを使用するデータベースの一部として、[Marketo](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)でスマートリストを作成します。 送信したフォームのリードとフォーム名を挿入します。

   ![](assets/image2016-3-11-8-3a59-3a34-1.png)

1. 次に、「**[!UICONTROL ユーザー]**」タブをクリックして、同期が正しく動作していることを確認します。

   ![](assets/people.png)

>[!MORELIKETHIS]
>
>[[!UICONTROL Facebook リード広告]](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)の設定
