---
unique-page-id: 2360370
description: 同期前のプログラムのステータスとSalesforceキャンペーンのステータスを照合する方法 — Marketto Docs — 製品ドキュメント
title: 同期前のプログラムのステータスとSalesforceキャンペーンのステータスを照合する方法
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---


# 同期前のプログラムのステータスとSalesforceキャンペーンのステータスを照合する方法 {#how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync}

この記事では、MarketoプログラムとSalesforceキャンペーンの同期の前に、互換性のないステータスエラーを修正し、ステータスをマッピングする方法について説明します。

## エラーメッセージが表示された場合の対処方法 {#what-do-you-do-if-you-received-an-error-message}

リードを含む既存のSalesforceキャンペーンと同期しようとすると、そのキャンペーンに互換性のない1つ以上のステータスが含まれている場合は、エラーメッセージが表示されます。 ステータスが完全に一致しない場合、MarketoプログラムとSalesforceキャンペーン *は* 、同期されません。

![](assets/image2015-7-22-9-3a23-3a29.png)

このエラーメッセージから、次を選択できます。

1. 別のキャンペーンを選択して同期します。または、
1. 取り消し、ステータスエラーを修正し、エラーが修復されたら同期を試みることができます。 ステータスエラーを修正するには、次のいずれかを実行します。

   * Salesforceにログインし、互換性のないキャンペーン「メンバーのステータス」を削除または名前変更して、Marketoプログラムに関連付けられているチャネルタイプに使用される「マーケティングプログラムのステータス」に対応付けます。
   * Marketoのプログラムステータスを変更して、所定のSalesforceキャンペーンメンバーステータスに対応付けます。 これは、マーケティング担当者の機能です。 詳しくは、「プログラムチャネルの [作成](../../../../../product-docs/administration/tags/create-a-program-channel.md)」を参照してください。

