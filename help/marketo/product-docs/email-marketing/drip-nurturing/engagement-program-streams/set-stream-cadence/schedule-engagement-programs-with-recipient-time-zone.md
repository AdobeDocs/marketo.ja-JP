---
unique-page-id: 12982909
description: 受信者のタイムゾーンを使用してエンゲージメントプログラムのキャストをスケジュールする方法について説明します。 最初のキャストを少なくとも25時間先に設定して、グローバル配信を行います。
title: 受信者タイムゾーンを使用してエンゲージメントプログラムをスケジュールする
exl-id: 818615be-3c7e-4051-adc7-2341783484b9
feature: Engagement Programs
TQID: 'https://experienceleague.adobe.com/PkmvMBNzpWUNrJy9K-4TVrJMBWfKp5Vm2K-jiIeKBVg'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
    internal-label: Programs
  - id: c2dbad80-0f5c-4d96-a798-2a65f93b8721
    internal-label: Assets
subfeature_v2:
  - id: fc5011cf-5b46-40b1-a5de-d7f042f85633
    internal-label: Engagement programs
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 36%
---
# 受信者タイムゾーンを使用してエンゲージメントプログラムをスケジュールする {#schedule-engagement-programs-with-recipient-time-zone}

エンゲージメントプログラムストリームをスケジュールし、受信者タイムゾーンがアクティブな場合、プログラムキャストは最初のタイムゾーン（UTC +14:00）の午前0時に実行を開始します。 最初のキャストは、世界中のあらゆるタイムゾーンでキャストの資格を持つ人がいる可能性があるため、今後&#x200B;**少なくとも25時間**&#x200B;にスケジュールする必要があります。 1つ目のタイムゾーンでこの時間に処理を開始すると、電子メールがすべての受信者に対してスケジュールされた日時に配信されることが保証されます。

1. エンゲージメントプログラムで、「**[!UICONTROL ストリーム]**」タブをクリックし、ストリームのケイデンススケジュールをクリックして編集します。

   ![](assets/image2017-12-5-13-3a36-3a21.png)

1. 通常どおりに[ケイデンス設定を指定](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence.md)してから、「**[!UICONTROL 受信者タイムゾーン]**」ボックスをクリックします。 最初のキャストは、少なくとも 25 時間後である必要があります。 「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2017-12-5-13-3a50-3a32.png)

1. 受信者タイムゾーンがアクティブな場合、複数のタイムゾーンが存在する可能性があるため、ケイデンススケジュールには特定のタイムゾーンは表示されません。 時間のみが表示されます。

   ![](assets/image2017-12-5-13-3a56-3a21.png)

>[!MORELIKETHIS]
>
>* [受信者タイムゾーンについて](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [ストリームケイデンスの設定](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence.md)
