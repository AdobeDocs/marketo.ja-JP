---
unique-page-id: 12982909
description: 受信者タイムゾーンを使用してエンゲージメントプログラムをスケジュールする - Marketo ドキュメント - 製品ドキュメント
title: 受信者タイムゾーンを使用してエンゲージメントプログラムをスケジュールする
exl-id: 818615be-3c7e-4051-adc7-2341783484b9
feature: Engagement Programs
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 85%

---

# 受信者タイムゾーンを使用してエンゲージメントプログラムをスケジュールする {#schedule-engagement-programs-with-recipient-time-zone}

エンゲージメントプログラムストリームをスケジュールし、受信者のタイムゾーンがアクティブな場合、プログラムキャストは最初のタイムゾーン （UTC +14:00）の午前 0 時に実行を開始します。 最初のキャストのスケジュールは&#x200B;**少なくとも 25 時間**&#x200B;後に設定する必要があります。これは、世界中のすべてのタイムゾーンにキャストの資格があるユーザーがいる可能性があるので必要です。この時点で初めてのタイムゾーンで処理を開始すると、すべての受信者に対してスケジュールされた日時にメールが配信されます。

1. エンゲージメントプログラムで、「**[!UICONTROL ストリーム]**」タブをクリックし、ストリームのケイデンススケジュールをクリックして編集します。

   ![](assets/image2017-12-5-13-3a36-3a21.png)

1. 通常どおりに[ケイデンス設定を指定](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence.md)してから、「**[!UICONTROL 受信者タイムゾーン]**」ボックスをクリックします。最初のキャストは、少なくとも 25 時間後である必要があります。「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2017-12-5-13-3a50-3a32.png)

1. 受信者タイムゾーンがアクティブな場合、タイムゾーンは複数存在する可能性があるため、ケイデンススケジュールには特定のタイムゾーンが表示されません。時間のみが表示されます。

   ![](assets/image2017-12-5-13-3a56-3a21.png)

>[!MORELIKETHIS]
>
>* [受信者タイムゾーンについて](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [ストリームケイデンスの設定](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence.md)
