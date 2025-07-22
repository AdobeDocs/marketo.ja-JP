---
unique-page-id: 2360370
description: 同期前のプログラムステータスと Salesforce キャンペーンステータスの照合方法 - Marketo ドキュメント - 製品ドキュメント
title: 同期前のプログラムステータスと Salesforce キャンペーンステータスの照合方法
exl-id: 623676ff-ce63-484f-8467-71127fa40fe0
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 66%

---

# 同期前にプログラムステータスと [!DNL Salesforce] キャンペーンステータスを照合する方法 {#how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync}

ここでは、Marketo プログラムと [!DNL Salesforce] Campaign の同期を開始する前に、互換性のないステータスエラーを修正し、ステータスをマッピングする方法について説明します。

## エラーメッセージが表示された場合の対処方法 {#what-do-you-do-if-you-received-an-error-message}

リードを含む既存の [!DNL Salesforce] Campaign に同期しようとして、そのキャンペーンに 1 つ以上の互換性のないステータスが含まれている場合は、エラーメッセージが表示されます。 ステータスが完全には一致しない場合、Marketo プログラムと [!DNL Salesforce] キャンペーンは同期されません *同期されません*。

![](assets/image2015-7-22-9-3a23-3a29.png)

このエラーメッセージから、次ができます。

1. 同期先となる別のキャンペーンをドロップダウンメニューから選択する、または、
1. キャンセルしてステータスエラーを修正し、エラーが修正された後に同期を試みる。ステータスエラーを修正するには、次のいずれかの操作をおこないます。

   * Salesforce にログインし、互換性のないキャンペーンメンバーステータスを削除または名前変更して、Marketo プログラムに関連付けられたチャネルタイプに使用される Marketo プログラムステータスにマッピングする。
   * Marketo のプログラムステータスを変更して、指定した Salesforce キャンペーンメンバーステータスにマッピングする。これは Marketo 管理機能です。詳しくは、[プログラムチャネルの作成](/help/marketo/product-docs/administration/tags/create-a-program-channel.md){target="_blank"}を参照してください。
