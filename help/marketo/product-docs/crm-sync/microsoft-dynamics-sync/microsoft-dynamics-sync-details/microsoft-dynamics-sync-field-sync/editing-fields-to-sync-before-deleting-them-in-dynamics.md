---
description: Dynamics -Marketoドキュメント — 製品ドキュメントで削除する前に、同期するフィールドを編集する
title: Dynamicsで削除する前に、同期するフィールドを編集する
exl-id: 6fa9f6c0-c69d-478f-b333-13a5c910f577
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 0%

---

# Dynamics {#editing-fields-to-sync-before-deleting-them-in-dynamics}で削除する前に、同期するフィールドを編集する

場合によっては、Dynamicsのフィールドを削除する必要があります。 Marketoは、フィールドリストを、同期のベースとなる参照として保持します。 同期がオンの間にDynamicsでフィールドを削除すると、同期でエラーが発生する可能性があります。 フィールドを削除する前に、次の手順に従ってください。

1. Marketoで、**管理者**&#x200B;をクリックします。

   ![](assets/sync-before-deleting-them-in-dynamics-1.png)

1. [統合]で[**Microsoft Dynamics**]をクリックします。

   ![](assets/sync-before-deleting-them-in-dynamics-2.png)

1. 「**同期を無効にする**」をクリックします。

   ![](assets/sync-before-deleting-them-in-dynamics-3.png)

1. ブラウザーの新しいタブで、Dynamicsにログインし、目的のフィールドを削除します。

1. Marketoに戻る、Microsoft Dynamicsで、「手順2:「同期するフィールドを選択」****

   ![](assets/sync-before-deleting-them-in-dynamics-4.png)

1. フィールドを確認し、「**保存**」をクリックします。

   ![](assets/sync-before-deleting-them-in-dynamics-5.png)

>[!CAUTION]
>
>更新したスキーマを同期用に保存するには、変更が行われていない場合でも、[**保存**]をクリックする必要があります。

>[!NOTE]
>
>Dynamicsでフィールドを削除する前に同期が停止しない場合は、同期でエラーが発生する可能性があります。 同期が終了すると、同期は停止します。 再開する前に、Marketo管理者は、スキーマの変更を同期で受け入れるために、「同期するフィールドを選択」（上述）を確認し、「**保存**」をクリックする必要があります。

変更が保存された後は、同期を必ず有効にしてください。
