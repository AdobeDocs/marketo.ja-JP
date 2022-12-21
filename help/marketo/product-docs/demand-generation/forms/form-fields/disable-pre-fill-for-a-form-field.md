---
unique-page-id: 2359675
description: フォームフィールドの事前入力を無効にする - Marketo ドキュメント - 製品ドキュメント
title: フォームフィールドの事前入力を無効にする
exl-id: c600e0ce-1b94-4f7b-b75d-f550a2904799
source-git-commit: 35e86ac356e61e9d6b9a663e468ced1e9a947144
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 100%

---

# フォームフィールドの事前入力を無効にする {#disable-pre-fill-for-a-form-field}

Web 訪問者が既知の（cookie が有効）場合、Marketo のフォームはデフォルトで、フィールドにその情報を事前に入力します。これをオフにするには、次の方法を使用します。

>[!NOTE]
>
>**フォームの事前入力**&#x200B;はデフォルトで有効になっています。ランディングページレベルの事前入力設定と管理者レベルの事前入力設定は、フォームレベルの設定より優先されます。
>
>フォーム＞ランディングページ＞管理者

## 事前入力を無効にする方法 {#how-to-disable-pre-fill}

1. **マーケティング活動**&#x200B;に移動します。

   ![](assets/login-marketing-activities-7.png)

1. フォームを選択して、「**フォームの編集**」をクリックします。

   ![](assets/image2014-9-15-14-3a26-3a46.png)

   >[!CAUTION]
   >
   >フォームを独自のページに埋め込むと、フォームの事前入力が機能しません。これは、Marketo のランディングページでのみ機能します。

1. いずれかのフィールドを選択し、**フォームの事前入力**&#x200B;を&#x200B;**無効**&#x200B;に設定します。

   ![](assets/image2014-9-15-14-3a26-3a54.png)

   >[!TIP]
   >
   >また、ランディングページレベルまたは管理者レベルで、フォームの事前入力を無効にすることもできます。

1. 「**終了**」をクリックします。

   ![](assets/image2014-9-15-14-3a27-3a1.png)

1. 「**承認して閉じる**」をクリックします。

   ![](assets/image2014-9-15-14-3a27-3a6.png)

## 機密フィールド {#sensitive-fields}

[フィールドを機密としてマーク](/help/marketo/product-docs/administration/field-management/mark-a-field-as-sensitive.md)すると、値がフォームに事前入力されないように設定できます。これは、「事前入力」オプションに表示されます。

![](assets/disable-pre-fill.png)