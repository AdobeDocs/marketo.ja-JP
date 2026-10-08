---
unique-page-id: 11378713
description: カスタムオブジェクトの使用方法Marketo カスタムオブジェクトのスマートキャンペーンのスマートリストでトリガーを追加または変更する方法と、トリガーを追加して制約を設定する手順を説明します。
title: カスタムオブジェクトの変更のトリガー
exl-id: a2a3d82f-33ae-4191-b114-dbbf944a66c8
feature: Custom Objects
TQID: 'https://experienceleague.adobe.com/KjZuM-gPLIFa1umPF4pzN2OTak51i9I5TUcC7SacmZ8'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
    internal-label: Configuration
subfeature_v2:
  - id: ea4e3ff5-e7b9-4b4c-a5a0-dc27cc3f4275
    internal-label: Custom objects
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 81%
---
# カスタムオブジェクトの変更のトリガー {#trigger-off-custom-object-changes}

>[!NOTE]
>
>この機能は以下の場合にのみ使用できます。
>
>* Marketo カスタムオブジェクトでのみ使用し、ネイティブの [!DNL Salesforce] または [!DNL Microsoft Dynamics] 統合を通じて同期されたカスタムオブジェクトでは使用しません。
>
>* フィルターとしてではなくトリガーとして使用
>
>カスタムオブジェクト変更トリガーを有効にするには、[Marketo サポート ](https://nation.marketo.com/t5/Support/ct-p/Support)にお問い合わせください。

スマートキャンペーンのスマートリストでは、カスタムオブジェクトが個人または会社に追加されたときのフローアクションをトリガーできます。 また、カスタムオブジェクトの&#x200B;_変更_&#x200B;をトリガーとして使用するスマートリストを作成することもできます。 例えば、コース名が更新されたときにメールを送信する場合に使用します。

>[!NOTE]
>
>カスタムオブジェクトレコードが変更されても、アクティビティログエントリは作成されません。

1. Marketo Engage で、**[!UICONTROL マーケティングアクティビティ]**&#x200B;に移動します。

   ![](assets/trigger-off-custom-object-changes-1.png)

1. 新規にスマートキャンペーンを作成するか、既存のスマートキャンペーンを開き、「スマートリスト」を選択します。

   ![](assets/trigger-off-custom-object-changes-2.png)

1. 必要なトリガーを検索し、キャンバスにドラッグします。

   ![](assets/trigger-off-custom-object-changes-3.png)

1. [!UICONTROL トリガー属性]を選択します。

   ![](assets/trigger-off-custom-object-changes-4.png)

1. 必要に応じて、制約を設定します。

   ![](assets/trigger-off-custom-object-changes-5.png)

1. 変更は自動的に保存されます。

   ![](assets/trigger-off-custom-object-changes-6.png)

   >[!NOTE]
   >
   >* [スマートリストの作成](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
   >* [Marketo カスタムオブジェクトについて](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
