---
unique-page-id: 10094576
description: 永続的な登録解除 - Marketo ドキュメント - 製品ドキュメント
title: 永続的な登録解除
exl-id: e03a5a01-7395-45b3-8351-7931ec413236
feature: Deliverability
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 97%

---

# 永続的な登録解除 {#durable-unsubscribe}

Marketo で登録解除が「永続的」になるように、機能が強化されました。マスターメールステータスが追加され、これはリード詳細レコードで確認できる登録解除フラグとは別に機能します。

登録解除フラグを false から true に変更すると、マスターメールステータスが更新され、その変更は同じメールアドレスを持つ他のリードにも反映されます。リードが削除されて再作成されるとき、または新規レコードが同じメールアドレスで作成されるとき、登録解除フラグは&#x200B;**上書きされません**。

>[!NOTE]
>
>永続的な登録解除は、Marketo データベース全体のすべてのパーティションで機能します。

## 登録解除フラグを true から false に更新（再度の配信登録） {#update-the-unsubscribe-flag-from-true-to-false-e-g-re-subscribe-a-person}

リードを再度配信登録するには、いくつかの方法があります。

Salesforce では、リード／取引先責任者のレコードにある「メールオプトアウト」フィールドをクリアします。これで Marketo に同期されます。

![Salesforce 画面](assets/durable-unsubscribe-1.png)

Marketo では、ユーザのレコードの「情報」タブにある登録解除ボックスをオフにします。

![ユーザレコードの登録解除ボックスをオフにする ](assets/durable-unsubscribe-2.png)

1 つまたは複数のユーザで、「_データ値を変更_」フローステップを実行します。

![「データ値を変更」フローステップ](assets/durable-unsubscribe-3.png)

## 新しいリードの作成 {#creating-a-new-person}

新しいリードを作成すると、マスターメールステータスのテーブルと照合されます。リードを以前に登録解除した場合、そのレコードは登録解除として更新されます。

## メールアドレスの変更 {#changing-an-email-address}

リードのメールアドレスを登録解除に変更すると、そのリードは登録解除になります。この変更は、Marketoまたは [!DNL Salesforce] で行われます。

## 再度の配信登録 {#re-subscribing}

登録解除すると、同じメールアドレスを使っているリードがすべて登録解除になるように、再度配信登録すると、同じメールアドレスを使っているどのリードも再度配信登録されます。

>[!MORELIKETHIS]
>
>[登録解除について](/help/marketo/product-docs/email-marketing/deliverability/understanding-unsubscribe.md)
