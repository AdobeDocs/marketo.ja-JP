---
unique-page-id: 2359504
description: 送信元アドレスのA/B テストを実行する方法について説明します。 さまざまな送信者アドレスをテストし、パフォーマンスごとに勝者を選択します。
title: 「送信元アドレス」A/B テストを使用する
exl-id: 83e2994b-39ec-4c88-87b0-8f2501ea2bf1
feature: Email Programs, A/B Testing
TQID: 'https://experienceleague.adobe.com/rerG-Wyn1X53QQBDXFwyg74uEOznGcYcBis9EwX4vQU'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
    internal-label: Programs
  - id: 69a7f8d6-582c-5b66-841e-32cf07fd164c
    internal-label: A/B Testing
  - id: c2dbad80-0f5c-4d96-a798-2a65f93b8721
    internal-label: Assets
subfeature_v2:
  - id: c0f0afc1-a5a8-4b01-8b43-cc38f9169499
    internal-label: Email programs
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 74%
---
# 「[!UICONTROL 送信元アドレス]」A/B テストを使用する {#use-from-address-a-b-testing}

メールの A/B テストはとても簡単に実施できます。 なかでも興味深いのが、**[!UICONTROL 送信元アドレス]**&#x200B;テストです。 その設定方法を説明します。

>[!PREREQUISITES]
>
>[A/B テストの追加](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

1. 「**[!UICONTROL メール]**」タイルで、目的のメールを選択して「**[!UICONTROL A/B テストの追加]**」をクリックします。

   ![](assets/image2014-9-12-15-3a32-3a8.png)

1. 新しいウィンドウが開かれるので、「**[!UICONTROL テストタイプ]**」で「**[!UICONTROL 送信元アドレス]**」を選択します。

   ![](assets/image2014-9-12-15-3a32-3a22.png)

1. 既存のテスト情報（件名テストなど）がある場合は、「**[!UICONTROL テストのリセット]**」をクリックします。

   ![](assets/image2014-9-12-15-3a32-3a28.png)

1. テストする 2 つ目の&#x200B;**[!UICONTROL 送信元アドレス]**&#x200B;情報を入力します。

   >[!NOTE]
   >
   >選択 A には、選択したメールに含まれる情報が事前入力されます。

   ![](assets/image2014-9-12-15-3a32-3a34.png)

   >[!TIP]
   >
   >「**+**」をクリックして、送信元アドレスを必要な数だけ追加できます。

1. A/B テストを送信したいオーディエンスの割合をスライダーで選択して、「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/image2014-9-12-15-3a33-3a41.png)

   >[!NOTE]
   >
   >それぞれのバリエーションの割合は、選択された「テストサンプルサイズ」を等分したものとなります。

   >[!CAUTION]
   >
   >**サンプルサイズを 100% に設定しないことをお勧めします**。 静的リストを使用している場合、サンプルサイズを100%に設定すると、オーディエンス全員にメールが送信され、勝者は誰にも送信されません。 **smart** リストを使用している場合、サンプルサイズを100%に設定すると、その時点で&#x200B;_オーディエンスのすべてのユーザーにメールが送信されます。_ メールプログラムが後日再度実行されると、スマートリストの条件を満たすようになった新しい人物も、オーディエンスに含まれるためメールを受け取ります。

   ここまで来れば、あと一歩です。 続いて、[A/B テストの勝者の条件を定義](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md)する必要があります。
