---
unique-page-id: 10094576
description: 永続的な登録解除 - Marketo ドキュメント - 製品ドキュメント
title: 永続的な登録解除
exl-id: e03a5a01-7395-45b3-8351-7931ec413236
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '319'
ht-degree: 100%

---

# 永続的な登録解除 {#durable-unsubscribe}

登録解除が「永続的」になるように、機能が強化されました。マスターメールステータスが追加され、これはリード詳細レコードで確認できる登録解除フラグとは別に機能します。

登録解除フラグを false から true に変更すると、マスターメールステータスが更新され、その変更は同じメールアドレスを持つ他のリードにも反映されます。リードをインポートするとき、登録解除フラグはインポート操作によって&#x200B;**上書きされません**。

>[!NOTE]
>
>永続的な登録解除は、Marketo データベース全体のすべてのパーティションで機能します。

## 登録解除フラグを true から false に更新（再度の配信登録） {#update-the-unsubscribe-flag-from-true-to-false-e-g-re-subscribe-a-person}

リードを再度配信登録するには、いくつかの方法があります。

Salesforce では、リード／連絡先のレコードにある「メールオプトアウト」フィールドを&#x200B;**クリア**&#x200B;します。これで Marketo に同期されます。

![](assets/one.png)

Marketo では、リードのレコードで「リード情報」タブの「登録解除」フィールドを&#x200B;**クリア**&#x200B;します。

![](assets/two.png)

1 つまたは複数のリードで、「**データ値を変更**」フローステップを実行します。

![](assets/three.png)

SOAP API を介して既存のリードを更新します。

## 新しいリードの作成 {#creating-a-new-person}

新しいリードを作成すると、マスターメールステータスのテーブルと照合されます。リードを以前に登録解除した場合、そのレコードは登録解除として更新されます。

## メールアドレスの変更 {#changing-an-email-address}

リードのメールアドレスを登録解除に変更すると、そのリードは登録解除になります。この変更は、Marketo でも Salesforce でも発生します。

登録解除のメールアドレスを登録済みに変更すると、そのリードは登録済みになります。

## 再度の配信登録 {#re-subscribing}

登録解除すると、同じメールアドレスを使っているリードがすべて登録解除になるように、再度配信登録すると、同じメールアドレスを使っているどのリードも再度配信登録されます。

## アクティビティログ {#activity-log}

_updateLeadEmailStatus_ と _resetLeadEmailStatus_ のデータ値変更の定義は、[このコミュニティの記事](https://nation.marketo.com/t5/Knowledgebase/Durable-Unsubscribe-Activity-Log/ta-p/252688)に記載されています。

>[!MORELIKETHIS]
>
>[登録解除について](/help/marketo/product-docs/email-marketing/deliverability/understanding-unsubscribe.md)
