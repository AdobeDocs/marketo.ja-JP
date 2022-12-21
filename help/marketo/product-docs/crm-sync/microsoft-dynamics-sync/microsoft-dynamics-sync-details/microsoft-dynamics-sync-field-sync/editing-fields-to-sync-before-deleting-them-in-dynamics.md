---
description: Dynamics で削除する前に同期するフィールドを編集 - Marketo ドキュメント - 製品ドキュメント
title: Dynamics で削除する前に同期するフィールドを編集
exl-id: 6fa9f6c0-c69d-478f-b333-13a5c910f577
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 100%

---

# Dynamics で削除する前に同期するフィールドを編集 {#editing-fields-to-sync-before-deleting-them-in-dynamics}

Dynamics のフィールドを削除する場合があります。Marketo は、同期の基になるフィールドリストを参照として保持します。同期の実行中に Dynamics でフィールドを削除すると、同期でエラーが発生する場合があります。フィールドを削除する前に、次の手順に従います。

1. Marketo で、「**管理者**」をクリックします。

   ![](assets/sync-before-deleting-them-in-dynamics-1.png)

1. 「統合」で、「**Microsoft Dynamics**」をクリックします。

   ![](assets/sync-before-deleting-them-in-dynamics-2.png)

1. 「**同期の無効化**」をクリックします。

   ![](assets/sync-before-deleting-them-in-dynamics-3.png)

1. ブラウザーの新しいタブで、Dynamics にログインし、目的のフィールドを削除します。

1. Marketo に戻り、Microsoft Dynamics で、手順 2：同期するフィールドを選択の横の「**編集**」をクリックします。

   ![](assets/sync-before-deleting-them-in-dynamics-4.png)

1. フィールドを再確認し、「**保存**」をクリックします。

   ![](assets/sync-before-deleting-them-in-dynamics-5.png)

>[!CAUTION]
>
>「**保存**」をクリックすると、変更が加えられなかった場合でも、同期用に更新されたスキーマを保存する必要があります。

>[!NOTE]
>
>Dynamics でフィールドを削除する前に同期が停止していない場合は、同期でエラーが発生する場合があります。エラーが発生した場合、同期は停止します。再開する前に、Marketo 管理者は「同期するフィールドを選択」（上述の説明）を確認し、「**保存**」をクリックして、同期でスキーマの変更を受け入れる必要があります。

変更が保存された後、忘れずに同期を有効にしてください。
