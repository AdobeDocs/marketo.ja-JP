---
unique-page-id: 2359675
description: Marketoでフォームフィールドの事前入力を無効にする方法について説明します。 既知の訪問者データがフィールドに自動入力されるのを防ぎます。
title: フォームフィールドの事前入力を無効にする
exl-id: c600e0ce-1b94-4f7b-b75d-f550a2904799
feature: Forms
TQID: https://experienceleague.adobe.com/loH0b6d25kDL0dReI7lU62IFyXGr3p8tygqwTPx-OVk
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 192
ht-degree: 89%

---

# フォームフィールドの事前入力を無効にする {#disable-pre-fill-for-a-form-field}

Web 訪問者が既知の（cookie が有効）場合、Marketo のフォームはデフォルトで、フィールドにその情報を事前に入力します。 これをオフにするには、次の方法を使用します。

>[!NOTE]
>
>**フォームの事前入力**&#x200B;はデフォルトで有効になっています。 ランディングページレベルの事前入力設定と管理者レベルの事前入力設定は、フォームレベルの設定より優先されます。
>
>優先順位：管理者、ランディングページ、フォーム（左が優先）

## 事前入力を無効にする方法 {#how-to-disable-pre-fill}

1. **[!UICONTROL マーケティングアクティビティ]**&#x200B;に移動します。

   ![](assets/login-marketing-activities-7.png)

1. フォームを選択し、「**[!UICONTROL フォームの編集]**」をクリックします。

   ![](assets/image2014-9-15-14-3a26-3a46.png)

   >[!CAUTION]
   >
   >フォームを独自のページに埋め込むと、フォームの事前入力が機能しません。 これは、Marketo のランディングページでのみ機能します。

1. いずれかのフィールドを選択し、**[!UICONTROL フォームの事前入力]**&#x200B;を&#x200B;**[!UICONTROL 無効]**&#x200B;に設定します。

   ![](assets/image2014-9-15-14-3a26-3a54.png)

   >[!TIP]
   >
   >また、ランディングページレベルまたは管理者レベルで、フォームの事前入力を無効にすることもできます。

1. 「**[!UICONTROL 終了]**」をクリックします。

   ![](assets/image2014-9-15-14-3a27-3a1.png)

1. 「**[!UICONTROL 承認して閉じる]**」をクリックします。

   ![](assets/image2014-9-15-14-3a27-3a6.png)

## 機密フィールド {#sensitive-fields}

[フィールドを機密としてマーク](/help/marketo/product-docs/administration/field-management/mark-a-field-as-sensitive.md)すると、値がフォームに事前入力されないように設定できます。これは、「事前入力」オプションに表示されます。

![](assets/disable-pre-fill.png)
