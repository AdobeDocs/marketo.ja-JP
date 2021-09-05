---
unique-page-id: 2953384
description: カスタムエンティティの同期の有効化 - Marketo ドキュメント - 製品ドキュメント
title: カスタムエンティティの同期の有効化
exl-id: 4b075bf3-f10b-4725-8c8e-a6ecee63d756
source-git-commit: d81a4a3caa12c5ec642afadf9328b3825bde6fed
workflow-type: ht
source-wordcount: '196'
ht-degree: 100%

---

# カスタムエンティティの同期の有効化 {#enable-sync-for-a-custom-entity}

Marketo で Dynamics のカスタムエンティティデータを使用できるようにするのに、その同期を有効にする方法を次に示します。

>[!NOTE]
>
>**管理者権限が必要**

>[!NOTE]
>
>カスタムエンティティの同期を有効にすると、Marketo で初期同期が実行され、カスタムオブジェクトのすべてのデータが取り込まれます。

1. **管理**&#x200B;セクションに移動します。

   ![](assets/image2014-10-20-14-3a32-3a16.png)

1. 「**Microsoft Dynamics**」を選択し、「**同期を無効にする**」をクリックします。

   カスタムエンティティを有効または無効にするには、グローバル同期を一時的に無効にする必要があります。

   ![](assets/image2015-11-10-9-3a0-3a6.png)

1. データベース管理にある「**Dynamics エンティティ同期**」リンクをクリックします。

   ![](assets/image2015-11-10-9-3a6-3a55.png)

1. 「**スキーマを同期**」リンクをクリックします。

   ![](assets/image2015-11-10-9-3a41-3a37.png)

1. 同期するエンティティを選択し、「**同期を有効にする**」をクリックします。

   ![](assets/image2015-11-10-9-3a44-3a35.png)

1. 同期するまたはスマートリストの[制約](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md)やトリガーとして使用するフィールドを選択します。完了したら、「**同期を有効にする**」をクリックします。

   ![](assets/image2014-10-20-14-3a32-3a55.png)

   >[!NOTE]
   >
   >同期の処理中に、「Dynamic エンティティ同期」項目がナビゲーションツリーから消える場合があります。これは期待された動作で、この項目は同期が完了した後で再び表示されます。

1. エンティティに緑のチェックマークが付きます。

   ![](assets/image2014-10-20-14-3a33-3a4.png)

1. グローバル同期を再度有効にすることを忘れないでください。

   ![](assets/image2015-11-10-9-3a48-3a35.png)

これは、本当に強力です。
