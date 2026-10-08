---
unique-page-id: 4719340
description: Web Personalizationで追跡される特定のIP アドレスまたはIP範囲を除外する方法について説明します。 アカウント設定でのトラッキングとレポートから従業員と組織を除外します。
title: 特定の IP をトラッキングから除外する
exl-id: d6989c8f-46ff-40a8-bf7f-5d34e701b359
feature: Web Personalization
TQID: 'https://experienceleague.adobe.com/iWnjpI93pHG0A5xXrQhz8EP7CB-4-QeNAaLh203-l5o'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
    internal-label: Reporting
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
    internal-label: Personalization
  - id: 664d862c-1673-5ed4-a3d6-386ac83225e4
    internal-label: Web Personalization
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
    internal-label: Personalization
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '224'
ht-degree: 79%
---
# 特定の IP をトラッキングから除外する {#exclude-specific-ips-from-being-tracked}

[!UICONTROL Web パーソナライゼーション]のトラッキングとレポートから自分の従業員や組織名を除外したい場合は、

個別の IP および IP の範囲の全部または一部を除外できます。

>[!NOTE]
>
>この処理は、完了までに最大 5 分かかる場合があります。

1. [!UICONTROL Web パーソナライゼーション]にログインし、ログインで、「**[!UICONTROL アカウント設定]**」をクリックします。

   ![](assets/image2014-11-19-19-3a25-3a41.png)

1. 「**[!UICONTROL IP の除外]**」領域まで下にスクロールします。 初めてIP アドレスを除外する場合は、空の「**[!UICONTROL IP アドレスを除外]**」フィールドをクリックします。

   ![](assets/image2016-11-4-10-3a27-3a1.png)

1. トラッキングおよびレポートから除外する個々の IP または IP の範囲を入力し、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/exclude-ips-form-hands.png)

   >[!NOTE]
   >
   >1 つの IPv4 または IPv6 アドレス、または全範囲、一部の範囲、あるいはサブネットマスクで指定した範囲を除外できます。 上記の例の項目は、Marketo フォーム自体に用意されている例に基づいて、それぞれ 1 つを示しています。

1. 「[!UICONTROL IP アドレスを除外]」フィールドに、入力した IP アドレスが一覧表示されます。 IP 除外を編集するには、緑色のプラス記号をクリックしてフォームを再度開きます。

   ![](assets/exclude-ips-after.png)

   簡単でしたよね？ これで、個別の IP または範囲別に追加された IP からすべてのデータを除外できます。
