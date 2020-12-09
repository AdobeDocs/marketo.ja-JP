---
unique-page-id: 12983291
description: 受信者のタイムゾーンについて — Marketto Docs — 製品ドキュメント
title: 受信者のタイムゾーンについて
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---


# 受信者のタイムゾーンについて {#understanding-recipient-time-zone}

受信者のタイムゾーンに従って電子メールやエンゲージメントのプログラムを配信するように設定できるため、複数のプログラムを作成する必要がなく、1回だけ送信すると、Marketoはローカルの正しい時刻まで電子メールを自動的に保持します。

>[!NOTE]
>
>受信者タイムゾーンは、現在、電子メールコンテンツ **でのみ機能します** 。 デフォルトのエンゲージメントプログラムでは機能しません。

## 電子メールプログラム {#email-programs}

電子メールプログラムを [スケジュールする場合、主に次の2つのシナリオがあります](schedule-email-programs-with-recipient-time-zone.md)。

1. 次の25時間以内にプログラムを実行するようにスケジュールします。
1. プログラムを25時間以上（翌週など）実行するようにスケジュールする。

各タイムゾーンに対応するために、受信者のタイムゾーン開始がスケジュールされた電子メールプログラムは、世界の **最初または最も古いタイムゾーン(UTC +14:00)の深夜** に実行されます。

## アクションプログラム {#engagement-programs}

エンゲージメントプログラムストリーム [、および受信者タイムゾーンがアクティブであることを](../../../../../product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md) スケジュールする場合、プログラムキャストはUTC +14:00の深夜に実行される開始です。 世界中のすべてのタイムゾーンでキャストの資格を得られる可能性があるので、少なくとも25時間(キャンペーンを開始するには24時間+一定時間)後に最初のキャストをスケジュールする必要があります。 この時刻にUTC +14:00で処理を開始すると、このキャストに該当するすべての人に対して、予定された日時に電子メールが配信されます。

## タイムゾーンの計算 {#calculating-time-zone}

Marketorは、人の市区町村、都道府県、国または郵便番号に基づいてタイムゾーンを計算します。 これらの値から誰かのタイムゾーンを計算できない場合は、推定市区町村、推定国、推定郵便番号の各フィールドに戻します。

***only **Country or **only** State availableの場合：

* タイムゾーンが3つ以下の国の場合は、中間タイムゾーンを選択します。
* 2つのタイムゾーンを持つ州の場合は、2つのタイムゾーンのうち、前の方を選択します。

これらのフィールドの組み合わせによって、ユーザーのタイムゾーンがまだ特定できない場合、タイムゾーンは割り当て **られません** 。電子メールは、マーケティング担当者の購読タイムゾーンに基づいて配信されます。 したがって、プログラムが午前9時のPDTに予定されている場合、タイムゾーンが割り当てられていないユーザーは、午前9時のPDTに電子メールを受信します。

>[!NOTE]
>
>上記の入力フィールドのいずれかが変更された場合に、ユーザーのタイムゾーンが自動的に再計算されます。

>[!MORELIKETHIS]
>
>* [受信者のタイムゾーンでの電子メールプログラムのスケジュール](schedule-email-programs-with-recipient-time-zone.md)
>* [電子メールプログラムのヘッド開始](../../../../../product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)

   >
   >
* [受信者のタイムゾーンでのエンゲージメントプログラムのスケジュール](../../../../../product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md)

>



