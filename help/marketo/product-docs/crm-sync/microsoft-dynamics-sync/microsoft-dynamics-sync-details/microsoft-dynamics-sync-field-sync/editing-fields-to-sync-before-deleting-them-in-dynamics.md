---
description: Dynamics で削除する前に同期するフィールドを編集 - Marketo ドキュメント - 製品ドキュメント
title: Dynamics で削除する前に同期するフィールドを編集
exl-id: 6fa9f6c0-c69d-478f-b333-13a5c910f577
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 79%

---

# Dynamics で削除する前に同期するフィールドを編集 {#editing-fields-to-sync-before-deleting-them-in-dynamics}

Dynamics のフィールドを削除する場合があります。Marketo Engageでは、同期のベースとなる参照としてフィールドリストを保持します。 同期の実行中に Dynamics でフィールドを削除すると、同期でエラーが発生する場合があります。フィールドを削除する前に、次の手順に従います。

1. Marketo で、「**[!UICONTROL 管理者]**」をクリックします。

   ![](assets/sync-before-deleting-them-in-dynamics-1.png)

1. 「統合」で、「**[!UICONTROL Microsoft Dynamics]**」をクリックします。

   ![](assets/sync-before-deleting-them-in-dynamics-2.png)

1. 「**[!UICONTROL 同期の無効化]**」をクリックします。

   ![](assets/sync-before-deleting-them-in-dynamics-3.png)

1. ブラウザーの新しいタブで、Dynamics にログインし、目的のフィールドを削除します。

1. Marketo に戻り、Microsoft Dynamics で、手順 2：同期するフィールドを選択の横の「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/sync-before-deleting-them-in-dynamics-4.png)

1. フィールドを再確認し、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/sync-before-deleting-them-in-dynamics-5.png)

>[!CAUTION]
>
>「**[!UICONTROL 保存]**」をクリックすると、変更が加えられなかった場合でも、同期用に更新されたスキーマを保存する必要があります。

>[!NOTE]
>
>Dynamics でフィールドを削除する前に同期が停止していない場合は、同期でエラーが発生する場合があります。エラーが発生した場合、同期は停止します。再開する前に、同期でスキーマの変更を受け入れるために、Marketo管理者は「Select Fields to Sync」（上記）を確認し、**[!UICONTROL 保存]** をクリックする必要があります。

変更が保存された後、忘れずに同期を有効にしてください。
