---
unique-page-id: 10094188
description: 1対多、多対多、中間オブジェクトの要件を含め、管理者で新しいカスタムオブジェクトまたは編集されたカスタムオブジェクトを承認する方法。
title: カスタムオブジェクトの承認
exl-id: 8bae94df-91fe-4722-8c75-c26df882c65d
feature: Custom Objects
source-git-commit: 40d7e8a0723946970c49a6dfc4f0de4c71b0df65
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 47%

---

# カスタムオブジェクトの承認 {#approve-a-custom-object}

カスタムオブジェクトを使用するには、その前にカスタムオブジェクトを承認する必要があります。 プロセスは、新しいカスタムオブジェクトと編集したカスタムオブジェクトで若干異なります。

## 新規カスタムオブジェクトの承認 {#approve-a-new-custom-object}

新しいカスタムオブジェクトが作成されました。 承認するには、次の手順に従います。

1. 「**[!UICONTROL 管理者]**」領域に移動します。

   ![](assets/approve-a-custom-object-1.png)

1. 「**[!UICONTROL Marketo カスタムオブジェクト]**」をクリックします。

   ![](assets/approve-a-custom-object-2.png)

1. ドラフト状態にあるオブジェクトを選択します。

   ![](assets/approve-a-custom-object-3.png)

1. **[!UICONTROL カスタムオブジェクトアクション]**&#x200B;ドロップダウンをクリックし、**[!UICONTROL オブジェクトを承認]**&#x200B;を選択します。

   ![](assets/approve-a-custom-object-4.png)

1. ステートが「[!UICONTROL 承認済み]」に変わります。

   ![](assets/approve-a-custom-object-5.png)

   >[!NOTE]
   >
   >_一対多構造_&#x200B;を使用したカスタムオブジェクトは、承認される重複排除フィールド、リンクフィールド、リンクされたオブジェクト名、リンクされたフィールド名が少なくとも 1 つ必要です。
   >
   >_多対多の構造_ **で使用されるカスタムオブジェクトは、承認時にリンクフィールド、リンクされたオブジェクト名、またはリンクされたフィールド名を必要としません（これらは中間オブジェクトに存在するため）。**
   >
   >_中間オブジェクト_&#x200B;として使用されるカスタムオブジェクトには、リンクフィールド、リンクされたオブジェクト名、リンクされたフィールド名が必要ですが、**には重複排除フィールドは必要ありません。**
   >
   >詳しくは、[Marketo カスタムオブジェクトについて](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)を参照してください。

これで、フィルターやトリガーの制約でカスタムオブジェクトを選択して、キャンペーンで使用できるようになります。

## 編集されたカスタムオブジェクトの承認 {#approve-an-edited-custom-object}

承認済みのカスタムオブジェクトを編集した後、ドラフトを承認して、カスタムオブジェクトを承認済みのステートに戻す必要があります。

1. 既に承認済みのカスタムオブジェクトを編集すると、[!UICONTROL 承認待ち下書きあり]ステートが返されます。

   ![](assets/approve-a-custom-object-6.png)

1. ドラフトを承認する準備ができたら、「**[!UICONTROL カスタムオブジェクトアクション]**」ドロップダウンをクリックし、「**[!UICONTROL オブジェクトを承認]**」を選択します。

   ![](assets/approve-a-custom-object-7.png)

1. プレビューには、ドラフトで変更された項目が表示されます。 「**[!UICONTROL 承認]**」をクリックします。

   ![](assets/approve-a-custom-object-8.png)
