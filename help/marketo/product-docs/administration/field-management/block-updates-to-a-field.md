---
unique-page-id: 2360291
description: フィールドの更新をブロックして、最初に書き込まれた値がレコードのライフタイム間保持されるようにします。
title: フィールドの更新のブロック
exl-id: 763097a3-cfa0-4df7-bfd1-40332b8dda1e
feature: Field Management
TQID: https://experienceleague.adobe.com/XHwNOU3s7CWDUp21LaxOTo--NA1nYZvCL7G4y5AjUFg
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 182
ht-degree: 76%

---

# フィールドの更新のブロック {#block-updates-to-a-field}

フィールドの更新をブロックすると、フィールドに1回書き込み、レコードのライフタイムに対して元の値を保持できます。 これは、「[!UICONTROL 人物ソース]」などのフィールドに役立ちます。

>[!NOTE]
>
>**管理者権限が必要**

1. 「**[!UICONTROL 管理者]**」領域に移動します。

   ![](assets/block-updates-to-a-field-1.png)

1. 「**[!UICONTROL フィールド管理]**」をクリックします。

   ![](assets/block-updates-to-a-field-2.png)

1. フィールドを探して選択し、「**[!UICONTROL フィールドアクション]**」で「**[!UICONTROL フィールドの更新をブロック]**」をクリックします。

   ![](assets/block-updates-to-a-field-3.png)

   >[!NOTE]
   >
   >[プログラムメンバーのカスタムフィールド](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md)の更新もブロックできます。

1. ブロックする&#x200B;**[!UICONTROL 入力ソース]**&#x200B;を選択し、「**[!UICONTROL 適用]**」をクリックします。

   ![](assets/block-updates-to-a-field-4.png)

   >[!CAUTION]
   >
   >リストのインポートを実行すると、インポートプレビューでブロックされるフィールドのステータスは、_exactly_ に一致するフィールドの名前に基づいて、Marketo がフィールドを自動的に認識した場合にのみ表示されます。 フィールドを Marketo フィールドドロップダウンから手動で選択した場合、読み込みプレビューにブロックステータスは表示されませんが、そのフィールドに対する更新ブロックは引き続き実装されます。
