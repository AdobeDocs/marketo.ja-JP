---
unique-page-id: 1147324
description: フィールド値の消去 — マーケティング担当者向けドキュメント — 製品ドキュメント
title: フィールド値をクリア
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '121'
ht-degree: 0%

---


# フィールド値をクリア {#clear-field-values}

** [Change Data Value](../../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md)**は非常に優れていますが、値を完全に *削除するにはどうすればよいですか* 。 良い質問だ！

1. フローの手順で、クリアするフィールドを選択し、「 **新しい値**」に「**NULL **（すべて大文字）」を入力します。

   ![](assets/image2015-3-19-10-3a6-3a14.png)

1. ブーム！ 知らなかったと思う！ フロー手順が終了すると、選択したフィールドの値がクリアされます。

   ![](assets/image2015-3-19-10-3a11-3a9.png)

   >[!CAUTION]
   >
   >新しい値を空白にしたり、単にSPACEを入力したりしても、フィールドは実際には空になりません。 NULLを入力する必要があります。 また、フローステップは実行後に元に戻すことができません。

   ![（笑顔）](assets/smile.svg)

ところで、この小さなテクニックはMarketoの認定試験です。 言うな！