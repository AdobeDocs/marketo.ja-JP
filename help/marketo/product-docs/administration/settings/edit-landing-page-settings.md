---
unique-page-id: 2359918
description: ランディングページ設定の編集 - Marketo ドキュメント - 製品ドキュメント
title: ランディングページ設定の編集
exl-id: 019b4651-3a66-46f9-8722-66af30194380
feature: Administration, Landing Pages
source-git-commit: 43565104a7f6512d2f99eae6bc47e1ae048b2231
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 100%

---

# ランディングページ設定の編集 {#edit-landing-page-settings}

ドメイン名とフォールバックページの編集、フォームの事前入力の有効化や無効化、ランディングページの誤用の防止などを行うことができます。手順は以下のとおりです。

>[!NOTE]
>
>**管理者権限が必要**

1. 「**[!UICONTROL 管理者]**」領域に移動します。

   ![](assets/edit-landing-page-settings-1.png)

1. 「**[!UICONTROL ランディングページ]**」をクリックします。

   ![](assets/edit-landing-page-settings-2.png)

1. **[!UICONTROL ランディングページ]**&#x200B;セクションで、「**[!UICONTROL 編集]**」ボタンをクリックします。

   ![](assets/edit-landing-page-settings-3.png)

1. ドメインとページ情報を入力します。

   ![](assets/edit-landing-page-settings-4.png)

   | 用語 | 定義 |
   |---|---|
   | [!UICONTROL ランディングページのドメイン名] | これは、あなたの CNAME です。CNAME は、ランディングページの訪問者に与える URL の最初の部分です。例えば、`https://go.yourCompany.com` の場合、「go」が CNAME です。複数を使用できますが、ほとんどのユーザーは 1 つのみを使用します。 |
   | [!UICONTROL フォールバックページ] | ランディングページが存在しないか停止している場合に表示するページです。詳しくは、[フォールバックページ](/help/marketo/product-docs/administration/settings/set-a-fallback-page.md)を参照してください。 |
   | [!UICONTROL ホームページ] | 企業サイトの URL を入力します。 |

1. 「**[!UICONTROL フォームの事前入力]**」チェックボックスをオンにすると、既知の（Cookie が保存されている）リードに関する情報をフォームに事前入力できます。ブロックする場合はオフにします。

   ![](assets/edit-landing-page-settings-5.png)

   >[!NOTE]
   >
   >`<script>` タグをコードの `<head>` タグの最後に事前入力する場合は、「**[!UICONTROL Head の最後に Script を事前挿入]**」ボックスをオンにします。最初に表示する場合は、オフのままにします。
   >
   >「**[!UICONTROL デフォルトの Favicon リンクを削除]**」をオンにして、Marketo が Favicon リンクをコードに挿入しないようにします。

1. 選択したら、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/edit-landing-page-settings-6.png)

   完成です。これで、ランディングページに適切な情報が表示され、すぐに作業を開始できます。
