---
unique-page-id: 2952636
description: カスタムロジックを使用した重複ユーザーの検索 —Marketoドキュメント — 製品ドキュメント
title: カスタムロジックを使用した重複ユーザーの検索
exl-id: e268ca34-03a3-403a-8869-4e2b60bba05c
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 6%

---

# カスタムロジックを使用した重複人物の検索{#find-duplicate-people-with-custom-logic}

Marketoには、電子メールアドレスを照合して重複の人々を見つけるシステムスマートリストがあります。 別のフィールドを使用して重複を検索する場合は、次のようにします。

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

   * メールアドレス
   * 氏名
   * 姓
   * 更新時刻

   >[!NOTE]
   >
   >「電子メールアドレス」を除くすべてのフィールドでは、大文字と小文字が区別されます。 したがって、フルネームフィールドに「john doe」を入力すると、John Doeの結果は&#x200B;__&#x200B;返されません。

   ![](assets/four-2.png)

   完了! スマートリストを実行して、前に選択したフィールドに同じ値を持つ人を検索します。
