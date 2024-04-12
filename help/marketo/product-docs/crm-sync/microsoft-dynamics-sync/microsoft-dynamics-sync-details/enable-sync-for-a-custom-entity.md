---
unique-page-id: 2953384
description: カスタムエンティティの同期の有効化 - Marketo ドキュメント - 製品ドキュメント
title: カスタムエンティティの同期の有効化
exl-id: 4b075bf3-f10b-4725-8c8e-a6ecee63d756
feature: Microsoft Dynamics
source-git-commit: d522950af40c5e3e702a6522101ebe9550432be5
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 58%

---

# カスタムエンティティの同期の有効化 {#enable-sync-for-a-custom-entity}

Dynamics のカスタムエンティティデータをMarketo Engageで使用できるようにする必要がある場合は、次の方法で同期を有効にします。

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

1. [ データベースの管理 ] で、 **[!UICONTROL Dynamics エンティティ同期]**.

   ![](assets/enable-sync-for-a-custom-entity-3.png)

1. クリック **[!UICONTROL スキーマを同期]**.

   ![](assets/enable-sync-for-a-custom-entity-4.png)

1. 同期するエンティティを選択し、「**[!UICONTROL 同期を有効にする]**」をクリックします。

   ![](assets/enable-sync-for-a-custom-entity-5.png)

1. 同期または使用するフィールドを選択 [制約](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md) トリガー（追加されたレコードの場合） _ではない_ （更新）をスマート・リストで使用できます。 完了したら、「**[!UICONTROL 同期を有効にする]**」をクリックします。

   ![](assets/enable-sync-for-a-custom-entity-6.png)

   >[!NOTE]
   >
   >同期プロセス中に、「[!UICONTROL 動的エンティティ同期]「」項目がナビゲーションツリーから消えます。 これは期待された動作で、この項目は同期が完了した後で再び表示されます。

1. エンティティには緑色のチェックマークが付いています。

   ![](assets/enable-sync-for-a-custom-entity-7.png)

1. グローバル同期を再度有効にすることを忘れないでください。

   ![](assets/enable-sync-for-a-custom-entity-8.png)
