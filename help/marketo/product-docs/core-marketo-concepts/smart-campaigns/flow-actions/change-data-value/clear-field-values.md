---
unique-page-id: 1147324
description: フィールド値のクリア - Marketo ドキュメント - 製品ドキュメント
title: フィールド値のクリア
exl-id: cddc7697-4e8f-4a62-865c-efd451abea0c
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '102'
ht-degree: 100%

---

# フィールド値のクリア {#clear-field-values}

[データ値の変更](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md)は便利ですが、値を完全に&#x200B;_削除_&#x200B;するには、どうすればいいでしょう？良い質問です。

1. フローステップで、クリアするフィールドを選択し、**新しい値**&#x200B;として **NULL**（すべて大文字）と入力します。

   ![](assets/image2015-3-19-10-3a6-3a14.png)

1. いかがですか？知らなかったですよね。フローステップが終了すると、選択したフィールドの値がクリアされます。

   ![](assets/image2015-3-19-10-3a11-3a9.png)

   >[!CAUTION]
   >
   >新しい値を空白のままにしたり、単にスペースを入力したりしても、フィールドは空にはなりません。NULL を入力する必要があります。また、実行後にフローステップを元に戻すことはできません。
