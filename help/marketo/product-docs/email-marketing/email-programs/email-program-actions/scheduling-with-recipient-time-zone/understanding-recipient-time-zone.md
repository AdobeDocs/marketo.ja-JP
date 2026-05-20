---
unique-page-id: 12983291
description: メールプログラムの受信者タイムゾーンのスケジュール設定について説明します。 各受信者に対して、同じ現地時間で電子メールを配信します。
title: 受信者タイムゾーンについて
exl-id: 8895241e-94c9-43a2-9158-11c1994df09b
feature: Email Programs
TQID: https://experienceleague.adobe.com/KAj3dO4Md7Zel5SqR4m2OrTjp93ZD735gNWWRinNV5k
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 409
ht-degree: 63%

---

# 受信者タイムゾーンについて {#understanding-recipient-time-zone}

受信者のタイムゾーンに合わせて電子メールやエンゲージメントプログラムを設定できるため、複数のプログラムを作成する必要がありません。一度送信すると、Marketoは適切な現地時間まで電子メールを自動的に保持します。

>[!NOTE]
>
>[!UICONTROL 受信者タイムゾーン]は現在メールコンテンツ&#x200B;**のみ**&#x200B;で機能します。 デフォルトのエンゲージメントプログラムに対しては機能しません。

## メールプログラム {#email-programs}

[メールプログラムのスケジュール](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)には、次の 2 つの主なシナリオが考えられます。

1. 今後 25 時間以内に実行するようにプログラムをスケジュールする。
1. プログラムを25時間以上先に実行するようにスケジュール設定します（つまり、来週）。

すべてのタイムゾーンに対応するために、[!UICONTROL 受信者タイムゾーン &#x200B;]でスケジュールされたメールプログラムは、世界の&#x200B;**最初/最も早い** タイムゾーン （UTC +14:00）の午前0時に実行を開始します。

## エンゲージメントプログラム {#engagement-programs}

[&#x200B; エンゲージメントプログラムストリーム &#x200B;](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md)をスケジュールし、[!UICONTROL 受信者タイムゾーン &#x200B;]がアクティブな場合、プログラムキャストはUTC +14:00の午前0時に実行を開始します。 ユーザは世界中のすべてのタイムゾーンでキャストの対象として認定される可能性があるので、最初のキャストを少なくとも 25 時間後（24 時間+キャンペーンの開始までしばらく）にスケジュールする必要があります。 UTC +14:00でこの時間に処理を開始すると、このキャストに適格なすべてのユーザーに対して、スケジュールされた日時に電子メールが送信されます。

## タイムゾーンの計算 {#calculating-time-zone}

Marketo は、ユーザーの市区町村、都道府県、国または郵便番号に基づいてタイムゾーンを計算します。 これらの値からタイムゾーンを計算できない場合は、推測される市区町村、推測される都道府県、推測される国、推測される郵便番号の各フィールドが使用されます。

国&#x200B;**のみ**&#x200B;または州&#x200B;**のみ**&#x200B;の場合は、次のようになります。

* 3 つ以下のタイムゾーンを持つ国の場合は、真ん中のタイムゾーンが選択されます。
* 2 つのタイムゾーンを持つ州の場合は、2 つのうち早いほうが選択されます。

これらのフィールドの組み合わせによってもユーザーのタイムゾーンを判断できない場合、タイムゾーンは割り当て&#x200B;**られず**、メールは Marketo サブスクリプションのタイムゾーンに基づいて送信されます。 したがって、プログラムが午前 9:00am（PDT）にスケジュールされている場合、タイムゾーンが割り当てられていないユーザへのメールは午前 9:00am（PDT）に送信されます。

>[!NOTE]
>
>上記の入力フィールドのいずれかが変更された場合、ユーザのタイムゾーンは自動的に再計算されます。

>[!MORELIKETHIS]
>
>* [[!UICONTROL 受信者タイムゾーン]](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)を使用したメールプログラムのスケジュール設定
>* [メールプログラムのヘッドスタート](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>
>* [[!UICONTROL 受信者タイムゾーン]](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md)を使用したエンゲージメントプログラムのスケジュール設定
