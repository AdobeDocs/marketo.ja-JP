---
unique-page-id: 7514918
description: Marketoの購読解除タイプについて説明します（購読解除、マーケティング休止、購読解除）。 キャンペーンの各シナリオに「適切な」フィールドを使用します。
title: 登録解除について
exl-id: 30866dc0-cdac-4e73-8dbf-d4b509012269
feature: Deliverability
TQID: https://experienceleague.adobe.com/zmsCI3a7GECVNiuFjtjqgDQsjelBoccugPeuzAF4c4k
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b0bb9048-d951-48d8-8232-45cf248a7e27
source-git-commit: 39b6fecdc7aa16ab1205582d3bf372a8538a2d35
workflow-type: tm+mt
source-wordcount: 238
ht-degree: 68%

---

# 登録解除について {#understanding-unsubscribe}

Marketoには、組み込みの登録解除にはいくつかの種類があります。 ファーストネームと同様に、すべてperson オブジェクトのフィールドで表されます。

これらのフィールドはすべて、Marketo での登録にビルトインされています。 これらはすべてブール型（チェックボックス）です。 これらは Forms または[データ値を変更](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md)フローステップで使用できます。

## 配信停止完了 {#unsubscribed}

これは、標準の登録解除ページで使用されます。 ユーザーがこのボックスをオンにした場合、または電子メールの登録解除リンクをクリックした場合、そのユーザーはマーケティング電子メールを受け取らなくなります。 ただし、[オペレーショナルメール](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)は受け取ります。

## マーケティングを中断したリード {#marketing-suspended}

このフィールドは、ユーザーが一時的な登録解除にリードを配置するために設定します。 リードは、手動で変更した場合、またはデータ値の変更フローステップを利用した場合にのみ、このステータスを達成できます。

## メールの中断 {#email-suspended}

このステータスは、ハードバウンスが発生してから 24 時間、リードへのメール送信をブロックします。 24 時間後、その人物は再びメールを利用できるようになります。

>[!NOTE]
>
>メールの中断は、24 時間が過ぎてもチェックされたままになるので、過去にそのようにマークされた人を指すことができます。 顧客が郵送可能かどうかを確認するには、電子メールの配信を停止してから24時間後に計算します。

## ブロックリスト登録済み {#blocklisted}

[競合他社などの人物に使用](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.md)。 **no**&#x200B;のメールを受信したい方は誰でも、運用上、マーケティング上などのメールを受信できます。メールは届きません。

![](assets/image2015-5-18-12-3a6-3a40.png)
