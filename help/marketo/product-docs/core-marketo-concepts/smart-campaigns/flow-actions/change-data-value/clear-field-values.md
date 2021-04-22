---
unique-page-id: 1147324
description: フィールド値の消去 —Marketoドキュメント — 製品ドキュメント
title: フィールド値をクリア
exl-id: cddc7697-4e8f-4a62-865c-efd451abea0c
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '102'
ht-degree: 0%

---

# フィールド値をクリア{#clear-field-values}

[データ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) 値の変更は非常に優れていますが、値を完全に __ 削除するにはどうしたらよいですか。良い質問だ！

1. フロー手順で、クリアするフィールドを選択し、**NULL**（すべて大文字）を&#x200B;**新しい値**&#x200B;として入力します。

   ![](assets/image2015-3-19-10-3a6-3a14.png)

1. ブーム！ 知らなかったと思う！ フロー手順が終了すると、選択したフィールドの値がクリアされます。

   ![](assets/image2015-3-19-10-3a11-3a9.png)

   >[!CAUTION]
   >
   >新しい値を空白にしたり、単にSPACEを入力したりしても、フィールドは実際には空になりません。 NULLを入力する必要があります。 また、フローステップは実行後に元に戻すことができません。
