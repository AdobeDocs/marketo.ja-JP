---
unique-page-id: 12983291
description: 受信者タイムゾーンについて — Marketo ドキュメント — 製品ドキュメント
title: 受信者タイムゾーンについて
exl-id: 8895241e-94c9-43a2-9158-11c1994df09b
feature: Email Programs
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 67%

---

# 受信者タイムゾーンについて {#understanding-recipient-time-zone}

メールとエンゲージメントプログラムを受信者のタイムゾーンに応じて配信するように設定すると、複数のプログラムを作成する必要がなくなります。1 回送信すると、Marketoによって、正しい現地時間までメールが自動保持されます。

>[!NOTE]
>
>[!UICONTROL 受信者タイムゾーン]は現在メールコンテンツ&#x200B;**のみ**&#x200B;で機能します。デフォルトのエンゲージメントプログラムに対しては機能しません。

## メールプログラム {#email-programs}

[メールプログラムのスケジュール](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)には、次の 2 つの主なシナリオが考えられます。

1. 今後 25 時間以内に実行するようにプログラムをスケジュールする。
1. 25 時間以上先（来週）に実行するようにプログラムをスケジュールする。

すべてのタイムゾーンに対応するために、[!UICONTROL &#x200B; 受信者タイムゾーン &#x200B;] でスケジュールされたメールプログラムは、世界の **最初/最も早い** タイムゾーン（UTC +14:00）の午前 0 時に実行を開始します。

## エンゲージメントプログラム {#engagement-programs}

[ エンゲージメントプログラムストリームのスケジュール ](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md) と [!UICONTROL &#x200B; 受信者のタイムゾーン &#x200B;] がアクティブになると、プログラムキャストは UTC +14:00 の午前 0 時に実行を開始します。 ユーザは世界中のすべてのタイムゾーンでキャストの対象として認定される可能性があるので、最初のキャストを少なくとも 25 時間後（24 時間+キャンペーンの開始までしばらく）にスケジュールする必要があります。この時間に UTC +14 で処理を開始すると :00 このキャストの対象となるすべての人物に対して、スケジュールされた日時にメールが送信されることが保証されます。

## タイムゾーンの計算 {#calculating-time-zone}

Marketo は、ユーザーの市区町村、都道府県、国または郵便番号に基づいてタイムゾーンを計算します。これらの値からタイムゾーンを計算できない場合は、推測される市区町村、推測される都道府県、推測される国、推測される郵便番号の各フィールドが使用されます。

国&#x200B;**のみ**&#x200B;または州&#x200B;**のみ**&#x200B;の場合は、次のようになります。

* 3 つ以下のタイムゾーンを持つ国の場合は、真ん中のタイムゾーンが選択されます。
* 2 つのタイムゾーンを持つ州の場合は、2 つのうち早いほうが選択されます。

これらのフィールドの組み合わせによってもユーザーのタイムゾーンを判断できない場合、タイムゾーンは割り当て&#x200B;**られず**、メールは Marketo サブスクリプションのタイムゾーンに基づいて送信されます。したがって、プログラムが午前 9:00am（PDT）にスケジュールされている場合、タイムゾーンが割り当てられていないユーザへのメールは午前 9:00am（PDT）に送信されます。

>[!NOTE]
>
>上記の入力フィールドのいずれかが変更された場合、ユーザのタイムゾーンは自動的に再計算されます。

>[!MORELIKETHIS]
>
>* [[!UICONTROL 受信者タイムゾーン]](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)を使用したメールプログラムのスケジュール設定
>* [メールプログラムのヘッドスタート](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>
>* [[!UICONTROL 受信者タイムゾーン]](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md)を使用したエンゲージメントプログラムのスケジュール設定
