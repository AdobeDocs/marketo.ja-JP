---
unique-page-id: 10097202
description: メールプログラムの優先スタート - Marketo ドキュメント - 製品ドキュメント
title: メールプログラムの優先スタート
exl-id: f7c8b082-4d83-4e3b-8aa4-7b252e3dacd3
feature: Email Programs
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 100%

---

# メールプログラムの優先スタート {#head-start-for-email-programs}

>[!PREREQUISITES]
>
>[メールプログラムの作成](/help/marketo/product-docs/email-marketing/email-programs/creating-an-email-program/create-an-email-program.md)

メールプログラムの日時を選択すると、プログラムの処理を開始するタイミングが決まります。選択した時刻にメールを起動させたい場合は、優先スタートがプログラムを事前に処理して、そのオプションを提供します。

## 標準優先スタート {#standard-head-start}

1. 「**[!UICONTROL マーケティングアクティビティ]**」をクリックします。

   ![](assets/one-1.png)

1. メールプログラムを選択します。

   ![](assets/selectemailprogram-4.jpg)

   >[!NOTE]
   >
   >優先スタートは A/B テストでは使用できません。

1. [!UICONTROL スケジュール]タイルで、メールのスケジュールを設定し、「**[!UICONTROL 優先スタート]**」ボックスを選択します。

   ![](assets/three-1.png)

   [!UICONTROL 優先スタート]を選択すると、プログラムは予定時間の約 12 時間前に処理を開始します。処理が開始されると、プログラムはロックされます。

   >[!CAUTION]
   >
   >プログラムのロック後に登録解除したオーディエンスは、引き続きメールを受け取ります。登録解除の通知を調整して、登録解除の処理に 1 ～ 2 営業日かかる場合があることを反映することをお勧めします。

1. 「**[!UICONTROL プログラムを承認]**」をクリックします。

   ![](assets/four-1.png)

   プログラムの承認後、承認タイルには、4 つの異なるステータスが表示されます。

   * **[!UICONTROL 実行待機中]：**&#x200B;プログラムが承認された後。
   * **[!UICONTROL 処理を開始しました。実行待機中]：**&#x200B;処理中です。
   * **[!UICONTROL 処理が完了しました。実行待機中]：**&#x200B;処理が完了しました。メールは、開始予定時間を待機中です。
   * **[!UICONTROL 終了]：**&#x200B;プログラムが完了しました。

   >[!TIP]
   >
   >プログラムがロックされた後、メールが送信される前なら、簡単にキャンセルできます。承認タイルの右下の「**[!UICONTROL プログラムを停止]**」をクリックするだけです。

   >[!NOTE]
   >
   >スケジュールされた実行時間の 12 時間前より後にメールプログラムの承認を取り消し、その後変更した場合は、承認の 12 時間以上後の新しい日時を選択する必要があります。

## 受信者タイムゾーンで優先スタート {#head-start-with-recipient-time-zone}

既存の優先スタート機能を使用するには、プログラムが少なくとも 12 時間前にスケジュールされている必要があります。受信者タイムゾーンとは何でしょうか。受信者タイムゾーンがアクティブになっている場合、最も早いタイムゾーン（UTC +14:00）の午前 0 時にメールプログラムの実行が開始されることを思い出してください。したがって、優先スタートと受信者の&#x200B;**両方**&#x200B;のタイムゾーンを有効にするには、プログラムを&#x200B;**最も早いタイムゾーン（UTC +14:00**）の少なくとも 12 時間前にスケジュールする必要があります。

つまり、米国ロサンゼルスにいて、優先スタートと受信者タイムゾーンの両方を有効にする場合は、プログラムを **34 時間**&#x200B;前にスケジュールする必要があります。どうやってこの数字にたどり着いたのでしょうか。

![](assets/image2017-12-5-13-3a11-3a46.png)

受信者タイムゾーンを使用したメールプログラムのスケジュール方法についての[詳細](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)をご覧ください。

>[!MORELIKETHIS]
>
>* [メールプログラムのスケジュール設定](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/schedule-your-email-program.md)
>* [受信者タイムゾーンを使用したメールプログラムのスケジュール設定](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [受信者タイムゾーンについて](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
