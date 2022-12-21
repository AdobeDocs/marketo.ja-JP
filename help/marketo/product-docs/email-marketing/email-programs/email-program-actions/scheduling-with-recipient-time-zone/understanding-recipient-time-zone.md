---
unique-page-id: 12983291
description: 受信者タイムゾーンについて — Marketo ドキュメント — 製品ドキュメント
title: 受信者タイムゾーンについて
exl-id: 8895241e-94c9-43a2-9158-11c1994df09b
source-git-commit: 46812deb41ed56328a4a64fbd36340d13c50dde4
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 100%

---

# 受信者タイムゾーンについて {#understanding-recipient-time-zone}

メールおよびエンゲージメントプログラムは、受信者のタイムゾーンに従って配信するように設定できるので、複数のプログラムを作成する必要がなくなります。1 度送信すると、メールは自動的にローカルで正しい時間まで保持されます。

>[!NOTE]
>
>受信者タイムゾーンは現在&#x200B;**メールコンテンツのみ**&#x200B;で機能します。デフォルトのエンゲージメントプログラムに対しては機能しません。

## メールプログラム {#email-programs}

[メールプログラムのスケジュール](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)には、次の 2 つの主なシナリオが考えられます。

1. 今後 25 時間以内に実行するようにプログラムをスケジュールする。
1. 25 時間以上後（例：来週）に実行するようにプログラムをスケジュールする。

各タイムゾーンに対応するために、受信者タイムゾーンでスケジュールされたメールプログラムの実行は、世界で&#x200B;**一番早い／最初の**&#x200B;タイムゾーン（UTC +14:00）で開始されます。

## エンゲージメントプログラム {#engagement-programs}

[エンゲージメントプログラムストリームをスケジュール](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md)して受信者のタイムゾーンがアクティブな場合、プログラムキャストは午前 0 時（UTC +14:00）に実行を開始します。ユーザーは世界中のすべてのタイムゾーンでキャストの対象として認定される可能性があるので、最初のキャストを少なくとも 25 時間後（24 時間+キャンペーンの開始までしばらく）にスケジュールする必要があります。UTC +14:00 で処理を開始すると、キャストに該当するすべてのユーザーに対して、スケジュールされた日時にメールが送信されることが保証されます。

## タイムゾーンの計算 {#calculating-time-zone}

Marketo は、ユーザーの市区町村、都道府県、国または郵便番号に基づいてタイムゾーンを計算します。これらの値からタイムゾーンを計算できない場合は、推測される市区町村、推測される都道府県、推測される国、推測される郵便番号の各フィールドが使用されます。

国&#x200B;**のみ**&#x200B;または州&#x200B;**のみ**&#x200B;の場合は、次のようになります。

* 3 つ以下のタイムゾーンを持つ国の場合は、真ん中のタイムゾーンが選択されます。
* 2 つのタイムゾーンを持つ州の場合は、2 つのうち早いほうが選択されます。

これらのフィールドの組み合わせによってもユーザーのタイムゾーンを判断できない場合、タイムゾーンは割り当て&#x200B;**られず**、メールは Marketo サブスクリプションのタイムゾーンに基づいて送信されます。したがって、プログラムが午前 9 時（PDT）にスケジュールされている場合、タイムゾーンが割り当てられていないユーザーへのメールは午前 9 時（PDT）に送信されます。

>[!NOTE]
>
>上記の入力フィールドのいずれかが変更された場合、ユーザーのタイムゾーンは自動的に再計算されます。

>[!MORELIKETHIS]
>
>* [受信者タイムゾーンを使用したメールプログラムのスケジュール設定](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [メールプログラムのヘッドスタート](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>
>* [受信者タイムゾーンを使用してエンゲージメントプログラムをスケジュールする](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md)

