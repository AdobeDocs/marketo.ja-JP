---
unique-page-id: 11378713
description: カスタムオブジェクトの変更のトリガー- Marketo ドキュメント - 製品ドキュメント
title: カスタムオブジェクトの変更のトリガー
exl-id: a2a3d82f-33ae-4191-b114-dbbf944a66c8
source-git-commit: 99b11e17e9c2255a19c658b166e7b38c45cf1001
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 100%

---

# カスタムオブジェクトの変更のトリガー {#trigger-off-custom-object-changes}

>[!NOTE]
>
>この機能は以下の場合にのみ使用できます。
>
>* Orion インフラストラクチャのお客様向け
>* Marketo カスタムオブジェクトでのみ使用し、ネイティブの Salesforce または Microsoft Dynamics 統合を通じて同期されたカスタムオブジェクトでは使用しません。
>* フィルターとしてではなくトリガーとして使用
>
>カスタムオブジェクト変更トリガーを有効にするには、[Marketo サポート](https://nation.marketo.com/t5/Support/ct-p/Support)に連絡してください。

スマートキャンペーンのスマートリストでは、カスタムオブジェクトが個人または会社に追加されたときのフローアクションをトリガーできます。また、カスタムオブジェクトの&#x200B;*変更*&#x200B;をトリガーとして使用するスマートリストを作成することもできます。例えば、コース名が更新されたときにメールを送信する場合に使用します。

>[!NOTE]
>
>カスタムオブジェクトレコードが変更されても、アクティビティログエントリは作成されません。

1. Marketo で、「**マーケティング活動**」に移動します。

   ![](assets/trigger-off-custom-object-changes-1.png)

1. 既存のスマートキャンペーンを作成するか開いて、「スマートリスト」を選択します。

   ![](assets/trigger-off-custom-object-changes-2.png)

1. 必要なトリガーを検索し、キャンバスにドラッグします。

   ![](assets/trigger-off-custom-object-changes-3.png)

1. 「トリガー」属性を選択します。

   ![](assets/trigger-off-custom-object-changes-4.png)

1. オプションで、制約を設定します。

   ![](assets/trigger-off-custom-object-changes-5.png)

1. これで完了です。変更は自動的に保存されます。

   ![](assets/trigger-off-custom-object-changes-6.png)

   >[!NOTE]
   >
   >* [スマートリストの作成](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
   >* [Marketo カスタムオブジェクトについて](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)

