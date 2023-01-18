---
unique-page-id: 2953384
description: カスタムエンティティの同期の有効化 - Marketo ドキュメント - 製品ドキュメント
title: カスタムエンティティの同期の有効化
exl-id: 4b075bf3-f10b-4725-8c8e-a6ecee63d756
source-git-commit: 79cfb0396f690a370cdce4e4df3a23c7439c252e
workflow-type: ht
source-wordcount: '224'
ht-degree: 100%

---

# カスタムエンティティの同期の有効化 {#enable-sync-for-a-custom-entity}

Marketo で Dynamics のカスタムエンティティデータを使用できるようにする場合、その同期を有効にする方法を次に示します。

>[!NOTE]
>
>**管理者権限が必要**

>[!NOTE]
>
>* カスタムエンティティの同期を有効にすると、Marketo で初期同期が実行され、カスタムオブジェクトのすべてのデータが取り込まれます。
>* マーケティングリストとマーケティングリストのメンバーは、この時点では&#x200B;**サポート対象外**&#x200B;です。


>[!IMPORTANT]
>
>Marketo 同期ユーザは、カスタムオブジェクトをリストし、同期を実行するために、カスタムオブジェクトへの読み取りアクセス権が必要です。

1. 「**管理者**」セクションに移動します。

   ![](assets/enable-sync-for-a-custom-entity-1.png)

1. 「**Microsoft Dynamics**」を選択し、「**同期を無効にする**」をクリックします。

   ![](assets/enable-sync-for-a-custom-entity-2.png)

   >[!NOTE]
   >
   >カスタムエンティティを有効または無効にするには、グローバル同期を一時的に無効にする必要があります。

1. データベース管理にある「**Dynamics エンティティ同期**」リンクをクリックします。

   ![](assets/enable-sync-for-a-custom-entity-3.png)

1. 「**スキーマを同期**」リンクをクリックします。

   ![](assets/enable-sync-for-a-custom-entity-4.png)

1. 同期するエンティティを選択し、「**同期を有効にする**」をクリックします。

   ![](assets/enable-sync-for-a-custom-entity-5.png)

1. 同期するまたはスマートリストの[制約](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md)やトリガーとして使用するフィールドを選択します。完了したら、「**同期を有効にする**」をクリックします。

   ![](assets/enable-sync-for-a-custom-entity-6.png)

   >[!NOTE]
   >
   >同期の処理中に、「Dynamic エンティティ同期」項目がナビゲーションツリーから消える場合があります。これは期待された動作で、この項目は同期が完了した後で再び表示されます。

1. エンティティに緑のチェックマークが付きます。

   ![](assets/enable-sync-for-a-custom-entity-7.png)

1. グローバル同期を再度有効にすることを忘れないでください。

   ![](assets/enable-sync-for-a-custom-entity-8.png)
