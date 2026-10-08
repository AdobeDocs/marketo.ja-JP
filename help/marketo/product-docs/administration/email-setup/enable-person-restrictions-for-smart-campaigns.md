---
unique-page-id: 2360243
description: データベース全体に誤ってメールを送信するのを防ぐために、スマートキャンペーンの対象となるユーザーの最大数を設定します。
title: スマートキャンペーンの対象者制限の有効化
exl-id: 45bdaf3f-874c-493f-9746-440f7703713c
feature: Email Setup
TQID: 'https://experienceleague.adobe.com/6VwkOwN9nTqSyNcXvzyggPTk0Um5x1GPXIp2DBf2kww'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
    internal-label: Smart Campaigns
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
    internal-label: Database
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
    internal-label: Programs
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
    internal-label: Configuration
subfeature_v2:
  - id: a03c57fb-0705-4a0d-b463-bbc931d4cefa
    internal-label: Email setup
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '153'
ht-degree: 47%
---
# スマートキャンペーンの対象者制限の有効化 {#enable-person-restrictions-for-smart-campaigns}

Marketoには、スマートキャンペーンの対象となるユーザーの数を&#x200B;_最大_&#x200B;人に制限する機能があります。 これにより、データベース全体に誤ってメールが送信されるのを防ぎます。

>[!NOTE]
>
>**管理者権限が必要**

>[!CAUTION]
>
>これは、バッチキャンペーンとメールプログラムにのみ適用されます。

1. 「**[!UICONTROL 管理者]**」領域に移動します。

   ![](assets/enable-person-restrictions-for-smart-campaigns-1.png)

1. 「**[!UICONTROL スマートキャンペーン]**」をクリックします。

   ![](assets/enable-person-restrictions-for-smart-campaigns-2.png)

1. 「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/enable-person-restrictions-for-smart-campaigns-3.png)

   >[!CAUTION]
   >
   >スマートキャンペーンを実行する資格を持つユーザーの数が制限セットを超えた場合、まったく実行されません。

1. 制限を入力し、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/enable-person-restrictions-for-smart-campaigns-4.png)

   >[!TIP]
   >
   >この機能を無効にするには、フィールドを空白にします。

   >[!CAUTION]
   >
   >この制限はすべてのスマートキャンペーンに適用されますが、キャンペーンレベルで上書きできます。 [スマートキャンペーンでの人物制限の上書き](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/override-person-restrictions-in-a-smart-campaign.md)方法を参照してください。

>[!MORELIKETHIS]
>
>[スマートキャンペーンでの人物制限の上書き](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/override-person-restrictions-in-a-smart-campaign.md)
