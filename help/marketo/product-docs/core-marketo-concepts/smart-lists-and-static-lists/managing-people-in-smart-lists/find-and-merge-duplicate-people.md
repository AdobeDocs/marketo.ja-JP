---
unique-page-id: 557339
description: 重複ユーザーの検索と結合 —Marketoドキュメント — 製品ドキュメント
title: 重複ユーザーの検索と結合
exl-id: a6d46096-587a-4e3a-b37a-917c0d2098b1
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---

# 重複ユーザーの検索と結合{#find-and-merge-duplicate-people}

Marketoは、新しい人がシステムに入ると自動的に重複を取り消します。 ただし、CRMが最初に重複をMarketoに送信した可能性があります。 これらを統合する方法を次に示します。

>[!NOTE]
>
>Marketoは、SalesforceまたはMicrosoft Dynamicsの同期に対する重複除外を自動的に行わないか、またはユーザーを手動で入力した場合に重複除外を行いません。

>[!PREREQUISITES]
>
>重複の検索と結合には、[組み込み/システムスマートリスト](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-built-in-system-smart-lists.md)を使用します。

## 重複の検索{#find-duplicates}

1. **Database**&#x200B;領域に移動します。

   ![](assets/db.png)

   >[!CAUTION]
   >
   >Salesforce個人アカウントを使用している場合、Marketoでのユーザーの結合は機能しない場合があります。 可能な場合は、Salesforceのレコードを結合してください。

1. **可能な重複**&#x200B;システムスマートリストを選択し、「**人**」タブをクリックします。

   ![](assets/two.png)

   >[!NOTE]
   >
   >また、[カスタムロジック](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-duplicate-people-with-custom-logic.md)を使用して重複ユーザーを検索することもできます。

## ユーザーを手動で結合{#merge-people-manually}

>[!CAUTION]
>
>人を結合する際に、敗れた人物がMarketoのカスタムオブジェクトを持っている場合、その人物は勝者に再び関連付けられません。**** 結合を実行する前に、カスタムオブジェクトの親を再度設定してください。

1. Ctrl/Commandキーを押しながらクリックし、「**人を結合**」をクリックして重複を選択します。

   ![](assets/three.png)

   >[!TIP]
   >
   >同じ人物に対して複数の重複を設定できます。すべてを一度に選択します。

1. _一致しない_&#x200B;レコード間の値が表示されます。 各フィールドに保持する値を選択します。 完了したら、「**Merge**」をクリックします。 どちらの値も必要ない場合は、**カスタム**&#x200B;をチェックし、選択した値を入力します。

   ![](assets/four.png)

   >[!NOTE]
   >
   >ユーザーを手動で結合する場合、最初に選択したユーザーが「勝者」になります。 したがって、198と199のレコードIDを結合している場合、最初に199をクリックすると、「人」タブで、結合した人のレコードIDが199になります。 これは、3つ以上のレコードが結合される場合にも当てはまります。

   >[!TIP]
   >
   >結合は、削除するよりも良いです。 すべての履歴（ページ訪問数、リンククリック数、電子メールの開封、フォームの入力など）を節約します。

## Salesforceでの効果{#effect-in-salesforce}

Salesforce統合を使用している場合、Salesforceでのリードの結合の効果についていくつかのメモがあります。

* リードのみまたは連絡先のみをマージする場合、通常のSalesforceルールごとにマージされます。
* リードとコンタクトをマージする場合、通常のSalesforceルールごとにマージする前に、すべてのリードがコンタクトに変換されます。

リードまたは連絡先を結合する際のSalesforceの動作の詳細については、以下のSalesforceドキュメントを確認してください。

* [重複リードの結合](https://help.salesforce.com/HTViewHelpDoc?id=leads_merge.htm&amp;language=en_US)
* [重複の連絡先の結合](https://help.salesforce.com/HTViewHelpDoc?id=contacts_merge.htm&amp;language=en_US)

## 一括マージ{#bulk-merging}

手動で結合する重複が多すぎる場合は、カスタマーサクセスマネージャーにお問い合わせください。

超！ CRMに接続している場合、レコードは次の規則に従ってCRMに結合されます。
