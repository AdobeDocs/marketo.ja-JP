---
description: グローバルフォーム検証ルール — Marketoドキュメント — 製品ドキュメント
title: グローバルフォーム検証ルール
hide: true
hidefromtoc: true
exl-id: a44db893-00b5-40d2-8be3-41d52b2fd7b5
source-git-commit: 0354267afa8e11dbe7ac3b56bc8a4c2886c84676
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# グローバルフォーム検証ルール {#global-form-validation-rules}

この機能を使用すると、特定のドメインがドメインフォームに送信されるのをMarketo Engageでブロックできます。

## アクセスを有効にする方法 {#how-to-enable-access}

この機能を利用する前に、目的の役割に応じて権限を有効にする必要があります。

1. Marketo で、「**管理者**」をクリックします。

   ![](assets/global-form-validation-rules-1.png)

1. 「**ユーザーと役割**」をクリックします。

   ![](assets/global-form-validation-rules-2.png)

1. 次をクリック： **役割** タブをクリックします。

   ![](assets/global-form-validation-rules-3.png)

1. 権限を付与する役割をダブルクリックします。

   ![](assets/global-form-validation-rules-4.png)

1. 次をクリック： **+** 「管理者にアクセス」の横に「 」を入力します。

   ![](assets/global-form-validation-rules-5.png)

1. 下にスクロールして、「 」を選択します。 **フォーム検証ルールにアクセス** をクリックし、 **保存**.

   ![](assets/global-form-validation-rules-6.png)

## 新規フォーム検証ルールの作成 {#create-new-form-validation-rule}

>[!IMPORTANT]
>
>これらのルールは、Marketo Engage購読内のすべてのフォームに適用されます。

1. Marketo で、「**管理者**」をクリックします。

   ![](assets/global-form-validation-rules-7.png)

1. クリック **グローバルフォーム検証ルール**.

   ![](assets/global-form-validation-rules-8.png)

1. クリック **新規フォームの検証ルール**.

   ![](assets/global-form-validation-rules-9.png)

   >[!NOTE]
   >
   >フォーム検証ルールのアクションドロップダウンを使用して、既存のルールを削除または編集できます。

1. ルールに名前を付け、オプションの説明を入力し、フォーム訪問者に表示するエラーメッセージを入力します。 ブロックするドメインを [ ルール ] ボックスに入力し、[ **ルールをアクティブ化**&#x200B;をクリックし、 **作成**.

   ![](assets/global-form-validation-rules-10.png)

>[!NOTE]
>
>Marketo Engageは、事前に読み込まれた「消費者の E メールドメインブロックリスト」ルールの使用時にブロックされる、無料の消費者の E メールドメインの定義されたブロックリストを提供します。 [ここにリストを表示](/help/marketo/product-docs/administration/settings/assets/freemaildomains.csv).
