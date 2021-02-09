---
unique-page-id: 12983291
description: 受信者のタイムゾーンについて — Marketto Docs — 製品ドキュメント
title: 受信者のタイムゾーンについて
translation-type: tm+mt
source-git-commit: 8d45a28e1c2adad3e04645f7150f1757414092f0
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---


# 受信者のタイムゾーンについて{#understanding-recipient-time-zone}

受信者のタイムゾーンに従って電子メールやエンゲージメントのプログラムを配信するように設定できるため、複数のプログラムを作成する必要がなく、1回だけ送信すると、Marketoはローカルの正しい時刻まで電子メールを自動的に保持します。

>[!NOTE]
>
>受信者タイムゾーンは、現在、電子メールコンテンツと共に&#x200B;****&#x200B;のみ機能します。 デフォルトのエンゲージメントプログラムでは機能しません。

## 電子メールプログラム{#email-programs}

[電子メールプログラム](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)をスケジュールする場合、主に次の2つのシナリオが考えられます。

1. 次の25時間以内にプログラムを実行するようにスケジュールします。
1. プログラムを25時間以上（翌週など）実行するようにスケジュールする。

各タイムゾーンに対応するために、受信者のタイムゾーン開始がスケジュールされた電子メールプログラムは、世界の&#x200B;**最初/最も古い**&#x200B;タイムゾーンの午前0時(UTC +14:00)に実行されます。

## アクションプログラム{#engagement-programs}

[エンゲージメントプログラムストリーム](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md)をスケジュールし、受信者タイムゾーンがアクティブな場合、プログラムキャストはUTC +14:00で実行される開始です。 世界中のすべてのタイムゾーンでキャストの資格を得られる可能性があるので、少なくとも25時間(キャンペーンを開始するには24時間+一定時間)後に最初のキャストをスケジュールする必要があります。 この時刻にUTC +14:00で処理を開始すると、このキャストに該当するすべての人に対して、予定された日時に電子メールが配信されます。

## タイムゾーンの計算{#calculating-time-zone}

Marketorは、人の市区町村、都道府県、国または郵便番号に基づいてタイムゾーンを計算します。 これらの値から誰かのタイムゾーンを計算できない場合は、推定市区町村、推定国、推定郵便番号の各フィールドに戻します。

**唯一**&#x200B;国または&#x200B;**のみ**&#x200B;の州が使用可能な場合：

* タイムゾーンが3つ以下の国の場合は、中間タイムゾーンを選択します。
* 2つのタイムゾーンを持つ州の場合は、2つのタイムゾーンのうち、前の方を選択します。

これらのフィールドの組み合わせで、まだ誰かのタイムゾーンを判断できない場合は、タイムゾーンを割り当てない&#x200B;****&#x200B;ので、Marketor購読のタイムゾーンに基づいて電子メールが配信されます。 したがって、プログラムが午前9時のPDTに予定されている場合、タイムゾーンが割り当てられていないユーザーは、午前9時のPDTに電子メールを受信します。

>[!NOTE]
>
>上記の入力フィールドのいずれかが変更された場合に、ユーザーのタイムゾーンが自動的に再計算されます。

>[!MORELIKETHIS]
>
>* [受信者のタイムゾーンでの電子メールプログラムのスケジュール](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [電子メールプログラムのヘッド開始](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)

   >
   >
* [受信者のタイムゾーンでのエンゲージメントプログラムのスケジュール](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md)

