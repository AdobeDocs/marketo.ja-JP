---
unique-page-id: 10097202
description: 電子メールプログラム向けのヘッド開始-Marketoドキュメント — 製品ドキュメント
title: 電子メールプログラムのヘッド開始
exl-id: f7c8b082-4d83-4e3b-8aa4-7b252e3dacd3
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 0%

---

# 電子メールプログラムのヘッド開始{#head-start-for-email-programs}

>[!PREREQUISITES]
>
>[電子メールプログラムの作成](/help/marketo/product-docs/email-marketing/email-programs/creating-an-email-program/create-an-email-program.md)

電子メールプログラムの日付/時刻を選択すると、プログラムの処理を開始する日時が指定されます。 選択した時刻に電子メールを起動する場合は、ヘッド開始により、事前にプログラムを処理することでそのオプションが提供されます。

## 標準ヘッド開始{#standard-head-start}

1. 「**マーケティングアクティビティ**」をクリックします。

   ![](assets/one-1.png)

1. 電子メールプログラムを探して選択します。

   ![](assets/selectemailprogram-4.jpg)

   >[!NOTE]
   >
   >ヘッド開始はA/Bテストでは使用できません。

1. スケジュールタイルで、電子メールのスケジュールを設定し、「**ヘッド開始**」ボックスを選択します。

   ![](assets/three-1.png)

   ヘッド開始を選択した状態で、プログラムは、スケジュールされた時間の約12時間前に処理を開始します。 開始の処理が完了すると、プログラムはロックされます。

   >[!CAUTION]
   >
   >プログラムのロック後に購読を解除したオーディエンス上のユーザーは、全員が電子メールを受信します。 購読解除の通知を調整して、購読解除の処理に1 ～ 2営業日かかる場合があることを反映することをお勧めします。

1. 「**プログラムを承認**」をクリックします。

   ![](assets/four-1.png)

   プログラムの承認後、承認タイルに4つの異なるステータスが表示される場合があります。

   * **実行の待機中：プログラム** が承認された後。
   * **処理が開始されました。実行を待機中：** 処理が進行中です。
   * **処理が完了しました。実行の待機中：** 処理が完了しました。電子メールがスケジュールされた開始時間を待機するようになりました。
   * **完了：** プログラムが完了しました。

   >[!TIP]
   >
   >プログラムがロックされた後、電子メールが送信される前にキャンセルしますか？ 大丈夫！ 承認タイルの右下にある「プログラム&#x200B;**中止**」をクリックします。

   >[!NOTE]
   >
   >スケジュールされた実行時間の12時間未満で電子メールプログラムを未承認にし、その後変更した場合は、承認の12時間以上前の新しい日時を選択する必要があります。

## 受信者タイムゾーン{#head-start-with-recipient-time-zone}を持つヘッド開始

既存のヘッド開始機能では、プログラムを少なくとも12時間前にスケジュールする必要があります。 受信者のタイムゾーンの意味 受信者タイムゾーンがアクティブな場合、開始は最も早いタイムゾーン(UTC +14:00)の午前0時に電子メールプログラムを実行します。 したがって、**ヘッド開始と受信者タイムゾーンの両方**&#x200B;を有効にするには、プログラムは最も早いタイムゾーン(UTC +14:00 **)より少なくとも12時間早く**&#x200B;スケジュールする必要があります。

つまり、米国/ロサンゼルスにいて、ヘッド開始と受信者タイムゾーンの両方を有効にする場合は、事前にプログラム&#x200B;**34時間**&#x200B;をスケジュールする必要があります。 どうやってこの番号に着いた？

![](assets/image2017-12-5-13-3a11-3a46.png)

[受信者のタイムゾーンを使用して電子メールプログラムをスケジュールする方法につ](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md) いて詳しく説明します。

>[!MORELIKETHIS]
>
>* [電子メールプログラムのスケジュール](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/schedule-your-email-program.md)
>* [受信者のタイムゾーンでの電子メールプログラムのスケジュール](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [受信者のタイムゾーンについて](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)

