---
description: グローバルフォーム検証ルール - Marketo ドキュメント - 製品ドキュメント
title: グローバルフォーム検証ルール
exl-id: a44db893-00b5-40d2-8be3-41d52b2fd7b5
source-git-commit: b71729a678ff4a676bb60803d845d0a44118f7e5
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 81%

---

# グローバルフォーム検証ルール {#global-form-validation-rules}

この機能を使用すると、特定のドメインがドメインフォームに送信されるのを Marketo Engage でブロックできます。

## アクセスを有効にする方法 {#how-to-enable-access}

この機能を利用する前に、目的のロールに応じて権限を有効にする必要があります。

1. Marketo で、「**[!UICONTROL 管理者]**」をクリックします。

   ![](assets/global-form-validation-rules-1.png)

1. 「**[!UICONTROL ユーザ＆ロール]**」をクリックします。

   ![](assets/global-form-validation-rules-2.png)

1. 「**[!UICONTROL ロール]**」タブをクリックします。

   ![](assets/global-form-validation-rules-3.png)

1. 権限を付与するロールをダブルクリックします。

   ![](assets/global-form-validation-rules-4.png)

1. 「管理者にアクセス」の横の「**+**」記号をクリックします。

   ![](assets/global-form-validation-rules-5.png)

1. 下にスクロールして、「**[!UICONTROL フォーム検証ルールにアクセス]**」を選択し、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/global-form-validation-rules-6.png)

## 新規フォーム検証ルールの作成 {#create-new-form-validation-rule}

>[!IMPORTANT]
>
>これらのルールは、Marketo Engage サブスクリプション内のすべてのフォームに適用されます。

1. Marketo で、「**[!UICONTROL 管理者]**」をクリックします。

   ![](assets/global-form-validation-rules-7.png)

1. 「**[!UICONTROL グローバルフォーム検証ルール]**」をクリックします。

   ![](assets/global-form-validation-rules-8.png)

1. 「**[!UICONTROL 新規フォームの検証ルール]**」をクリックします。

   ![](assets/global-form-validation-rules-9.png)

   >[!NOTE]
   >
   >「フォーム検証ルールのアクション」ドロップダウンを使用して、既存のルールを削除または編集できます。

1. ルールに名前を付け、オプションの説明を入力し、フォーム訪問者に表示するエラーメッセージを入力します。ブロックするドメインを「ルール」ボックスに入力し、「**[!UICONTROL ルールをアクティブ化]**」を選択し、「**[!UICONTROL 作成]**」をクリックします。

   ![](assets/global-form-validation-rules-10.png)

>[!NOTE]
>
>Marketo Engage には、あらかじめ用意された「消費者向けメールドメインブロックリスト」ルールを使用する際にブロックされる、無料の消費者向けメールドメインのブロックリストが定義されています。[リスト表示はこちら](/help/marketo/product-docs/administration/settings/assets/freemaildomains.csv)。

## フォームごとのアクセスを無効にする方法{#how-to-disable-access-per-form}

有効にすると、ルールはすべてのフォームに適用されます。ただし、特定の要件を持つフォームがあり、何も拒否したくない場合は、無効にできます [!UICONTROL グローバルフォーム検証ルール] 」と入力します。

1. 目的のフォームで、「**[!UICONTROL フォーム設定]**」をクリックし、「**[!UICONTROL 設定]**」をクリックします。

   ![](assets/global-form-validation-rules-11.png)

1. 次をクリック： **[!UICONTROL グローバルフォーム検証ルール]** ドロップダウンで「 」を選択します。 **[!UICONTROL 無効]**.

   ![](assets/global-form-validation-rules-12.png)

フォームを承認して投稿すると、フォームは無視されます [!UICONTROL グローバルフォーム検証ルール].
