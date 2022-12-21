---
unique-page-id: 557339
description: 重複した人物の検索と結合 - Marketo ドキュメント - 製品ドキュメント
title: 重複した人物の検索と結合
exl-id: a6d46096-587a-4e3a-b37a-917c0d2098b1
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 100%

---

# 重複した人物の検索と結合 {#find-and-merge-duplicate-people}

Marketo は、新しい人物がシステムに入ると、自動的に重複排除します。ただし、CRM が最初に重複を Marketo に送信している可能性があります。結合する方法は以下のとおりです。

>[!NOTE]
>
>Marketo は、Salesforce や Microsoft Dynamics の同期や、人物を手動で入力した場合には、自動的に重複排除を行いません。

>[!PREREQUISITES]
>
>重複の検索とマージには、[組み込み／システムスマートリスト](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-built-in-system-smart-lists.md)を使用することになります。

## 重複を検索する {#find-duplicates}

1. 「**データベース**」領域に移動します。

   ![](assets/db.png)

   >[!CAUTION]
   >
   >Salesforce の人物アカウントを使用している場合は、Marketo の人物の結合が機能しない場合があります。可能な場合は、Salesforce でレコードを結合してください。

1. 「**重複の可能性**」システムスマートリストを選択し、「**人物**」タブをクリックします。

   ![](assets/two.png)

   >[!NOTE]
   >
   >また、[カスタムロジックで重複する人物を検索](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-duplicate-people-with-custom-logic.md)することもできます。

## 人物を手動で結合する {#merge-people-manually}

>[!CAUTION]
>
>人物を結合する際に、敗者に Marketo のカスタムオブジェクトがあっても、勝者への再関連付けは&#x200B;**行われません**。結合を実行する前に、カスタムオブジェクトの親の関連付けを再度行ってください。

1. Ctrl／Cmd キーを押しながら重複を選択し、「**人物を結合**」をクリックします。

   ![](assets/three.png)

   >[!TIP]
   >
   >同じ人物に対して 2 つ以上の重複が存在する場合があります。それらすべてを一度に選択します。

1. レコード間で&#x200B;_一致しない_&#x200B;値が表示されます。各フィールドに保持する値を選択します。終了したら「**結合**」をクリックします。どちらの値も不要な場合は、「**カスタム**」にチェックを入れて任意の値を入力します。

   ![](assets/four.png)

   >[!NOTE]
   >
   >人物を手動で結合する場合、最初に選択した人物が「勝者」になります。つまり、「人物」タブでレコード ID 198 と 199 を結合するときに、最初に 199 をクリックした場合、199 が結合された人のレコード ID になります。これは、2 つ以上のレコードが結合される場合にも当てはまります。

   >[!TIP]
   >
   >結合は削除よりも適しています。すべての履歴（ページ訪問数、リンククリック数、メール開封数、フォームの入力数など）は維持されます。

## Salesforce での効果 {#effect-in-salesforce}

Salesforce と統合している場合、Salesforce のリードの結合の効果に関していくつかの注意事項があります。

* リードのみまたは連絡先のみを結合する場合、通常の Salesforce ルールに従って結合されます。
* リードと連絡先を結合する場合、通常の Salesforce ルールに従って結合する前に、すべてのリードが連絡先にコンバージョンされます。

リードまたは連絡先を結合する際の Salesforce の動作の詳細は、次の Salesforce ドキュメントを確認してください。

* [重複したリードの結合](https://help.salesforce.com/HTViewHelpDoc?id=leads_merge.htm&amp;language=en_US)
* [重複した連絡先の結合](https://help.salesforce.com/HTViewHelpDoc?id=contacts_merge.htm&amp;language=en_US)

## 一括結合 {#bulk-merging}

重複が多すぎて手動で結合できない場合は、カスタマーサクセスマネージャーに問い合わせて、方法についてご相談ください。

完了です。CRM に接続している場合、以下のルールに従ってレコードが CRM に結合されます。
