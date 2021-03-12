---
unique-page-id: 2952636
description: カスタムロジックを使用した重複の人物の検索 — Marketto Docs — 製品ドキュメント
title: カスタムロジックを使用した重複ユーザーの検索
translation-type: tm+mt
source-git-commit: cfefff241b34571b9778cbd827f45d1b468d121e
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 0%

---


# カスタムロジックを使用した重複人物の検索{#find-duplicate-people-with-custom-logic}

Marketoには、重複の電子メールアドレスを一致させて、ユーザーを見つけるシステムスマートリストがあります。 別のフィールドを使用して重複を検索する場合は、次のようにします。

>[!PREREQUISITES]
>
>[スマートリストの作成](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)

1. **マーケティングアクティビティ**&#x200B;エリアに移動します。

![](assets/ma-2.png)

1. スマートリストを選択し、「**スマートリスト**」タブをクリックします。

   ![](assets/two-4.png)

1. **重複フィールド**&#x200B;フィルターを探してキャンバスにドラッグします。

   ![](assets/three-4.png)

1. 次の4つのオプションから1つ選択します。

   * 電子メールアドレス
   * フルネーム
   * 姓
   * 更新日時

   >[!NOTE]
   >
   >「電子メールアドレス」を除くすべてのフィールドでは、大文字と小文字が区別されます。 したがって、フルネームフィールドに「john doe」を入力すると、John Doeの結果は&#x200B;__&#x200B;返されません。

   ![](assets/four-2.png)

   完了！ スマートリストを実行して、前に選択したフィールドに同じ値を持つ人を検索します。
