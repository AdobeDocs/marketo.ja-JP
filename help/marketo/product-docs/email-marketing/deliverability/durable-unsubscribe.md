---
unique-page-id: 10094576
description: 永続的な配信停止について学び、マスターメールのステータスが人々にどのように反映されるかをご確認ください。 Marketoで再購読と人物レコードを管理します。
title: 永続的な登録解除
exl-id: e03a5a01-7395-45b3-8351-7931ec413236
feature: Deliverability
TQID: https://experienceleague.adobe.com/Zr7XyDDSHtWW4lp4ATAM6xlPrNnTJlqoOOjjln-YuqI
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
source-git-commit: 39b6fecdc7aa16ab1205582d3bf372a8538a2d35
workflow-type: tm+mt
source-wordcount: 304
ht-degree: 73%

---

# 永続的な登録解除 {#durable-unsubscribe}

Marketo で登録解除が「永続的」になるように、機能が強化されました。 マスターメールのステータスが追加されました。これは、人物の詳細レコードに表示される購読解除フラグとは別のものです。

登録解除フラグを false から true に変更すると、マスターメールステータスが更新され、その変更は同じメールアドレスを持つ他のリードにも反映されます。 リードが削除されて再作成されるとき、または新規レコードが同じメールアドレスで作成されるとき、登録解除フラグは&#x200B;**上書きされません**。

>[!NOTE]
>
>永続的な登録解除は、Marketo データベース全体のすべてのパーティションで機能します。

## 登録解除フラグを true から false に更新（再度の配信登録） {#update-the-unsubscribe-flag-from-true-to-false-e-g-re-subscribe-a-person}

リードを再度配信登録するには、いくつかの方法があります。

Salesforce では、リード／取引先責任者のレコードにある「メールオプトアウト」フィールドをクリアします。 これで Marketo に同期されます。

![Salesforce 画面](assets/durable-unsubscribe-1.png)

Marketo では、ユーザのレコードの「情報」タブにある登録解除ボックスをオフにします。

![ユーザレコードの登録解除ボックスをオフにする &#x200B;](assets/durable-unsubscribe-2.png)

1 つまたは複数のユーザで、「**[!UICONTROL データ値を変更]**」フローステップを実行します。

![「データ値を変更」フローステップ](assets/durable-unsubscribe-3.png)

## 新しいリードの作成 {#creating-a-new-person}

新しいリードを作成すると、マスターメールステータスのテーブルと照合されます。 以前に購読解除されていた場合、レコードは購読解除に更新されます。

## メールアドレスの変更 {#changing-an-email-address}

リードのメールアドレスを登録解除に変更すると、そのリードは登録解除になります。 この変更は、Marketo でも [!DNL Salesforce] でも発生します。

## 再度の配信登録 {#re-subscribing}

登録解除すると、同じメールアドレスを持つすべてのユーザーが登録解除されるのと同様に、再登録では、同じメールアドレスを持つすべてのユーザーが再度登録されます。

>[!MORELIKETHIS]
>
>[登録解除について](/help/marketo/product-docs/email-marketing/deliverability/understanding-unsubscribe.md)
