---
unique-page-id: 2360370
description: 同期前のプログラムのステータスとSalesforceキャンペーンのステータスを照合する方法 —Marketoドキュメント — 製品ドキュメント
title: 同期前のプログラムのステータスとSalesforceキャンペーンのステータスを照合する方法
exl-id: 623676ff-ce63-484f-8467-71127fa40fe0
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---

# 同期の前にプログラムのステータスとSalesforceキャンペーンのステータスを一致させる方法{#how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync}

この記事では、MarketoプログラムとSalesforceキャンペーンの同期の前に、互換性のないステータスエラーを修正し、ステータスをマッピングする方法について説明します。

## エラーメッセージ{#what-do-you-do-if-you-received-an-error-message}を受け取った場合はどうしますか？

リードを含む既存のSalesforceキャンペーンと同期しようとすると、そのキャンペーンに互換性のない1つ以上のステータスが含まれている場合は、エラーメッセージが表示されます。 ステータスが完全一致でない場合、MarketoプログラムとSalesforceキャンペーン&#x200B;*は*&#x200B;同期しません。

![](assets/image2015-7-22-9-3a23-3a29.png)

このエラーメッセージから、次を選択できます。

1. 別のキャンペーンを選択して同期します。または、
1. 取り消し、ステータスエラーを修正し、エラーが修復されたら同期を試みることができます。 ステータスエラーを修正するには、次のいずれかを実行します。

   * Salesforceにログインし、互換性のない「キャンペーンのステータス」を削除または名前変更して、Marketoプログラムに関連付けられたチャネルタイプに使用される「Marketoプログラムのステータス」に対応付けます。
   * Marketoのプログラムステータスを変更して、所定のSalesforceキャンペーンメンバーステータスに対応付けます。 これは、Marketo管理機能です。 詳しくは、[プログラムチャネルの作成](/help/marketo/product-docs/administration/tags/create-a-program-channel.md)を参照してください。
