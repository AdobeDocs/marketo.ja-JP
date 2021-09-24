---
unique-page-id: 12983291
description: 受信者のタイムゾーンについて — Marketoドキュメント — 製品ドキュメント
title: 受信者タイムゾーンを理解する
exl-id: 8895241e-94c9-43a2-9158-11c1994df09b
source-git-commit: 46812deb41ed56328a4a64fbd36340d13c50dde4
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 6%

---

# 受信者タイムゾーンを理解する {#understanding-recipient-time-zone}

Eメールおよびエンゲージメントプログラムは、受信者のタイムゾーンに従って配信するように設定できるので、複数のプログラムを作成する必要がなくなり、1回送信するだけで、Marketoはローカル時間が正しくなるまでEメールを自動的に保持します。

>[!NOTE]
>
>受信者のタイムゾーンは、現在、電子メールコンテンツで&#x200B;**のみ**&#x200B;機能します。 デフォルトのエンゲージメントプログラムでは機能しません。

## メールプログラム {#email-programs}

[電子メールプログラム](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)をスケジュールする場合、主に次の2つのシナリオが考えられます。

1. 次の25時間以内に実行するようにプログラムをスケジュールします。
1. 25時間以上後（例：来週）に実行するようにプログラムをスケジュールします。

各タイムゾーンに対応するために、受信者のタイムゾーンでスケジュールされた電子メールプログラムは、世界の&#x200B;**最初/最も早い**&#x200B;タイムゾーンの午前0時(UTC +14:00)に開始されます。

## エンゲージメントプログラム {#engagement-programs}

[スケジュールを設定し、エンゲージメントプログラムストリーム](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md)と受信者のタイムゾーンがアクティブになると、プログラムキャストはUTC +14:00の真夜中に実行を開始します。 ユーザーは世界中のすべてのタイムゾーンでキャストの資格を得る可能性があるので、最初のキャストを少なくとも25時間（24時間+キャンペーンを開始する時間）後にスケジュールする必要があります。 この時点での処理をUTC +14:00に開始すると、このキャストの資格を持つすべての人に対して、スケジュールされた日時にEメールを送信することが保証されます。

## タイムゾーンの計算 {#calculating-time-zone}

Marketoは、人の市区町村、都道府県、国または郵便番号に基づいてタイムゾーンを計算します。 これらの値から他のユーザーのタイムゾーンを計算できない場合は、「推定都市」、「推定州」、「推定国」および「推定郵便番号」の各フィールドに戻ります。

**唯一の**&#x200B;国または&#x200B;**のみ**&#x200B;の州がある場合：

* タイムゾーンが3つ以下の国の場合は、中間タイムゾーンを選択します。
* 2つのタイムゾーンのある状態の場合、前の2つを選択します。

これらのフィールドの組み合わせでもタイムゾーンが判断できない場合は、タイムゾーンを割り当てません。****&#x200B;電子メールはMarketoのサブスクリプションタイムゾーンに基づいて送信されます。 したがって、プログラムが午前9時にPDTに予約されている場合、タイムゾーンが割り当てられていない人は、午前9時に電子メールを送信します。

>[!NOTE]
>
>Marketoは、上記の入力フィールドのいずれかが変更された場合、自動的にタイムゾーンを再計算します。

>[!MORELIKETHIS]
>
>* [受信者タイムゾーンを使用してメールプログラムをスケジュールする](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [メールプログラムのヘッドスタート](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>
>* [受信者のタイムゾーンに対するエンゲージメントプログラムのスケジュール](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md)

