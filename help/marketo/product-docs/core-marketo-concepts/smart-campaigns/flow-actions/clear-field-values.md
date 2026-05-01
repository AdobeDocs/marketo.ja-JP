---
unique-page-id: 1147324
description: スマートキャンペーンのフローステップでフィールド値をクリアする方法を説明します。 個人または会社のフィールドから値を削除します。
title: フィールド値のクリア
exl-id: cddc7697-4e8f-4a62-865c-efd451abea0c
feature: Smart Campaigns
source-git-commit: 60c5603fa29bb1039b9d477633beb2c6f5c63486
workflow-type: tm+mt
source-wordcount: '106'
ht-degree: 59%

---

# フィールド値のクリア {#clear-field-values}

[データ値の変更](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md)は便利ですが、値を完全に&#x200B;_削除_&#x200B;するには、どうすればいいでしょう？ 良い質問です。

1. フローステップで、クリアするフィールドを選択し、**[!UICONTROL 新しい値]**&#x200B;として **[!UICONTROL NULL]**（すべて大文字）と入力します。

   ![](assets/clear-field-values-1.png)

1. フローステップが終了すると、選択したフィールドの値がクリアされます。

   ![](assets/clear-field-values-2.png)

   >[!CAUTION]
   >
   >新しい値を空白のままにしたり、スペースを入力したりしても、フィールドが完全に空になるわけではありません。 NULL を入力する必要があります。 また、実行後にフローステップを元に戻すことはできません。
