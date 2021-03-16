---
unique-page-id: 2360291
description: フィールドの更新のブロック — Marketto Docs — 製品ドキュメント
title: フィールドの更新をブロックする
translation-type: tm+mt
source-git-commit: 9f88e7cebc5e9d0d4491d65d332ccfdd9a31c395
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---


# フィールドの更新をブロック{#block-updates-to-a-field}

フィールドに対する更新をブロックすると、1回だけフィールドに書き込みを行い、その後、フィールドの有効期間内は元の値を保持できます。 これは、「ユーザーのソース」などのフィールドで役立ちます。

>[!NOTE]
>
>**必要な管理者権限**

1. **管理者**&#x200B;に移動し、**フィールド管理**&#x200B;をクリックします。

   ![](assets/image2014-9-24-13-3a54-3a40.png)

1. フィールドを探して選択し、「**フィールドアクション**」で「**フィールドの更新をブロック**」をクリックします。

   ![](assets/two-1.png)

   >[!NOTE]
   >
   >[プログラムメンバのカスタムフィールド](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md)に対する更新もブロックできます。

1. ブロックする&#x200B;**入力ソース**&#x200B;を選択し、**適用**&#x200B;をクリックします。

   ![](assets/image2014-9-24-13-3a55-3a16.png)

   >[!CAUTION]
   >
   >リストのインポートを実行すると、インポートプレビューでブロックされるフィールドのステータスは、_exactly_&#x200B;に一致する（またはエイリアスが確立されている）フィールドの名前に基づいて、Marketorによってフィールドが自動的に認識された場合にのみ表示されます。 「マーケティング先フィールド」ドロップダウンから手動でフィールドを選択した場合、「読み込み」プレビューにブロック状態は表示されませんが、そのフィールドに対する更新ブロックは引き続き実装されます。
