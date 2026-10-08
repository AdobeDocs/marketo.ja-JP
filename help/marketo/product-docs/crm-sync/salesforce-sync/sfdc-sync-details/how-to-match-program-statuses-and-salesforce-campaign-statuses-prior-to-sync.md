---
unique-page-id: 2360370
description: 同期前にMarketo プログラムのステータスをSalesforce campaign メンバーのステータスと一致させる方法を説明します。 エラーを修正し、ステータスをマッピングして、プログラムをキャンペーンに同期できます。
title: 同期前のプログラムステータスと Salesforce キャンペーンステータスの照合方法
exl-id: 623676ff-ce63-484f-8467-71127fa40fe0
feature: Salesforce Integration
TQID: 'https://experienceleague.adobe.com/54XVLabyXlccM45i9yxPRoMqyrCtoDsATu1o1bEy-50'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
subfeature_v2:
  - id: edcca97f-2314-445f-9a79-3ac30a2a9c27
    internal-label: Salesforce integration
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 89%
---
# 同期前のプログラムステータスと [!DNL Salesforce] キャンペーンステータスの照合方法 {#how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync}

この記事では、Marketo プログラムと [!DNL Salesforce] キャンペーンを同期する前に、互換性のないステータスエラーを修正し、ステータスをマッピングする方法について説明します。

## エラーメッセージが表示された場合の対処方法 {#what-do-you-do-if-you-received-an-error-message}

リードを含む既存の [!DNL Salesforce] キャンペーンの同期を試みた際にキャンペーンに 1 つ以上の互換性のないステータスが含まれていると、エラーメッセージが表示されます。 ステータスが完全に一致しない場合、Marketo プログラムと [!DNL Salesforce] キャンペーンは同期&#x200B;*されません*。

![](assets/image2015-7-22-9-3a23-3a29.png)

このエラーメッセージから、次ができます。

1. 同期先となる別のキャンペーンをドロップダウンメニューから選択する、または
1. キャンセルしてステータスエラーを修正し、エラーが修正された後に同期を試みる。 ステータスエラーを修正するには、次のいずれかの操作を行います。

   * Salesforce にログインし、互換性のないキャンペーンメンバーステータスを削除または名前変更して、Marketo プログラムに関連付けられたチャネルタイプに使用される Marketo プログラムステータスにマッピングする。
   * Marketo のプログラムステータスを変更して、Salesforce キャンペーンメンバーステータスにマッピングする。 これは Marketo 管理機能です。 詳しくは、[プログラムチャネルの作成](/help/marketo/product-docs/administration/tags/create-a-program-channel.md){target="_blank"}を参照してください。
