---
unique-page-id: 2953384
description: カスタムエンティティの同期の有効化 - Marketo ドキュメント - 製品ドキュメント
title: カスタムエンティティの同期の有効化
exl-id: 4b075bf3-f10b-4725-8c8e-a6ecee63d756
feature: Microsoft Dynamics
source-git-commit: d522950af40c5e3e702a6522101ebe9550432be5
workflow-type: ht
source-wordcount: '222'
ht-degree: 100%

---

# カスタムエンティティの同期の有効化 {#enable-sync-for-a-custom-entity}

Marketo Engage で Dynamics のカスタムエンティティデータを使用できるようにする必要がある場合、その同期を有効にする方法を次に示します。

>[!NOTE]
>
>**管理者権限が必要**

>[!NOTE]
>
>* カスタムエンティティの同期を有効にすると、Marketo で初期同期が実行され、カスタムオブジェクトのすべてのデータが取り込まれます。
>* マーケティングリストとマーケティングリストのメンバーは、この時点では&#x200B;_サポート対象外_&#x200B;です。

>[!IMPORTANT]
>
>Marketo 同期ユーザは、カスタムオブジェクトをリストし、同期を実行するために、カスタムオブジェクトへの読み取りアクセス権が必要です。

1. 「**[!UICONTROL 管理者]**」セクションに移動します。

   ![](assets/enable-sync-for-a-custom-entity-1.png)

1. 「**[!UICONTROL Microsoft Dynamics]**」を選択し、「**[!UICONTROL 同期を無効にする]**」をクリックします。

   ![](assets/enable-sync-for-a-custom-entity-2.png)

   >[!NOTE]
   >
   >カスタムエンティティを有効または無効にするには、グローバル同期を一時的に無効にする必要があります。

1. データベース管理で、「**[!UICONTROL Dynamics エンティティ同期]**」をクリックします。

   ![](assets/enable-sync-for-a-custom-entity-3.png)

1. 「**[!UICONTROL 同期スキーマ]**」をクリックします。

   ![](assets/enable-sync-for-a-custom-entity-4.png)

1. 同期するエンティティを選択し、「**[!UICONTROL 同期を有効にする]**」をクリックします。

   ![](assets/enable-sync-for-a-custom-entity-5.png)

1. スマートリストで同期するフィールド、または[制約](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md)やトリガー（更新では&#x200B;_なく_、追加したレコードの場合）として使用するフィールドを選択します。完了したら、「**[!UICONTROL 同期を有効にする]**」をクリックします。

   ![](assets/enable-sync-for-a-custom-entity-6.png)

   >[!NOTE]
   >
   >同期の処理中に、「[!UICONTROL Dynamic エンティティ同期]」項目がナビゲーションツリーから消える場合があります。これは期待された動作で、この項目は同期が完了した後で再び表示されます。

1. エンティティに緑のチェックマークが付きます。

   ![](assets/enable-sync-for-a-custom-entity-7.png)

1. グローバル同期を再度有効にすることを忘れないでください。

   ![](assets/enable-sync-for-a-custom-entity-8.png)
