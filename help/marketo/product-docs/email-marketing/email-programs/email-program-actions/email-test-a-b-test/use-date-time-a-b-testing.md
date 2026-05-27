---
unique-page-id: 2359520
description: メールプログラムの日時A/B テストを実行する方法について説明します。 異なる送信時間をテストし、パフォーマンスごとに勝者を選択します。
title: 「日付／時間」A/B テストの使用
exl-id: ee686d46-9427-4f8b-a16f-858c5109cabd
feature: Email Programs, A/B Testing
TQID: https://experienceleague.adobe.com/V3lRJlUSegVZJbrhyPJRAKopziqMdmpseC16EFLGzrU
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 277
ht-degree: 73%

---

# 「日付／時間」A/B テストの使用 {#use-date-time-a-b-testing}

メールの A/B テストはとても簡単に実施できます。 1 つは&#x200B;**[!UICONTROL 日時]**&#x200B;テストです。 このテストでは、メールの送信に最適な時間帯または曜日をテストします。 その設定方法を説明しましょう。

>[!PREREQUISITES]
>
>[A/B テストの追加](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)
>

1. **[!UICONTROL メール]**&#x200B;タイルの下で、「**[!UICONTROL A/B テストを追加]**」をクリックします。

   ![](assets/image2014-9-12-15-3a41-3a3.png)

1. 新しいウィンドウが開きます。 「**[!UICONTROL テストタイプ]**」で「**[!UICONTROL 日時]**」を選択します。

   ![](assets/image2014-9-12-15-3a41-3a12.png)

1. 既存のテスト情報（件名テストなど）がある場合は、「**[!UICONTROL テストのリセット]**」をクリックします。

   ![](assets/image2014-9-12-15-3a41-3a19.png)

1. 最初の日時の日付を選択します。

   ![](assets/image2014-9-12-15-3a41-3a26.png)

1. 最初の日時の時刻を選択します。

   ![](assets/image2014-9-12-15-3a41-3a33.png)

1. 2 回目の日時にも同じ操作をおこないます。

   ![](assets/image2014-9-12-15-3a41-3a40.png)

1. A/B テストを送信したいオーディエンスの割合をスライダーで選択して、「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/image2014-9-12-15-3a41-3a53.png)

   >[!NOTE]
   >
   >それぞれのバリエーションの割合は、選択された「テストサンプルサイズ」を等分したものとなります。

   >[!CAUTION]
   >
   >**サンプルサイズを 100% に設定しないことをお勧めします**。 静的リストを使用している場合、サンプルサイズを100%に設定すると、オーディエンス全員にメールが送信され、勝者は誰にも送信されません。 **smart** リストを使用している場合、サンプルサイズを100%に設定すると、その時点で&#x200B;_オーディエンスのすべてのユーザーにメールが送信されます。_ メールプログラムが後日再実行されると、スマートリストに振り分けられた新しいリードも、オーディエンスに含まれるようになっているのでメールを受け取ります。

   ここまで来れば、あと一歩です。 続いて、[A/B テストの勝者の条件を定義](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md)する必要があります。
