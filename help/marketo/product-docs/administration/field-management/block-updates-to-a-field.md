---
unique-page-id: 2360291
description: フィールドの更新のブロック - Marketo ドキュメント - 製品ドキュメント
title: フィールドの更新のブロック
exl-id: 763097a3-cfa0-4df7-bfd1-40332b8dda1e
source-git-commit: 2776969be44ba1a3d795e99986d10cf0470fb9e9
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 100%

---

# フィールドの更新のブロック {#block-updates-to-a-field}

フィールドの更新をブロックすると、1 回フィールドに書き込み、フィールドの有効期間内に元の値を保持できます。これは、「ユーザーのソース」などのフィールドに役立ちます。

>[!NOTE]
>
>**管理者権限が必要**

1. 「**管理者**」領域に移動します。

   ![](assets/block-updates-to-a-field-1.png)

1. 「**フィールド管理**」をクリックします。

   ![](assets/block-updates-to-a-field-2.png)

1. フィールドを探して選択し、「**フィールドアクション**」で「**フィールドの更新をブロック**」をクリックします。

   ![](assets/block-updates-to-a-field-3.png)

   >[!NOTE]
   >
   >[プログラムメンバーのカスタムフィールド](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md)の更新もブロックできます。

1. ブロックする&#x200B;**入力ソース**&#x200B;を選択し、「**適用**」をクリックします。

   ![](assets/block-updates-to-a-field-4.png)

   >[!CAUTION]
   >
   >リストのインポートを実行すると、インポートプレビューでブロックされるフィールドのステータスは、_exactly_ に一致するフィールドの名前に基づいて、Marketo がフィールドを自動的に認識した場合にのみ表示されます。フィールドを Marketo フィールドドロップダウンから手動で選択した場合、読み込みプレビューにブロックステータスは表示されませんが、そのフィールドに対する更新ブロックは引き続き実装されます。
