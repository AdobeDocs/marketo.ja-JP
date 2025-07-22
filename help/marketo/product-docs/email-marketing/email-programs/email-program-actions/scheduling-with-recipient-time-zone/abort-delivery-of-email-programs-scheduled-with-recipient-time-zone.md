---
unique-page-id: 13795727
description: 受信者タイムゾーンを使用してスケジュールされたメールプログラムの配信を中止する - Marketo ドキュメント - 製品ドキュメント
title: 受信者タイムゾーンを使用してスケジュールされたメールプログラムの配信を中止する
exl-id: e69afa4a-32fb-4791-a9b6-683d64d610d6
feature: Email Programs
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 90%

---

# 受信者タイムゾーンを使用してスケジュールされたメールプログラムの配信を中止する {#abort-delivery-of-email-programs-scheduled-with-recipient-time-zone}

万一の場合には、「受信者タイムゾーン」が有効化された状態ですでに起動しているメールプログラムの配信を中止することができます。

「受信者タイムゾーン」を使用してスケジュールされたメールプログラムは最大で 24 時間動作するため、プログラムの配信を中止すると、それ以降の後続のメール送信はすべてキャンセルされます。

1. キャンセルするメールプログラムを選択し、コントロールパネルの **[!UICONTROL 承認]** タイルの下にある [!UICONTROL &#x200B; 配信中止 &#x200B;] をクリックします。

   ![](assets/ptz-abortdelivery.png)

1. 「**[!UICONTROL 中止]**」をクリックして、配信のキャンセルを確認します。

   ![](assets/image2018-2-23-11-3a20-3a27.png)

1. 配信がキャンセルされると、メールプログラムの「**[!UICONTROL 実行結果]**」グリッドは以下のように表示されます。後続のメール送信はすべてキャンセルされて、**[!UICONTROL アクティビティタイプ]**&#x200B;列で「ソフトバウンスメール」と表示されます。

   ![](assets/image2018-2-23-11-3a22-3a11.png)

   >[!NOTE]
   >
   >キャンされたメールは、個々のタイムゾーンでの元の配信予定時間になる&#x200B;*までは*、「ソフトバウンス」として表示され&#x200B;**ません**。その時間までは「送信済みメール」として表示されます。

1. グリッドからメールをクリックすると、アクティビティの詳細を確認できます。キャンセルされたメール送信については、詳細のポップアップが以下のように表示されます。

   ![](assets/image2018-2-23-11-3a30-3a46.png)

>[!MORELIKETHIS]
>
>* [受信者タイムゾーンについて](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [受信者タイムゾーンを使用したメールプログラムのスケジュール設定](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
