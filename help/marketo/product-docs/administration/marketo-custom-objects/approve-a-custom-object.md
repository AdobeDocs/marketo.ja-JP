---
unique-page-id: 10094188
description: カスタムオブジェクトの承認 - Marketo ドキュメント - 製品ドキュメント
title: カスタムオブジェクトの承認
exl-id: 8bae94df-91fe-4722-8c75-c26df882c65d
feature: Custom Objects
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 100%

---

# カスタムオブジェクトの承認 {#approve-a-custom-object}

カスタムオブジェクトを使用するには、その前にカスタムオブジェクトを承認する必要があります。新しいカスタムオブジェクトと編集したカスタムオブジェクトでは、プロセスが少し異なります。

## 新規カスタムオブジェクトの承認 {#approve-a-new-custom-object}

新しいカスタムオブジェクトを作成したら、承認する手順は以下のとおりです。

1. 「**[!UICONTROL 管理者]**」領域に移動します。

   ![](assets/approve-a-custom-object-1.png)

1. 「**[!UICONTROL Marketo カスタムオブジェクト]**」をクリックします。

   ![](assets/approve-a-custom-object-2.png)

1. ドラフト状態のオブジェクトを選択します。

   ![](assets/approve-a-custom-object-3.png)

1. **[!UICONTROL カスタムオブジェクトアクション]**&#x200B;ドロップダウンをクリックし、**[!UICONTROL オブジェクトを承認]**&#x200B;を選択します。

   ![](assets/approve-a-custom-object-4.png)

1. ステートが「[!UICONTROL 承認済み]」に変わります。

   ![](assets/approve-a-custom-object-5.png)

   >[!NOTE]
   >
   >_一対多構造_&#x200B;を使用したカスタムオブジェクトは、承認される重複排除フィールド、リンクフィールド、リンクされたオブジェクト名、リンクされたフィールド名が少なくとも 1 つ必要です。
   >
   >_多対多構造_&#x200B;を使用したカスタムオブジェクトは、承認するときに、リンクフィールド、リンクされたオブジェクト名、リンクされたフィールド名は&#x200B;**必要ありません**（それらは中間オブジェクトに存在するため）。
   >
   >_中間オブジェクト_&#x200B;を使用したカスタムオブジェクトは、リンクフィールド、リンクされたオブジェクト名、リンクされたフィールド名が必要ですが、重複排除フィールドは&#x200B;**必要ありません**。
   >
   >詳しくは、[Marketo カスタムオブジェクトについて](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)を参照してください。

これで完了です。キャンペーンで使用するフィルターやトリガーの制約内でカスタムオブジェクトを選択できるようになりました。

## 編集されたカスタムオブジェクトの承認 {#approve-an-edited-custom-object}

承認済みのカスタムオブジェクトを編集した後、ドラフトを承認して、カスタムオブジェクトを承認済みのステートに戻す必要があります。

1. 既に承認済みのカスタムオブジェクトを編集すると、[!UICONTROL 承認待ち下書きあり]ステートが返されます。

   ![](assets/approve-a-custom-object-6.png)

1. ドラフトを承認する準備が整ったら、**[!UICONTROL カスタムオブジェクトアクション]**&#x200B;ドロップダウンをクリックして、**[!UICONTROL オブジェクトを承認]**&#x200B;を選択します。

   ![](assets/approve-a-custom-object-7.png)

1. プレビューには、ドラフトで変更された項目が表示されます。「**[!UICONTROL 承認]**」をクリックします。

   ![](assets/approve-a-custom-object-8.png)
