---
unique-page-id: 11378713
description: カスタムオブジェクトの変更のトリガー- Marketo ドキュメント - 製品ドキュメント
title: カスタムオブジェクトの変更のトリガー
exl-id: a2a3d82f-33ae-4191-b114-dbbf944a66c8
feature: Custom Objects
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 83%

---

# カスタムオブジェクトの変更のトリガー {#trigger-off-custom-object-changes}

>[!NOTE]
>
>この機能は以下の場合にのみ使用できます。
>
>* の [!DNL Orion] インフラ
>* Marketoカスタムオブジェクトでのみ使用し、ネイティブから同期されたカスタムオブジェクトでは使用しません [!DNL Salesforce] または [!DNL Microsoft Dynamics] 統合
>* フィルターとしてではなくトリガーとして使用
>
>カスタムオブジェクト変更トリガーを有効にするには、[Marketo サポート](https://nation.marketo.com/t5/Support/ct-p/Support)に連絡してください。

スマートキャンペーンのスマートリストでは、カスタムオブジェクトが個人または会社に追加されたときのフローアクションをトリガーできます。また、カスタムオブジェクトの&#x200B;*変更*&#x200B;をトリガーとして使用するスマートリストを作成することもできます。例えば、コース名が更新されたときにメールを送信する場合に使用します。

>[!NOTE]
>
>カスタムオブジェクトレコードが変更されても、アクティビティログエントリは作成されません。

1. Marketo Engageで、に移動します。 **[!UICONTROL マーケティング活動]**.

   ![](assets/trigger-off-custom-object-changes-1.png)

1. 既存のスマートキャンペーンを作成するか開いて、「スマートリスト」を選択します。

   ![](assets/trigger-off-custom-object-changes-2.png)

1. 必要なトリガーを検索し、キャンバスにドラッグします。

   ![](assets/trigger-off-custom-object-changes-3.png)

1. を選択します。 [!UICONTROL トリガー属性].

   ![](assets/trigger-off-custom-object-changes-4.png)

1. オプションで、制約を設定します。

   ![](assets/trigger-off-custom-object-changes-5.png)

1. これで完了です。変更は自動的に保存されます。

   ![](assets/trigger-off-custom-object-changes-6.png)

   >[!NOTE]
   >
   >* [スマートリストの作成](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
   >* [Marketo カスタムオブジェクトについて](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
