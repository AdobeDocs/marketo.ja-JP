---
unique-page-id: 2360370
description: 同期前のプログラムステータスとSalesforceキャンペーンステータスの照合方法 — Marketoドキュメント — 製品ドキュメント
title: 同期前のプログラムステータスとSalesforceキャンペーンステータスの照合方法
exl-id: 623676ff-ce63-484f-8467-71127fa40fe0
source-git-commit: 7376804bda915d7ff25cdc50cb78a6686bd36882
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---

# 同期前のプログラムステータスとSalesforceキャンペーンステータスの照合方法 {#how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync}

この記事では、MarketoプログラムとSalesforce Campaignの同期の前に、互換性のないステータスエラーを修正し、ステータスをマッピングする方法について説明します。

## エラーメッセージが表示された場合の対処方法 {#what-do-you-do-if-you-received-an-error-message}

リードを含む既存のSalesforceキャンペーンと同期しようとし、キャンペーンに互換性のない1つ以上のステータスが含まれている場合は、エラーメッセージが表示されます。 ステータスが完全に一致しない場合、MarketoプログラムとSalesforceキャンペーン&#x200B;*は同期*&#x200B;されません。

![](assets/image2015-7-22-9-3a23-3a29.png)

このエラーメッセージから、次の項目を選択できます。

1. 同期先となる別のキャンペーンをドロップダウンメニューから選択します。または、
1. エラーを取り消し、ステータスエラーを修正し、エラーが修復された後に同期を試みることができます。 ステータスエラーを修正するには、次のいずれかの操作を行います。

   * Salesforceにログインし、互換性のないキャンペーンメンバーステータスを削除または名前変更して、Marketoプログラムに関連付けられたチャネルタイプに使用されるMarketoプログラムステータスにマッピングします。
   * Marketoの「プログラムステータス」を変更して、配置されているSalesforceキャンペーンメンバーステータスにマッピングします。 これは、Marketo Admin関数です。 詳しくは、[プログラムチャネルの作成](/help/marketo/product-docs/administration/tags/create-a-program-channel.md)を参照してください。
